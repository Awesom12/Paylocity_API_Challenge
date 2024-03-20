# Paylocity Benefits Dashboard application -  API Tests 

Welcome to our Project! This repository contains API tests implemented using Postman. Postman is a popular tool for API development and testing, offering a user-friendly interface for sending HTTP requests and analyzing responses.

## Project Overview
This project aims to automate API tests for Paylocity Benefits Dashboard application. These API tests are placed in **Paylocity API Challenge** workspace which is public and can be accessed with link: https://www.postman.com/research-observer-88949110/workspace/paylocity-api-challenge

## Pre-requisite
Postman installed on your machine.

## Getting Started
To get started with the project, follow these steps:

1. Clone this repository to your local machine.
2. Open Postman
3. Import the collections **Paylocity Challenge** and **DataDriven_NegTests**
4. Import the **PaylocityEnv** file to configure necessary environment variables.
5. Data from **PayData.csv** file can be used to run the **DataDriven_NegTests** collection from collection runner or CLI.

## Workspace **Paylocity API Challenge** structure
The workspace is organised into collections, folders and requests, each representing a different aspect or endpoint of the API. <br/>
**Paylocity Challenge** collection is organised into 4 folders
- **Negative Security Tests:** This folders consists of security requests which verifies the response for various invalid inputs.
- **Happy Path Tests:** This folders consists of requests which verifies the response with known inputs.
- **Negative Tests_PUT & GET:** This folders consists of PUT & GET requests which verifies the response for invalid inputs.
- **Delete - Looping Request:** This folder consists of a Delete request which is looped for 3 times.<br/><br/>

The **DataDriven_NegTests** collection has POST and PUT requests those can be run with different invalid values.


## Running Tests
To run the tests:

- Select **PaylocityEnv**  and ensure your environment variables are correctly set.
- Each request can be separately run on Postman or the entire collection or a single folder in Collection Runner or on CLI using newman.
- Select **PayData.csv** data file when running **DataDriven_NegTests** collection
- Review the test results.