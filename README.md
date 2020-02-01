HW #5 Create a simple calendar application that allows the user to save events for each hour of the day. This app will run in the browser and feature dynamically updated HTML and CSS powered by jQuery.

Intro:
------------
This is my fourth homework Assignment for UCSD Extension Coding Bootcamp.

- I will build a work-day scheduler using JavaScript, web APIs and moment.js.


Instructions:
------------
Instructions are located in the readme.md file in the following location: 
https://ucsd.bootcampcontent.com/UCSD-Coding-Bootcamp/UCSD-SD-FSF-PT-12-2019-U-C/blob/master/05-Third-Party-APIs/02-Homework/README.md


Resources used:
------------
- Bootstrap CSS CDN - https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css
- fontawesome       - https://use.fontawesome.com/releases/v5.8.1/css/all.css
- google apis       - https://fonts.googleapis.com/css?family=Open+Sans&display=swap
- jQuery CDN        - https://code.jquery.com/jquery-3.4.1.min.js
- library              - https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.24.0/moment.min.js



Reference:
------------
- 05-third-party-apis-homework-demo.gif


Comprehension Check
------------
- What is jQuery? --> jQuery is a JavaScript library.

- What is the difference between a library and a framework? --> A library is a set of tools that you can call into your code, whereas a framework is a prebuilt model that calls for pieces of your code.  When using a library, you are in control of the flow, and can use the tools for any purpose.  When using a framework, the framework is in control of the flow, and allows for a set of prefabbed outcomes, and can accept your code for cusomizations.

- Why is dynamically generated HTML an issue for developers working with jQuery? --> jQuery functions inside of dynamically generated html will not work correctly. A workaround is to use event delegation, such as preventDefault().




Progress:
------------
2020.01.31.0330 - Initial commit.  Setup folder structure, and initialized the readme. Created asset-list.txt in assets folder and moved 05-third-party-apis-homework-demo.gif into a newly created reference folder.  Added script section to bottom of index.html, and created document(ready) function.  In this function I linked up the element with the id of 'currentDay' to moment.js.  I also added some comments to the code to explain each section.

2020.01.31.0335 - Corrected timestamp of previous commit. Updated code using moment.js library to conform to correct date format for project.

2020.01.31.0424 - Added pseudocode to index.html. Added for loop that will build the timeblocks rows and columns, though the function is WIP.

2020.01.31.0540 - For index.html, I completed first pass of 'createTimeBlocks' function, and added comments to explain process.

2020.01.31.0705 - For index.html, I reviewed first pass of 'createTimeBlocks' function, and completed second pass of said function, altering the for loop tp create 2 timeblocks, and adding conditional statements to seperate the timeblocks into 'am' vs 'pm'.

2020.01.31.0710 - Corrected timestamp of previous commit. For index.html, I added code to set the textarea to 100% width of its parent column.

2020.01.31.2005 - For index.html, I added more comments and console.logs to the script area of the code to further detail code and to allow quality control through console.  I changed the local variables 'textStamp' and 'hourStamp' to be global.

2020.01.31.2030 - For index.html, I added more comments and console.logs to the script area of the code to further detail the code and to allow for ease of quality control through console.  I moved the function 'setRowColors()' inside of the function 'createTimeBlocks()' near the end of the function.  This allowed for colors to dynamically appear in the textareas based on what the current time is.