# Power-Apps-and-Power-Automate
# Employee Onboarding Form

I have developed an Employee Onboarding Form using Power Apps to streamline the onboarding process for new hires. This custom app automates data collection, ensures accuracy, and improves the overall efficiency of onboarding.

**Database:** Dataverse  
**Environment:** Sandbox

## 1. Form Design

**Fields Included in the form:**
- First Name
- Last Name
- Job Title
- Upload Picture
- Department (Dropdown)
- Manager Name (Populated based on department selection)
- Manager Email (Automatically populated based on the manager’s name, retrieved from Active Directory)
- Start Date
- Phone Number
- Personal Email Address
- Equipment and software needed for position
- Orientation Status (Yes/No)

## 2. Interactive Features

- A '+' button allows users to add a new department manually.
- Upon form submission, the data is automatically saved to Dataverse.

## 3. Add Department

**Fields included in the add department page:**
- Department Name
- Assigned Manager
- Manager Email (Automatically populated based on the manager’s name, retrieved from Active Directory)
- Departments list
- Actions (Edit or Delete)

## 4. Validations

- First Name and Last Name must start with a capital letter.
- Email format validation.
- Date Picker restricts selection of previous dates.
- Phone Number contains only 11 digits and doesn’t contain any alphabets.
- A success pop-up appears when the submit button is clicked.
- An error pop-up appears if a required field is not filled in properly.

## 5. Form Functionality

- **Dropdown Logic:** Selecting a department automatically fills in the manager's name and email address.
- **Form Submission:** After submission, the data is saved in Dataverse. An automated email notification is then sent.
- **Email Notification:** After form submission, an email is automatically sent to the manager using their address retrieved from Active Directory in Office 365.

## 6. Automation

- **Power Automate Integration:** Outlines the automated flow in Power Automate that sends an email notification whenever the form is submitted.

## Benefits

- **Efficiency:** This form reduces the time required to gather employee information, automates repetitive tasks, and minimizes errors.
- **Scalability:** The form can be easily customized to meet the changing needs of the organization.
- **Seamless Integration:** It integrates smoothly with the company’s existing databases and systems, ensuring all information is up to date.

This employee onboarding form will significantly improve the onboarding process, allowing HR and managers to handle new hires more efficiently.
