# Warrior Tech Support Logging System
If you would like to download the project to check it out, please download the zip, unzip it, and run the `index.html`

## To input data into a spreadsheet
- Open up the desired spreadsheet and go to `Tools` and click `Script Editor`.
- Rename the script to Submit Form to Google Sheets.
- Now, delete the `function myFunction() {}` block within the `Code.gs` tab. In the zip open the `google_sheets_script.txt`, 
copy the text, then paste it into the google script and go to `File` then `Save`. 
- Next, go to `Run > Run Function > initialSetup` to run this function.
- In the `Authorization Required` dialog, click on `Review Permissions`.
- Sign in or pick the Google account associated with this projects.
- You should see a dialog that says `Hi {Your Name}`, `Submit Form to Google Sheets wants to`...
- Click `Allow`
## Add a new project trigger
- Click on `Edit > Current project’s triggers`.
- In the dialog click `No triggers set up. Click here to add one now`.
- In the dropdowns select `doPost`
- Set the events fields to `From spreadsheet` and `On form submit`
- Then click `Save`
## Publish the project as a web app
- Click on `Publish > Deploy as web app…`.
- Set `Project Version` to `New` and put `initial version` in the input field below.
- Leave `Execute the app as:` set to `Me(your@address.com)`.
- For `Who has access to the app:` select `Anyone, even anonymous`.
- Click `Deploy`.
- In the popup, copy the `Current web app URL` from the dialog.
- And click `OK`.
> IMPORTANT! If you have a custom domain with Gmail, you might need to click `OK`, refresh the page, and then go to 
`Publish > Deploy as web app…` again to get the proper web app URL. 
It should look something like `https://script.google.com/a/yourdomain.com/macros/s/XXXX…`.
## Input your web app URL
- Open the file named `index.html`. On line 64 replace the current URL in the `''` with your script URL
## Setting up your spreadsheet
In the spreadsheet, for the values you will need are **timestamp**, **student_name**, **log**, **final_inspection_needed**, and **chromes_worked_on** at the top of collumns A - E.
> IMPORTANT! These are case sensitive and each one needs to be in a seperate cell collumn.
