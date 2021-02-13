# Comments

    * It will not touch the code 
    * Helps to remember the code blocks
    * Puts tips to reading 
    * Helps other people to understand 
    * Never forget to close an open comment 
    * We can use a comment to disable parts of the code

    Comments starts with /* and finishes with */

```CSS

/* Basic */
/* ------------------------------------------------------- */

body {
    font: 1em/150% Helvetica, Arial, sans-serif;
    padding: 1em;
    margin: 0 auto;
    max-width: 33em;
}

@media (min-width:  70em) {
    body {
        font-size: 130%;
    }
}


/* Specific Elements */
/* ------------------------------------------------------- */

div p, #id:first-line {
    background-color: red;
    border-radius: 3px;
}

div p {
    margin: 0;
    padding: 1em;
}

div p + p {
    padding-top: 0;
}

p {
    color: blue;
}

```