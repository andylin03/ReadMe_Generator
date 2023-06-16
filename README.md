# ReadMe Generator and Node.js

# Description 
The what, why, and how:

Every good project needs a quality README with information about the app - what the app is for, how to use the app, how to install it, how to report issues, and how to make contributions so that other developers are more likely to use and contribute to the success of the project.

This is a command-line application that runs with Node.js that dynamically generates a README.md file based on input about your project.

# User Story 
AS A developer
I WANT a README generator
SO THAT I can quickly create a professional README for a new project

# Acceptance Criteria 
GIVEN a command-line application that accepts user input
WHEN I am prompted for information about my application repository
THEN a high-quality, professional README.md is generated with the title of my project and sections entitled Description, Table of Contents, Installation, Usage, License, Contributing, Tests, and Questions
WHEN I enter my project title
THEN this is displayed as the title of the README
WHEN I enter a description, installation instructions, usage information, contribution guidelines, and test instructions
THEN this information is added to the sections of the README entitled Description, Installation, Usage, Contributing, and Tests
WHEN I choose a license for my application from a list of options
THEN a badge for that license is added near the top of the README and a notice is added to the section of the README entitled License that explains which license the application is covered under
WHEN I enter my GitHub username
THEN this is added to the section of the README entitled Questions, with a link to my GitHub profile
WHEN I enter my email address
THEN this is added to the section of the README entitled Questions, with instructions on how to reach me with additional questions
WHEN I click on the links in the Table of Contents
THEN I am taken to the corresponding section of the README

# Screenshot


<img width="995" alt="Screenshot 2023-06-16 at 10 38 33 AM" src="https://github.com/andylin03/ReadMe_Generator/assets/126199540/badf9e36-6f99-4b2e-8d3a-bdabe40d8d5a">





# Installation 
To generate your own README, git clone the repo down to your local so you have the Node project on your local.

Run npm i inquirer@8.2.4 in order to install the following npm package dependencies as specified in the package.json:

The application will start by running node index.js in the command line.

Answer the prompts in your command line to generate the README.

After answering all the prompts, your README file will be named 'ExampleREADME.md' and will be ready for you at the root of the repo.

The README has some automatically generated badges for your repo courtesy of shields.io and will include your profile picture & email from GitHub.

# Usage
When you run node index.js, the application uses the inquirer package to prompt you in the command line with a series of questions about your GitHub and about your project.

Finally, fs.writeFile is used to generate your project's README.md file. Check out the [ExampleREADME.md] in this repo as an example on the final output.

# Methodology
The application utilizes modularization by separating the GitHub API call and generation of the markdown into separate modules: api.js and generateMarkdown.js, respectively, inside the utils folder.

The application also utilizes, as much as possible, syntax and paradigms introduced in ES6 and beyond, including:

Arrow functions,
const, let,
Template literals, and
async/await to handle inquirer and fs.writeFile promises.

# License 
MIT License
