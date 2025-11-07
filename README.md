# NUnit/Selenium Test Automation Assistant

This is a web application built with Flask that utilizes the Google Gemini API to provide assistance with C# test automation using NUnit, Selenium, and the Page Object Model.

## Features

- **Generate NUnit Test Case:** Create a new test case from a description.
- **Generate Page Object Class:** Create a new Page Object Model class.
- **Debug Code:** Find and fix errors in your NUnit/Selenium code.
- **Explain Code:** Get an explanation of a piece of NUnit/Selenium code.
- **Suggest Refactoring:** Receive suggestions for improving your test code.
- **Write Documentation:** Generate documentation for your test code.
- **Dark/Light Mode Toggle**

## Setup

1.  Clone the repository.
2.  Install dependencies: `pip install -r requirements.txt`
3.  Create a `.env` file in the project root with your Gemini API key: `GEMINI_API_KEY=YOUR_API_KEY`
4.  Run the application: `python gemini_agent_app.py`

## Usage Example

To generate a new NUnit test case for a login page, you would:

1.  **Select Action:** Choose `Generate NUnit Test Case` from the dropdown.
2.  **Enter Prompt or Code:** In the text area, enter a description of the test case you want to create. For example:

    ```
    Create a test case that navigates to the login page, enters a username and password, and verifies that the user is successfully logged in.

    - The login page URL is "http://example.com/login"
    - The username input field has an ID of "username"
    - The password input field has an ID of "password"
    - The login button has an ID of "login-button"
    - A successful login is indicated by the presence of an element with the ID "welcome-message"
    ```

3.  Click **Get Assistance**. The assistant will then generate the C# code for the NUnit test case.
