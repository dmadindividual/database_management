# Self-Evaluation Form

## Overview

This is a web-based self-evaluation form designed to streamline the process of gathering and collating self-assessment data. The form is structured into two sections: "Skill Cluster" and "Technical Cluster." Each section allows users to input and save data, which can then be submitted and saved to a Google Sheet.

## Features

- **Dynamic Row Addition**: Users can dynamically add rows in both the "Skill Cluster" and "Technical Cluster" sections to input their self-evaluation data.
- **Data Validation**: Each row requires all fields to be filled before the data can be saved. Incomplete rows are highlighted with an error background.
- **Session Storage**: The data inputted is stored in the browser's session storage to ensure it persists during the user's session.
- **Google Sheets Integration**: The data is saved to a specified Google Sheet once the user finishes and submits the form. The data is submitted through the Google Sheets API.
- **OAuth Authentication**: Users are authenticated through Google's OAuth 2.0 service to gain access to the Google Sheets API.

## Technologies Used

- **HTML/CSS**: For structuring and styling the web page.
- **JavaScript**: For adding dynamic functionalities, handling events, and managing data.
- **Google Sheets API**: For saving data directly to a Google Spreadsheet.
- **Google OAuth 2.0**: For user authentication to access Google Sheets.

## Usage

### Adding a New Row

1. Click on the "Add Row" button in either the "Skill Cluster" or "Technical Cluster" section.
2. Fill out the fields: Title, Description, Self Score, Experience, and Assignment.
3. Once all fields are filled, the "Save" button becomes enabled. Click it to save the data.

### Deleting a Row

- To delete a row, click the "Delete" button next to the row you want to remove.

### Finishing and Submitting Data

- After entering all your data, click the "Finish" button to save your data to the Google Sheet. You will need to authenticate via Google to complete this action.

## Setup Instructions

1. **Clone the Repository**: Download the code and open the `index.html` file in a browser.
2. **Google API Configuration**:
   - Replace the `CLIENT_ID`, `API_KEY`, `SPREADSHEET_ID`, and `SHEET_NAME` with your own Google API credentials and the target spreadsheet information.
   - Ensure you have enabled the Google Sheets API in your Google Cloud project.

3. **Run the Application**:
   - Open the `index.html` file in a web browser.
   - Use the interface to add, edit, and submit your self-evaluation data.

### Prerequisites

- A Google account with access to Google Sheets.
- A Google Cloud project with the Sheets API enabled.
- A spreadsheet in Google Sheets where the data will be saved.

## Known Issues

- **Popup Blocker**: If the Google OAuth popup is blocked by your browser, you will need to allow popups to complete the authentication process.
- **Error Handling**: Rows that are incomplete will be highlighted. Users must complete all fields to enable the "Save" button.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributions

Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.

---

This `README` provides all the necessary details for understanding and using the Self-Evaluation Form web application.