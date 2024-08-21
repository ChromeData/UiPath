# UiPath
Robotic process automation (RPA) is a technology that allows for the creation, deployment, and management of software robots that mimic human interactions with digital systems. These robots can read screens, input keystrokes, navigate systems, and extract data, performing tasks more quickly and consistently than humans without breaks.

# Building 5 Bots to Automate tasks on UiPATH + Azure Lab


## Weather Automation Workflow - Bot #1
This UiPath project automates the process of fetching weather information for any given city. It begins by prompting the user to enter a city name, then searches for the current weather on Google, and logs both the temperature and weather conditions. The workflow efficiently retrieves and displays relevant weather details using simple user interactions.

![Screenshot 2024-08-21 180441](https://github.com/user-attachments/assets/c435e55c-f63d-4333-8853-36234c03e534) 




1. Input Dialog: Get City Name
Purpose: Prompts the user to enter the name of a city.
Details:
Dialog Title: "Get the weather"
Input Label: "Enter a city name"
Input Type: Text box
Variable: CityName (stores the user input)


3. Write City Name
Purpose: Demonstrates the use of the CityName variable, possibly preparing it for further actions.


4. Open Google
Purpose: Opens Google's homepage in the default web browser.
Details:
URL: https://www.google.com/


5. Weather Details Interaction
Purpose: Automates the entry of the city name into Google's search bar to find weather details.
Details:
Type Into Action: Types "weather in " + CityName into Google's search bar and hits Enter to search.


6. Keyboard Shortcut (Enter Key)
Purpose: Ensures the search is executed by simulating an Enter key press.


7. Get Temperature
Purpose: Extracts the temperature from the Google search results.
Variable: Temperature (stores the extracted temperature)


8. Log Temperature
Purpose: Logs the extracted temperature for debugging or record-keeping.
Details:
Log Message: "Temperature: " + Temperature


9. Get Weather Description
Purpose: Extracts a brief description of the weather conditions from the search results.
Variable: Weather (stores the weather description)
Summary:
This workflow automates the process of fetching and logging weather details from Google based on a user-specified city. It demonstrates various UiPath activities like input handling, browser automation, data extraction, and logging. This sequence is particularly useful for learning about UiPath's capabilities in integrating web-based data extraction into automation workflows.



## UiPath Web Data Handling Workflow - Bot #2
This repository contains a UiPath workflow designed to automate the process of data extraction from a web application, specifically from a CRM-like system. The automation sequence involves reading customer data from an Excel file, inputting this data into a web form, and managing the customer information effectively within the application.

This UiPath workflow demonstrates an automation process for extracting and handling data from a excel sheet to be entered in a web application.



https://github.com/user-attachments/assets/948cae7e-9aa8-4e4f-a869-b379242875f0



1. **Read Customer Data from Excel:** The workflow starts by reading customer data stored in an Excel file into a DataTable, which is then processed in subsequent steps.

2. **Open Browser and Navigate to CRM:** A web browser is opened, and the workflow navigates to the CRM system where customer data will be managed.

3. **Data Entry Automation:**
   - For each customer (row in the DataTable), the workflow performs the following actions:
     - Input the customer's first and last names into the corresponding fields in the web form.
     - Depending on the gender specified in the Excel file, the workflow selects the appropriate gender option in the form.
     - Other customer details such as address, city, and contact information are also entered into the form.

4. **Submit Customer Data:** After all fields are filled, the workflow clicks the 'Add' button to submit the data, thereby creating or updating a customer record in the CRM.

5. **Error Handling and Logging:** Throughout the execution, the workflow includes error handling and logging mechanisms to ensure robust automation and ease of troubleshooting.

**Tools and Technologies Used:**
- UiPath Studio for workflow design and execution.
- Excel for storing initial customer data.
- Web-based CRM system for customer data management.

**Purpose and Benefits:**
- Automates repetitive data entry tasks, reducing manual effort and error rates.
- Enhances data processing speed and accuracy in customer relationship management.


