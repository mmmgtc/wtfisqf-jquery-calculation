# Quadratic Funding Calculator

## Description

This is a simple web application that calculates quadratic funding matches for multiple projects. The application is implemented in JavaScript and utilizes jQuery for UI manipulation and event handling.

Quadratic funding is a mechanism that optimizes the funding of public goods. It increases the impact of small contributions by calculating matching amounts using a quadratic formula. 

## Features

1. Enter a matching amount to be divided among the projects.
2. Add and remove projects.
3. Add and remove contributions to projects.
4. Calculate match amounts based on entered contributions and display them in the table.
5. Copy the current state of the calculator to the URL for sharing.
6. Reload the calculator's state from the URL parameters.

## Usage

Open the HTML file in a web browser to start using the application. 

- To change the total matching amount, edit the "Matching Amount" input field.
- To add a project, click the "Add Project" button.
- To remove a project, click the remove button ("X") in the project row.
- To add a contribution to a project, type the contribution amount in the project row's input field and press Enter.
- To remove a contribution, click the remove button ("X") next to the contribution.
- The "Funded Amount" column shows the sum of all contributions to the project.
- The "Match Amount" column shows the calculated match for the project based on its contributions and the total matching amount.
- To copy the current state of the calculator (matching amount, projects, and their contributions) to the URL for sharing, click the "Copy URL" button.

## Requirements

This application requires a web browser that supports JavaScript and the jQuery library. jQuery is included in the HTML file from a CDN.

## Notes

- This application uses the browser's history API to save and load its state from the URL. This feature might not work correctly if the file is opened as a local file (with a `file://` URL) in some browsers due to their security restrictions. To fully use this feature, serve the HTML file from a web server.
- The application does not have any backend or persist the data. If you refresh the page or close the browser, all data will be lost unless saved in the URL.
- The application does not perform any input validation. It's assumed that the users will enter positive numbers as the matching amount and contributions.

## Contact

Please feel free to contact the author if you have any questions or issues.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
