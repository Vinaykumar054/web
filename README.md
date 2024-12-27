[Type the document title]
WEB TECHNOLOGY LAB - BCSL504
2024-25
D E P A R T M E N T O F C O M P U T E R S C I E N C E & E N G I N E E R I N G , R Y M E C , B A L L A R I
1. Develop the HTML page named as “Myfirstwebpage.html”. Add the following
tags with relevant content.
i. Set the title of the page as “My First Web Page”
ii. Within the body use the following tags:
a) Moving text = “Basic HTML Tags”
b) Different heading tags (h1 to h6)
c) Paragraph
d) Horizontal line
e) Line Break
f) Block Quote
g) Pre tag
h) Different Logical Style (<b>, <u>, <sub>, <sup> etc.)
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>My First Web Page</title>
 </head>
 <body>
 <marquee>Basic HTML Tags</marquee>
 <h1>Heading 1</h1>
 <h2>Heading 2</h2>
 <h3>Heading 3</h3>
 <h4>Heading 4</h4>
 <h5>Heading 5</h5>
 <h6>Heading 6</h6>
 <p>This is a paragraph.</p>
 <hr>
 <p>This is a paragraph with a <br> line break.</p>
 <blockquote>
 "This is a block quote."
 </blockquote>
 <pre>
 This is a pre-formatted text.
 </pre>
 <strong>This is a strong text.</strong>
<p>This is <b>bold</b> text.</p>
 <p>This is <i>italicized</i> text.</p>
 <p>This is <u>underlined</u> text.</p>
 <p>This is <sup>superscript</sup> text.</p>
 <p>This is <sub>subscript</sub> text.</p>
 </body>
 </html>

OR
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>My First Web Page</title>
 <!-- <style>
 body {
 font-family: Arial, sans-serif;
 line-height: 1.6;
 margin: 0;
 padding: 20px;
 }
 </style> -->
 <link rel="stylesheet" href="style.css">
</head>
<body>
 <marquee>Basic HTML Tags</marquee>
 <h1>This is Heading 1</h1>
 <h2>This is Heading 2</h2>
 <h3>This is Heading 3</h3>
 <h4>This is Heading 4</h4>
 <h5>This is Heading 5</h5>
 <h6>This is Heading 6</h6>
 <p>This is a paragraph. It demonstrates the use of the paragraph tag in HTML.
Paragraphs are used to group related content together.</p>
 <hr>
 <p>This is another paragraph.<br>This text appears on a new line due to the line
break tag.</p>
 <blockquote>
 This is a block quote. It's often used to highlight quoted text from another source.
 </blockquote>
 <pre>
This is preformatted text.
It preserves both spaces and
line breaks, making it useful
for displaying code or ASCII art.
 </pre>
 <p>
 Here are examples of logical styles:<br>
 <b>Bold text</b><br>
 <i>Italic text</i><br>
 <u>Underlined text</u><br>
 <strong>Strong text</strong><br>
 <em>Emphasized text</em><br>
 Text with <sub>subscript</sub> and <sup>superscript</sup>
 </p>
</body>
</html>
2.Develop the HTML page named as “Table.html” to display your class time table.
a) Provide the title as Time Table with table header and table footer, row-span
and col-span etc.
b) Provide various colour options to the cells (Highlight the lab hours and elective
hours with different colours.)
c) Provide colour options for rows.
<!DOCTYPE html>
<html>
<head>
 <title>Time Table</title>
 <style>
 body {
 font-family: Arial, sans-serif;
 line-height: 1.6;
 margin: 0;
 padding: 20px;
 }
 table {
 width: 100%;
 }
 th, td {
 border: 1px solid #ddd;
 padding: 8px;
 text-align: center;
 }
 th {
 background-color: #f2f2f2;
 }
 .lab-hours {
 background-color: #ffcccb;
 }
 .elective-hours {
 background-color: #90ee90;
 }
 .lunch {
 background-color: #ffd700;
 }
 .odd-row {
 background-color: #f8f8f8;
 }
 tfoot {
 background-color: #e6e6e6;
 font-weight: bold;
 }
 </style>
</head>
<body>
 <table>
 <thead>
 <tr>
 <th colspan="7">Class Time Table</th>
 </tr>
 <tr>
 <th>Time</th>
 <th>Monday</th>
 <th>Tuesday</th>
 <th>Wednesday</th>
 <th>Thursday</th>
 <th>Friday</th>
 <th>Saturday</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <td>9:00 - 10:00</td>
 <td>UNIX</td>
 <td>SE</td>
 <td>CN</td>
 <td>TC</td>
 <td>WP</td>
 <td rowspan="6">No Classes</td>
 </tr>
 <tr class="odd-row">
 <td>10:00 - 11:00</td>
 <td>SE</td>
 <td>UNIX</td>
 <td>TC</td>
 <td class="elective-hours">UNIX</td>
 <td class="elective-hours">RM</td>
 </tr>
 <tr>
 <td>11:00 - 12:00</td>
 <td class="lab-hours" colspan="2">CN LAB</td>
 <td class="lab-hours" colspan="2">WP LAB</td>
 <td class="lab-hours">RM</td>
 </tr>
 <tr class="odd-row">
 <td>12:00 - 13:00</td>
 <td class="lunch" colspan="5">Lunch Break</td>
 </tr>
 <tr>
 <td>13:00 - 14:00</td>
 <td>TC</td>
 <td>UNIX</td>
 <td>SE</td>
 <td>CN</td>
 <td>WP</td>
 </tr>
 <tr class="odd-row">
 <td>14:00 - 15:00</td>
 <td class="elective-hours">UNIX</td>
 <td class="elective-hours">RM</td>
 <td class="lab-hours" colspan="3">WP LAB</td>
 </tr>
 </tbody>
 <tfoot>
 <tr>
 <td colspan="7">* Lab hours are highlighted in pink, elective hours in light
green</td>
 </tr>
 </tfoot>
 </table>
</body>
</html>
OR
<!DOCTYPE html>
<head>
 <title>Time Table</title>
 <style>
 body {
 font-family: Arial, sans-serif;
 }
 table {
 width: 80%;
 margin: 20px auto;
 border-collapse: collapse;
 }
 th,
 td {
 border: 1px solid #ddd;
 padding: 8px;
 text-align: center;
 }
 th {
 background-color: #f4f4f4;
 color: #333;
 }
 tr:nth-child(even) {
 background-color: #f9f9f9;
 }
 tr:nth-child(odd) {
 background-color: #e6f7ff;
 }
 .lab-hour {
 background-color: #ffcccc;
 }
 .elective-hour {
 background-color: #ccffcc;
 }
 .highlight {
 font-weight: bold;
 color: #d63384;
 }
 tfoot {
 background-color: #e0e0e0;
 font-weight: bold;
 }
 </style>
</head>
<body>
 <h1 style="text-align: center;">Time Table</h1>
 <table>
 <thead>
 <tr>
 <th>Day/Time</th>
 <th>9:00 - 10:00</th>
 <th>10:00 - 11:00</th>
 <th>11:00 - 12:00</th>
 <th>12:00 - 1:00</th>
 <th>Lunch Break</th>
 <th>2:00 - 3:00</th>
 <th>3:00 - 4:00</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <td>Monday</td>
 <td>UNIX</td>
 <td>SE</td>
 <td class="lab-hour">CN Lab</td>
 <td>Elective-RM</td>
 <td rowspan="5" class="highlight">Break</td>
 <td class="elective-hour">CN</td>
 <td>TC</td>
 </tr>
 <tr>
 <td>Tuesday</td>
 <td class="elective-hour">Elective-RM</td>
 <td>UNIX</td>
 <td>SE</td>
 <td class="lab-hour">CN Lab</td>
 <td>CN</td>
 <td>RM</td>
 </tr>
 <tr>
 <td>Wednesday</td>
 <td>UNIX</td>
 <td class="lab-hour">WP Lab</td>
 <td>SE</td>
 <td>TC</td>
 <td>SN</td>
 <td class="elective-hour">Elective-RM</td>
 </tr>
 <tr>
 <td>Thursday</td>
 <td>TC</td>
 <td>CN</td>
 <td>UNIX</td>
 <td class="elective-hour">Elective-RM</td>
 <td>SE</td>
 <td>SE</td>
 </tr>
 <tr>
 <td>Friday</td>
 <td class="lab-hour">WP Lab</td>
 <td>SE</td>
 <td>UNIX</td>
 <td>CN</td>
 <td class="elective-hour">Elective-RM</td>
 <td>TC</td>
 </tr>
 </tbody>
 <tfoot>
 <tr>
 <td colspan="8">End of Timetable</td>
 </tr>
 </tfoot>
 </table>
</body>
</html>
3. Develop an external style sheet named as “style.css” and provide different
styles for h2, h3, hr, p, div, span, time, img & a tags. Apply different CSS selectors
for tags and demonstrate the significance of each.
3.html
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Sample Styled Page (No Div)</title>
 <link rel="stylesheet" href="style.css">
</head>
<body>
 <main id="main-content">
 <h2>Welcome to Our Styled Page</h2>
 <p>This is a paragraph right after an h2. It demonstrates the adjacent sibling
selector.</p>
 <h3>Hover over me!</h3>
 <hr>
 <p lang="en">This paragraph has a lang attribute, demonstrating the attribute
selector.</p>

 <p>Here's a <span class="highlight">highlighted</span> word using the class
selector.</p>
 <section>
 <p>This paragraph is inside a section, showing the descendant selector.</p>
 <span>This span is a direct child of the section.</span>
 </section>
 <p>The current date and time: <time datetime="2024-08-15">August 15,
2024</time></p>
 <p>Notice how the first letter of each paragraph is styled differently.</p>
 <article class="special">
 <p>This paragraph is inside an article with class="special".</p>
 </article>
 <img src="https://rymec.edu.in/wp-content/uploads/2023/03/baim5.png"
alt="A placeholder image">
 <p>Check out this <a href="https://rymec.edu.in/">link</a> to see different
link states.</p>
 </main>
</body>
</html>
style.css
/* Element Selector */
h2 {
 color: #2c3e50;
 font-family: 'Arial', sans-serif;
 border-bottom: 2px solid #3498db;
 padding-bottom: 10px;
}
/* Element Selector with Pseudo-class */
h3:hover {
 color: #e74c3c;
 cursor: pointer;
 transition: color 0.3s ease;
}
/* Element Selector */
hr {
 border: 0;
 height: 1px;
 background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0,
0, 0, 0));
}
/* Element Selector with Attribute */
p[lang] {
 font-style: italic;
}
/* Class Selector */
.highlight {
 background-color: #f1c40f;
 padding: 5px;
}
/* ID Selector */
#main-content {
 max-width: 800px;
 margin: 0 auto;
 padding: 20px;
 background-color: #ecf0f1;
}
/* Descendant Selector */
div p {
 line-height: 1.6;
 margin-bottom: 15px;
}
/* Child Selector */
div > span {
 font-weight: bold;
 color: #16a085;
}
/* Adjacent Sibling Selector */
h2 + p {
 font-size: 1.1em;
 color: #7f8c8d;
}
/* Attribute Selector */
time[datetime] {
 color: #8e44ad;
 font-weight: bold;
}
/* Pseudo-element Selector */
p::first-letter {
 font-size: 1.5em;
 font-weight: bold;
 color: #c0392b;
}
/* Multiple Selectors */
img, a {
 border: 1px solid #bdc3c7;
 padding: 5px;
}
/* Pseudo-class Selector for Links */
a:link, a:visited {
 color: #3498db;
 text-decoration: none;
}
a:hover, a:active {
 color: #e74c3c;
 text-decoration: underline;
}
/* Attribute Selector for Images */
img[alt] {
 max-width: 100%;
 height: auto;
}
/* Combining Selectors */
div.special p {
 text-indent: 20px;
 color: #27ae60;
}
OR
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Styled HTML Elements</title>
 <link rel="stylesheet" href="style.css">
</head>
<body>
 <h2>This is an H2 Heading</h2>
 <h3>This is an H3 Heading</h3>
 <hr>
 <p>This is a paragraph with some <span>highlighted text</span> using a span
element.</p>
 <div>
 <p>This paragraph is inside a div element with a background color and
padding.</p>
 </div>
 <time datetime="2024-11-17">November 17, 2024</time>
 <p>
 Here is an image example:
 <img src="https://rymec.edu.in/wp-content/uploads/2023/03/baim5.png"
alt="A RYMEC image">
 </p>
 <p>
 Visit my <a href="https://rymec.edu.in">website</a> for more information.
 </p>
</body>
</html>
style.css
h2 {
 color: blue;
 font-size: 24px;
}
 h3 {
 color: green;
}
 hr {
 border: 2px solid red;
}
p {
 font-size: 18px;
}

div {
 background-color: #f0f0f0;
 padding: 10px;
}
span {
 color: red;
}
time {
 font-style: italic;
}
img {
 width: 100px;
 height: 100px;
}
a {
 text-decoration: none;
 color: purple;
}


4. Develop HTML page named as “registration.html” having variety of HTML input
elements with background colors, table for alignment & provide font colors & size
using CSS styles.
<!DOCTYPE html>
<head>
 <title>Registration Form</title>
 <style>
 body {
 font-family: Arial, sans-serif;
 background-color: #f0f4f8;
 margin: 0;
 padding: 20px;
 display: flex;
 justify-content: center;
 align-items: center;
 min-height: 100vh;
 }
 .container {
 width: 100%;
 max-width: 600px;
 background-color: #fff;
 padding: 20px;
 border-radius: 8px;
 box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
 display: flex;
 flex-direction: column;
 gap: 20px;
 }
 h2 {
 text-align: center;
 color: #333;
 margin: 0;
 }
 .form-group {
 display: flex;
 flex-direction: column;
 gap: 5px;
 margin-bottom: 10px;
 }
 label {
 font-size: 14px;
 color: #555;
 }
 input[type="text"],
 input[type="email"],
 input[type="password"],
 input[type="date"],
 select,
 textarea {
 padding: 10px;
 border: 1px solid #ccc;
 border-radius: 4px;
 font-size: 14px;
 }
 .gender-options {
 display: flex;
 gap: 10px;
 align-items: center;
 }
 input[type="submit"],
 input[type="reset"] {
 padding: 10px 20px;
 border: none;
 border-radius: 4px;
 cursor: pointer;
 font-size: 16px;
 flex: 1;
 }
 .button-group {
 display: flex;
 gap: 10px;
 justify-content: center;
 }
 input[type="submit"] {
 background-color: #4CAF50;
 color: white;
 }
 input[type="reset"] {
 background-color: #f44336;
 color: white;
 }
 .form-group textarea {
 margin-bottom: 10px;
 }
 </style>
</head>
<body>
 <div class="container">
 <h2>Registration Form</h2>
 <form action="#" method="post">
 <div class="form-group">
 <label for="firstName">First Name:</label>
 <input type="text" id="firstName" name="firstName" required>
 </div>
 <div class="form-group">
 <label for="lastName">Last Name:</label>
 <input type="text" id="lastName" name="lastName" required>
 </div>
 <div class="form-group">
 <label for="email">Email:</label>
 <input type="email" id="email" name="email" required>
 </div>
 <div class="form-group">
 <label for="password">Password:</label>
 <input type="password" id="password" name="password" required>
 </div>
 <div class="form-group">
 <label for="dob">Date of Birth:</label>
 <input type="date" id="dob" name="dob">
 </div>
 <div class="form-group">
 <label>Gender:</label>
 <div class="gender-options">
 <input type="radio" id="male" name="gender" value="male">
 <label for="male">Male</label>
 <input type="radio" id="female" name="gender" value="female">
 <label for="female">Female</label>
 </div>
 </div>
 <div class="form-group">
 <label for="country">Country:</label>
 <select id="country" name="country">
 <option value="usa">USA</option>
 <option value="canada">Canada</option>
 <option value="uk">UK</option>
 <option value="india">India</option>
 </select>
 </div>
 <div class="form-group">
 <label for="bio">Bio:</label>
 <textarea id="bio" name="bio" rows="4"></textarea>
 </div>
 <div class="button-group">
 <input type="submit" value="Register">
 <input type="reset" value="Reset">
 </div>
 </form>
 </div></body> </html>
5. Develop HTML page named as “newpaper.html” having variety of HTML
semantic elements with background colors, text-colors & size for figure, table,
aside, section, article, header, footer… etc.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>The Daily Chronicle</title>
 <style>
 body {
 font-family: 'Georgia', serif;
 line-height: 1.6;
 color: #333;
 max-width: 1200px;
 margin: 0 auto;
 padding: 20px;
 background-color: #f4f4f4;
 }
 header {
 background-color: #1a1a1a;
 color: #fff;
 padding: 20px;
 text-align: center;
 }
 header h1 {
 margin: 0;
 font-size: 2.5em;
 }
 nav {
 background-color: #333;
 color: #fff;
 padding: 10px;
 }
 nav ul {
 list-style-type: none;
 padding: 0;
 margin: 0;
 display: flex;
 justify-content: center;
 }
 nav ul li {
 margin: 0 10px;
 }
 nav ul li a {
 color: #fff;
 text-decoration: none;
 }
 main {
 display: flex;
 margin-top: 20px;
 }
 section {
 flex: 2;
 margin-right: 20px;
 }
 article {
 background-color: #fff;
 padding: 20px;
 margin-bottom: 20px;
 box-shadow: 0 0 10px rgba(0,0,0,0.1);
 }
 article h2 {
 color: #1a1a1a;
 font-size: 1.8em;
 }
 aside {
 flex: 1;
 background-color: #e6e6e6;
 padding: 20px;
 box-shadow: 0 0 10px rgba(0,0,0,0.1);
 }
 figure {
 margin: 0;
 text-align: center;
 }
 figure img {
 max-width: 100%;
 height: auto;
 }
 figcaption {
 font-style: italic;
 color: #666;
 font-size: 0.9em;
 }
 table {
 width: 100%;
 border-collapse: collapse;
 margin-bottom: 20px;
 }
 th, td {
 border: 1px solid #ddd;
 padding: 10px;
 text-align: left;
 }
 th {
 background-color: #f2f2f2;
 }
 footer {
 background-color: #1a1a1a;
 color: #fff;
 text-align: center;
 padding: 10px;
 margin-top: 20px;
 }
 </style>
</head>
<body>
 <header>
 <h1>The Daily Chronicle</h1>
 </header>

 <nav>
 <ul>
 <li><a href="#">Home</a></li>
 <li><a href="#">Politics</a></li>
 <li><a href="#">Technology</a></li>
 <li><a href="#">Sports</a></li>
 <li><a href="#">Entertainment</a></li>
 </ul>
 </nav>
 <main>
 <section>
 <article>
 <h2>Breaking News: Major Technological Breakthrough</h2>
 <p>Scientists have announced a groundbreaking discovery in the field of
quantum computing, potentially revolutionizing the tech industry.</p>
 <figure>
<img src="https://rymec.edu.in/wp-content/uploads/2023/03/baim5.png"
alt="RYMEC image">
<figcaption>RYMEC</figcaption>
 </figure>
 </article>

 <article>
 <h2>Local Sports Team Wins Championship</h2>
 <p>In a thrilling match, our local team secured victory in the national
championship, bringing pride to our
city.</p>
 <table>
 <tr>
 <th>Team</th>
 <th>Score</th>
 </tr>
 <tr>
 <td>Local Heroes</td>
 <td>3</td>
 </tr>
 <tr>
 <td>Visiting Challengers</td>
 <td>2</td>
 </tr>
 </table>
 </article>
 </section>

 <aside>
 <h3>Weather Update</h3>
 <p>Expect sunny skies with a high of 75°F (24°C) today.</p>

 <h3>Upcoming Events</h3>
 <ul>
 <li>City Festival - This Weekend</li>
 <li>Tech Conference - Next Month</li>
 <li>Charity Run - In Two Weeks</li>
 </ul>
 </aside>
 </main>
 <footer>
 <p>&copy; 2024 The Daily Chronicle. All rights reserved.</p>
 </footer>
</body>
</html>
6. Apply HTML, CSS and JavaScript to design a simple calculator to perform the
following operations: sum, product, difference, remainder, quotient, power,
square-root and square.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Simple Calculator</title>
 <style>
 body {
 font-family: Arial, sans-serif;
 display: flex;
 justify-content: center;
 align-items: center;
 height: 100vh;
 margin: 0;
 background-color: #f0f0f0;
 }
 .calculator {
 background-color: #fff;
 border-radius: 8px;
 box-shadow: 0 0 10px rgba(0,0,0,0.1);
 padding: 20px;
 width: 300px;
 }
 #display {
 width: 100%;
 height: 40px;
 font-size: 1.5em;
 text-align: right;
 margin-bottom: 10px;
 padding: 5px;
 box-sizing: border-box;
 }
 .buttons {
 display: grid;
 grid-template-columns: repeat(4, 1fr);
 gap: 10px;
 }
 button {
 padding: 10px;
 font-size: 1.2em;
 border: none;
 background-color: #e0e0e0;
 cursor: pointer;
 border-radius: 4px;
 }
 button:hover {
 background-color: #d0d0d0;
 }
 .operator {
 background-color: #f0a030;
 color: white;
 }
 .operator:hover {
 background-color: #e09020;
 }
 </style>
</head>
<body>
 <div class="calculator">
 <input type="text" id="display" readonly>
 <div class="buttons">
 <button onclick="appendToDisplay('7')">7</button>
 <button onclick="appendToDisplay('8')">8</button>
 <button onclick="appendToDisplay('9')">9</button>
 <button class="operator" onclick="setOperation('+')">&plus;</button>
 <button onclick="appendToDisplay('4')">4</button>
 <button onclick="appendToDisplay('5')">5</button>
 <button onclick="appendToDisplay('6')">6</button>
 <button class="operator" onclick="setOperation('-')">&minus;</button>
 <button onclick="appendToDisplay('1')">1</button>
 <button onclick="appendToDisplay('2')">2</button>
 <button onclick="appendToDisplay('3')">3</button>
 <button class="operator" onclick="setOperation('*')">&times;</button>
 <button onclick="appendToDisplay('0')">0</button>
 <button onclick="appendToDisplay('.')">.</button>
 <button class="operator" onclick="calculate()">&equals;</button>
 <button class="operator" onclick="setOperation('/')">&divide;</button>
 <button class="operator" onclick="setOperation('%')">%</button>
 <button class="operator" onclick="setOperation('^')">x<sup>y</sup></button>
 <button class="operator" onclick="squareRoot()">√</button>
 <button class="operator" onclick="square()">x<sup>2</sup></button>
 <button onclick="clearDisplay()">C</button>
 </div>
 </div>
 <script>
 let display = document.getElementById('display');
 let currentValue = '';
 let operation = '';
 let previousValue = '';
 function appendToDisplay(value) {
 currentValue += value;
 display.value = currentValue;
 }
 function clearDisplay() {
 currentValue = '';
 operation = '';
 previousValue = '';
 display.value = '';
 }
 function setOperation(op) {
 if (currentValue !== '') {
 if (previousValue !== '') {
 calculate();
 }
 operation = op;
 previousValue = currentValue;
 currentValue = '';
 }
 }
 function calculate() {
 if (previousValue !== '' && currentValue !== '') {
 let result;
 const prev = parseFloat(previousValue);
 const current = parseFloat(currentValue);
 switch(operation) {
 case '+':
 result = prev + current;
 break;
 case '-':
 result = prev - current;
 break;
 case '*':
 result = prev * current;
 break;
 case '/':
 result = prev / current;
 break;
 case '%':
 result = prev % current;
 break;
 case '^':
 result = Math.pow(prev, current);
 break;
 }
 display.value = result;
 previousValue = result.toString();
 currentValue = '';
 operation = '';
 }
 }
 function squareRoot() {
 if (currentValue !== '') {
 const result = Math.sqrt(parseFloat(currentValue));
 display.value = result;
 currentValue = result.toString();
 }
 }
 function square() {
 if (currentValue !== '') {
 const result = Math.pow(parseFloat(currentValue), 2);
 display.value = result;
 currentValue = result.toString();
 }
 }
 </script>
</body>
</html>
7. Develop JavaScript program (with HTML/CSS) for:
a) Converting JSON text to JavaScript Object.
b) Convert JSON results into a date.
c) Converting From JSON To CSV and CSV to JSON.
d) Create hash from string using crypto.createHash() method.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>JSON/CSV Converter and Hash Generator</title>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/cryptojs.min.js"></script>
 <style>
 body {
 font-family: Arial, sans-serif;
 line-height: 1.6;
 margin: 0;
 padding: 20px;
 background-color: #f4f4f4;
 }
 .container {
 max-width: 800px;
 margin: auto;
 background: white;
 padding: 20px;
 border-radius: 5px;
 box-shadow: 0 0 10px rgba(0,0,0,0.1);
 }
 h1 {
 color: #333;
 }
 textarea {
 width: 100%;
 height: 100px;
 margin-bottom: 10px;
 }
 button {
 background-color: #4CAF50;
 color: white;
 padding: 10px 15px;
 border: none;
 border-radius: 4px;
 cursor: pointer;
 margin-right: 10px;
 }
 button:hover {
 background-color: #45a049;
 }
 #result {
 margin-top: 20px;
 padding: 10px;
 background-color: #e7e7e7;
 border-radius: 4px;
 }
 </style>
</head>
<body>
 <div class="container">
 <h1>JSON/CSV Converter and Hash Generator</h1>

 <h2>a) Convert JSON to JavaScript Object</h2>
 <textarea id="jsonInput" placeholder="Enter JSON here"></textarea>
 <button onclick="convertJsonToObject()">Convert to Object</button>

 <h2>b) Convert JSON to Date</h2>
 <textarea id="jsonDateInput" placeholder='Enter JSON date string (e.g., {"date":
"2023-05-15T12:00:00Z"})'></textarea>
 <button onclick="convertJsonToDate()">Convert to Date</button>

 <h2>c) Convert JSON to CSV and CSV to JSON</h2>
 <textarea id="dataInput" placeholder="Enter JSON or CSV here"></textarea>
 <button onclick="convertJsonToCsv()">JSON to CSV</button>
 <button onclick="convertCsvToJson()">CSV to JSON</button>

 <h2>d) Create Hash from String</h2>
 <textarea id="hashInput" placeholder="Enter string to hash"></textarea>
 <button onclick="createHash()">Generate Hash</button>

 <div id="result"></div>
 </div>
 <script>
 function convertJsonToObject() {
 try {
 const jsonInput = document.getElementById('jsonInput').value;
 const jsObject = JSON.parse(jsonInput);
 document.getElementById('result').innerText = 'Converted Object: ' +
JSON.stringify(jsObject, null, 2);
 } catch (error) {
 document.getElementById('result').innerText = 'Error: ' + error.message;
 }
 }
 function convertJsonToDate() {
 try {
 const jsonInput = document.getElementById('jsonDateInput').value;
 const jsObject = JSON.parse(jsonInput);
 const date = new Date(jsObject.date);
 document.getElementById('result').innerText = 'Converted Date: ' +
date.toString();
 } catch (error) {
 document.getElementById('result').innerText = 'Error: ' + error.message;
 }
 }
 function convertJsonToCsv() {
 try {
 const jsonInput = document.getElementById('dataInput').value;
 const jsObject = JSON.parse(jsonInput);
 const headers = Object.keys(jsObject[0]);
 const csvRows = [
 headers.join(','),
 ...jsObject.map(row => headers.map(fieldName =>
JSON.stringify(row[fieldName])).join(','))
 ];
 const csvString = csvRows.join('\n');
 document.getElementById('result').innerText = 'Converted CSV:\n' + csvString;
 } catch (error) {
 document.getElementById('result').innerText = 'Error: ' + error.message;
 }
 }
 function convertCsvToJson() {
 try {
 const csvInput = document.getElementById('dataInput').value;
 const lines = csvInput.split('\n');
 const headers = lines[0].split(',');
 const jsonArray = lines.slice(1).map(line => {
 const values = line.split(',');
 return headers.reduce((obj, header, index) => {
 obj[header] = values[index];
 return obj;
 }, {});
 });
 document.getElementById('result').innerText = 'Converted JSON:\n' +
JSON.stringify(jsonArray, null, 2);
 } catch (error) {
 document.getElementById('result').innerText = 'Error: ' + error.message;
 }
 }
 function createHash() {
 try {
 const input = document.getElementById('hashInput').value;
 const hash = CryptoJS.SHA256(input);
 document.getElementById('result').innerText = 'Generated Hash (SHA-256): ' +
hash;
 } catch (error) {
 document.getElementById('result').innerText = 'Error: ' + error.message;
 }
 }
 </script>
</body>
</html>
8a. Develop a PHP program (with HTML/CSS) to keep track of the number of
visitors visiting the web page and to display this count of visitors, with relevant
headings.
<!DOCTYPE html>
<html> <head> <title> Visitors Count </title></head>
<body bgcolor = "#99CC99">
<div style="position:absolute; top: 200px; left: 100px;
 font-size:25pt; font-family: 'Trebuchet MS';">
<?php
 if($handle=@fopen("counter.txt","r"))
 {
 $counter=fscanf($handle,"%d");
 fclose($handle);
 $counter[0]++;
 echo" This is the program to keep track the number of visits for this webpage";
 echo" <br /><br /> This Page is visited ". $counter[0] . " Times" ;
 $handle= fopen("counter.txt", "w" ) ;
 fprintf($handle,"%d",$counter[0]) ;
 fclose ($handle) ;
 }
 elseif($handle = fopen("counter.txt", "w"))
 {
 echo "Welcome to this Website <br /> This is your Firsrt Visit";
 fprintf($handle,"%d",1);
 fclose($handle);
 }
?>
</div>
<h1> Welcome to CSE </h1>
</body>
</html>
8b. Develop a PHP program (with HTML/CSS) to sort the student records which
are stored in the database using selection sort.
<!DOCTYPE html>
<html> <head> <title> Pattern Matching </title>
<style>
 table, td, th
 {
 border: 1px solid red;
 text-align: center;
 background-color:lightyellow;
 border-collapse:collapse;
 width: 30%;
 padding: 8px;
 }
 div
 {
 float: left;
 padding: 10px;
 margin-left: 1%;
 margin-top: 5%;
 border-left-style: outset;
 border-color: crimson;
 font-size:20pt;
 font-family: 'Trebuchet MS';
 }
</style>
</head>
<body bgcolor = "#CC99CC">
<center><h1> Applying Selection sort on Student Data in Data Base </h1> </center><hr />
<?php
$con=mysqli_connect("localhost:3306","root","","Bhagath") or die(mysql_error());
echo "<div>Student Details after Applying </br>Selection Sort is as follows </br>";
echo "<table><tr><th>USN</th><th>NAME</th><th>SEM</th></tr>";
$sel="select *from student";
$qh=mysqli_query($con,$sel);
$rowcount=mysqli_num_rows($qh);
if($rowcount>0)
{
 $fetchedarray=mysqli_fetch_all($qh,MYSQLI_ASSOC);
 for($i = 0; $i < $rowcount-1; $i++)
 {
 $minimum = $i;
 for($j = $i+1; $j < $rowcount; $j++)
 {
 if(strcmp($fetchedarray[$j]['usn'],$fetchedarray[$minimum]['usn'])<=0)
 {
 $minimum = $j;
 }
 }
 $temp=$fetchedarray[$minimum];
 $fetchedarray[$minimum]=$fetchedarray[$i];
 $fetchedarray[$i]=$temp;
 }
 $i=0;
 while($i<$rowcount)
 {
 echo "<tr><td>",$fetchedarray[$i]['usn'],"</td><td>",$fetchedarray[$i]['name'],
 "</td><td>",$fetchedarray[$i]['sem'],"</tr>";
 $i++;
 }
}
else
 echo "<tr><td colspan=3> No Records Found </td></tr>";
mysqli_free_result($qh);
echo "</table>";
echo "Total No of Student Records in DB : $rowcount </div>";
?>
<div> Enter New Student Record Here </ br>
<form method="post">
<table>
<tr><th>USN</th><th>NAME</th><th>SEM</th></tr>
<tr>
<td><input type="text" name="tusn" /></td>
<td><input type="text" name="tname" /></td>
<td><input type="text" name="tsem" /></td>
</tr>
<tr>
 <td><input type="submit" name="submit" value="Save"></td>
 <td><input type="reset" value="Clear"></td>
</tr>
</table>
</form>
<?php
if(isset($_POST['submit'])) // it checks submit is clicked
{
 $usn = $_POST['tusn'];
 $name = $_POST['tname'];
 $sem = $_POST['tsem'];
 if($usn=="" or $name=="" or $sem=="")
 echo "Enter Valid Input ";
 else
 {
 $insert="insert into student values('$usn','$name','$sem')";
 $qh=mysqli_query($con,$insert) or die(mysql_error());
 if($qh)
 {
 $secondswait=2;
 echo "Student details Saved Successfully";
 echo '<meta http-equiv="refresh" content="'.$secondswait.'">';
 }
 }
}
echo "</div>";
?>
9. Develop jQuery script (with HTML/CSS) for:
a. Appends the content at the end of the existing paragraph and list.
b. Change the state of the element with CSS style using animate() method.
c. Change the color of any div that is animated.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>jQuery Append, Animate, and Color Change Demo</title>
 <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
 <style>
 body {
 font-family: Arial, sans-serif;
 line-height: 1.6;
 margin: 0;
 padding: 20px;
 background-color: #f4f4f4;
 }
 .container {
 max-width: 800px;
 margin: auto;
 background: white;
 padding: 20px;
 border-radius: 5px;
 box-shadow: 0 0 10px rgba(0,0,0,0.1);
 }
 h1, h2 {
 color: #333;
 }
 .box {
 width: 100px;
 height: 100px;
 background-color: #3498db;
 margin: 20px 0;
 }
 button {
 padding: 10px 15px;
 background-color: #2ecc71;
 color: white;
 border: none;
 border-radius: 5px;
 cursor: pointer;
 margin-right: 10px;
 }
 button:hover {
 background-color: #27ae60;
 }
 </style>
</head>
<body>
 <div class="container">
 <h1>jQuery Demonstration</h1>
 <h2>a. Append Content</h2>
 <p id="existingParagraph">This is an existing paragraph. </p>
 <ul id="existingList">
 <li>Existing item 1</li>
 <li>Existing item 2</li>
 </ul>
 <button id="appendButton">Append Content</button>
 <h2>b. Animate Element</h2>
 <div id="animateBox" class="box"></div>
 <button id="animateButton">Animate Box</button>
 <h2>c. Change Color of Animated Div</h2>
 <div id="colorBox" class="box"></div>
 <button id="colorAnimateButton">Animate and Change Color</button>
 </div>
 <script>
 $(document).ready(function() {
 // a. Append content
 $("#appendButton").click(function() {
 $("#existingParagraph").append("This content is appended.");
 $("#existingList").append("<li>Appended item</li>");
 });
 // b. Animate element
 $("#animateButton").click(function() {
 $("#animateBox").animate({
 width: "200px",
 height: "200px",
 opacity: 0.5
 }, 1000);
 });
 // c. Animate and change color
 $("#colorAnimateButton").click(function() {
 $("#colorBox").animate({
 width: "200px",
 height: "200px"
 }, {
 duration: 1000,
 step: function(now, fx) {
 if (fx.prop === "width") {
 $(this).css("background-color", `rgb(${Math.round(now)}, 52, 219)`);
 }
 }
 });
 });
 });
 </script>
</body>
</html>
10. Develop a JavaScript program with Ajax (with HTML/CSS) for:
a. Use ajax() method (without Jquery) to add the text content from the text file by
sending ajax request.
b. Use ajax() method (with Jquery) to add the text content from the text file by
sending ajax request.
c. Illustrate the use of getJSON() method in jQuery.
d. Illustrate the use of parseJSON() method to display JSON values.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Ajax Demo Program</title>
 <script
src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
 <style>
 body {
 font-family: Arial, sans-serif;
 line-height: 1.6;
 margin: 0;
 padding: 20px;
 background-color: #f4f4f4;
 }
 .container {
 max-width: 800px;
 margin: auto;
 background: white;
 padding: 20px;
 border-radius: 5px;
 box-shadow: 0 0 10px rgba(0,0,0,0.1);
 }
 h1 {
 color: #333;
 }
 h2 {
 color: #666;
 }
 button {
 background-color: #4CAF50;
 border: none;
 color: white;
 padding: 10px 20px;
 text-align: center;
 text-decoration: none;
 display: inline-block;
 font-size: 16px;
 margin: 4px 2px;
 cursor: pointer;
 border-radius: 4px;
 }
 pre {
 background-color: #f8f8f8;
 border: 1px solid #ddd;
 border-radius: 4px;
 padding: 10px;
 white-space: pre-wrap;
 word-wrap: break-word;
 }
 </style>
</head>
<body>
 <div class="container">
 <h1>Ajax Demo Program</h1>
 <h2>a. Ajax-like operation without jQuery</h2>
 <button onclick="operationWithoutJQuery()">Perform Operation (without
jQuery)</button>
 <pre id="result-a"></pre>
 <h2>b. Ajax-like operation with jQuery</h2>
 <button onclick="operationWithJQuery()">Perform Operation (with
jQuery)</button>
 <pre id="result-b"></pre>
 <h2>c. jQuery-like getJSON() method</h2>
 <button onclick="getJSONOperation()">Get JSON</button>
 <pre id="result-c"></pre>
 <h2>d. jQuery parseJSON() method</h2>
 <button onclick="parseJSONExample()">Parse JSON</button>
 <pre id="result-d"></pre>
 </div>
 <script>
 // Simulated data
 const simulatedData = {
 text: "This is a sample text from a simulated server response.",
 json: {
 name: "John Doe",
 age: 30,
 city: "New York"
 }
 };
 // a. Ajax-like operation without jQuery
 function operationWithoutJQuery() {
 setTimeout(function() {
 document.getElementById("result-a").textContent = simulatedData.text;
 }, 500);
 }
 // b. Ajax-like operation with jQuery
 function operationWithJQuery() {
 $.Deferred(function(deferred) {
 setTimeout(function() {
 deferred.resolve(simulatedData.text);
 }, 500);
 }).done(function(result) {
 $("#result-b").text(result);
 });
 }
 // c. jQuery-like getJSON() method
 function getJSONOperation() {
 $.Deferred(function(deferred) {
 setTimeout(function() {
 deferred.resolve(simulatedData.json);
 }, 500);
 }).done(function(result) {
 $("#result-c").text(JSON.stringify(result, null, 2));
 });
 }
 // d. jQuery parseJSON() method
 function parseJSONExample() {
 var jsonString = JSON.stringify(simulatedData.json);
 var jsonObject = $.parseJSON(jsonString);
 $("#result-d").text(JSON.stringify(jsonObject, null, 2));
 }
 </script>
</body>
</html>
