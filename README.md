# Script Element Placement

This demo illustrates why it is important to position the `<script src="">` element at the end of the `<body>` element.

If the `<script>` element contains code that modifies an element that is further down in the HTML document, then that element will not have been loaded by the web browser at the time when the script code is executed.

The demo has a script element, that modifies the text color of the h1 with the id="title" element. 

#### Place the `<script>` before the `<h1>` element
The script causes a runtime error because the `<h1>` element hasn't been loaded by the web browser at the time when the script is executed. You can show the error in the console.

#### Place the `<script>` after the `<h1>` element
The script runs without error and changes the color of the text to red.



