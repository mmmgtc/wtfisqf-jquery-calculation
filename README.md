## Quadratic Funding Calculator

The script implements a quadratic funding mechanism, a method of public funding that incentivizes community participation. Written in JavaScript and jQuery, it provides an interactive interface where users can add, edit, and remove projects and their respective contributions. 

### Key Components

1. **Initialization of Parameters**  
   The script first initializes match amount and an array of projects, using values provided as URL parameters or defaults if parameters do not exist.

   ```javascript
   let quadraticFunding = {
     matchAmount: params.get('matchAmount') ? parseFloat(params.get('matchAmount')) : 1000,
     projects: params.get('projects') ? JSON.parse(params.get('projects')) : [],
   };
   ```

2. **Update URL Function**  
   The `updateUrl()` function updates the URL to reflect the current state of the application.

3. **HTML Elements Creation**  
   The script dynamically creates necessary HTML elements, such as inputs for the match amount and new project names, a button to add a new project, and a table to display project details.

4. **Event Handlers**  
   Various events are set up to handle user interactions, such as typing in the match amount input, clicking the 'Add Project' or 'Remove Project' buttons, entering a contribution, and clicking the 'Remove Contribution' button.

5. **Quadratic Funding Calculation**  
   The `calculateMatchAmounts()` function calculates the match amount for each project based on the quadratic funding formula: `(sum(sqrt(contribution))^2 / total) * matchAmount`.

6. **Initial Data Population**  
   The script can pre-fill the application with data from the projects array, populating the project names, contributions, and recalculating the match amounts accordingly.

### Usage

Simply run the script on your web page. It requires jQuery to operate. You can interact with the application by entering a match amount, adding projects, and specifying their contributions. The script will automatically calculate and display the match amounts for each project in real time.
