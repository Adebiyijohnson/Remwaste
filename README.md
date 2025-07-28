**Readme for Remwaste UI Automation and API Automation**

**UI Automation**
Note: The page object method was used in this project(POM)

 **Features Covered**
- Login with valid and invalid credentials
- Add product to cart
- Update quantity in cart
- Remove product from cart
- Assert success/error messages

**Install Cypress**
npm init -y
npm install cypress --save-dev

**Add Page Object Files**
Create the following files in cypress/support/pageObjects/:
HomePage.js
LoginPage.js
CartPage.js

**Create cartFlow.cy.js under cypress/e2e/**
Write the step definition and POM Scripts
include all assertions covering all scenarios 

**Run the test**
npx cypress open


**API Automation**

   **Prerequisites**
- Download Postman
- Download Node.js

   **Running Tests in Postman GUI**
- Open Postman Desktop App.
- Create the collection:
- Set the environment in the top-right dropdown.
- Select the collection → Click "Run".
- You can also view results via Test Results tab.

**Running Tests in CLI (with Newman)**
Install Newman globally: npm install -g newman
Run the test collection:newman run postman/remwastecollection.json

**Github Actions**
Create a github folder and a yml file
add your script
To Trigger the Tests
Push any commit or open a pull request to the main branch. GitHub Actions will automatically:
Install Node.js and project dependencies.
Run Cypress UI tests.
Run Newman API tests.
Upload API test results.

**Author
Adebiyi Johnson
Email: adebiyijohnson164@gmail.com**
