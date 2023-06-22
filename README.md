
# Testing Countdown API

The objective of this project is to thoroughly test the Countdown API, specifically focusing on its various eBay search endpoints. The Countdown API provides functionalities for searching items, retrieving product details, accessing customer reviews, obtaining seller data, exploring deals, and generating item suggestions. To accomplish this, the project will utilize Postman, a popular API testing tool that allows for efficient testing, automation, and validation of API endpoints. The testing approach will involve API chaining, multiple assertions, and data-driven testing techniques to ensure comprehensive coverage and robust validation of the Countdown API.

## Features

- API Chaining
- JSON Test Results
- HTML Test Results
- Multiple Assertions
- Data Driven Testing

## Countdown API Assertions

- Validate Response Contains/Not Contains
- Validate Query Parameters
- Validate Response Format
- Validate Response Time
- Validate Match Content
- Validate Status Codes

## Testing Process

https://user-images.githubusercontent.com/91252395/220158333-f2fc8c6d-0892-4e8d-9734-162db5cb18ff.mp4

## Test Report

![test report photo](https://user-images.githubusercontent.com/91252395/220152826-303461da-f8dc-4f89-b1ff-a13b3878f914.PNG)

## Setup without newman

- Install Postman and create an account

- Create an account and login on rapidapi.com

- Subscribe for the countdown api at: https://rapidapi.com/traject-data-traject-data-default/api/countdown4

- Copy the available API Key

- Import Ebay Search API or Ebay Search API DDT Collection available in Collections folder into postman

- Modify the QA Environment json file available in Environment folder with your Rapidapi API key

- Import the QA Environment json file into postman

- Click on view more actions near the collection

- Click on run collection

- If you use Ebay Search API DDT Collection click on 'select file' and import the test data

- Hit Run Ebay Search Api

## Setup with newman

- Install Postman and create an account

- Create an account and login on rapidapi.com

- Subscribe for the countdown api at: https://rapidapi.com/traject-data-traject-data-default/api/countdown4

- Copy the available API Key

- Modify the QA Environment json file available in Environment folder with your Rapidapi API key

- Install Node JS

- Install Newman: npm install newman

- Install Newman-reporter-html: npm install newman-reporter-html

- Modify the paths in the command and run the collection with: newman run path_to_collection.json --environment path_to_environment.json --reporters html --reporter-html-export path_to_save_html_report.html --delay-request 15000

- If you want to use the Ebay Search API DDT Collection then modify and use this command: newman run path_to_collection.json --environment path_to_environment.json --iteration-data path_to_data_file.json --reporters html --reporter-html-export path_to_save_html_report.html --delay-request 15000

