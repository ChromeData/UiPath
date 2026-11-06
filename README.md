# UiPath Automation Bots

Three software robots built in UiPath Studio that do repetitive computer work on their own: looking things up, entering data and collecting it from websites.

## Bot 1: Weather lookup

You type a city name. The bot searches Google for that city's weather, then pulls out and logs the temperature and conditions.

![Weather bot](https://github.com/user-attachments/assets/c435e55c-f63d-4333-8853-36234c03e534)

**How it works:** input box for the city → open Google → search "weather in [city]" → grab the temperature and description → write them to the log.

## Bot 2: Excel to web form data entry

Reads a list of customers from an Excel file and types each one into a web CRM form, then submits it. This replaces manual copy and paste.

https://github.com/user-attachments/assets/948cae7e-9aa8-4e4f-a869-b379242875f0

**How it works:**
- Loads the Excel sheet into a data table.
- For each customer: fills in name, gender, address, city and contact details, then clicks Add.
- Logs each step and handles errors so one bad row doesn't stop the run.

## Bot 3: Real estate scraper

You type a city name. The bot searches Zillow, collects the listings and exports them to an Excel spreadsheet with price, bedrooms, bathrooms and location.

https://github.com/user-attachments/assets/8a485b50-77e5-4528-bed2-f17320a8a456

**How it works:** open Zillow → search the city → read each listing's details → save everything to Excel → close the browser.

**Built with:** UiPath Studio, Excel, web automation
