
# Testing Countdown API

Countdown API provides various ebay search endpoints for searching items, product details, customer reviews, seller data, deals and item suggestions. Testing Countdown API endpoints using postman with API chaining, multiple assertions and data driven testing.

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



## Test Report



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

