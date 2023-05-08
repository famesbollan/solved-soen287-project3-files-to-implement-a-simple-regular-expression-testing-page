Download Link: https://assignmentchef.com/product/solved-soen287-project3-files-to-implement-a-simple-regular-expression-testing-page
<br>
<h1></h1>

Create 2 files, named <strong><em>a3q1.html</em></strong> and <strong><em>a3q1.js</em></strong>, to implement a simple regular expression testing page, like the one shown below. Try to match the layout in the screenshot. There is no need to put any CSS code to achieve this layout. The text area should have 10 rows and 80 columns, and the first 2 input text should have a size of 20 and the last one a size of 5. The title should be an <em>h1</em>.




All the JavaScript code should be put in the js file, except for connecting the search button with a search function located in the js file, which has to be included in the head element of the html file.

Your search function should:

<ol>

 <li>start by splitting the text from the text area according to the split characters given in the first input text box. If the first input text box is empty, then don’t split the text</li>

 <li>create a regular expression by providing the <em>RegExp</em> constructor function the text of the second and third input boxes (use <strong><em>new RegExp()</em></strong>, not <strong><em>/…/…</em></strong>)</li>

 <li>test the regular expression on each non‐empty word (or element) of the array obtained from step 1, or on the text directly if no splitting characters were given</li>

 <li>Output the number of non‐empty words in the text, plus the number of words matching the regular expression.</li>

</ol>




<h1>Question #2</h1>

Create 2 files, named <strong><em>a3q2.html</em></strong> and <strong><em>a3q2.js</em></strong>, to implement a page validating variable names, and adding them into a list, like in the 3 screenshots included below. Try to match the layout in the screenshots. The only CSS needed is to change the text and background colors of the input text box when the value input is not a valid variable name. What constitutes a valid variable name is given in the screenshots.




You should write at least 2 functions, in your js file, one to validate a variable name (function name: <em>validateVariable</em>), and another to add a variable (function name: <em>addVariable</em>). The validate function should be called on the <em>keyup</em> event of the input text. If the value in the input text is not a valid variable name, then it should change the text color to red and the background color to yellow. The easiest way to do this is to define a CSS class in the html file and set the <em>className</em> of the element to this error class. If the value is a valid variable name, then remove the class from the input text element (by setting the <em>className</em> to an empty string).




The add button should call the add variable function on the onclick event. It should first check if the variable name is valid, then check if the variable name has already been added to the list. If not, then it should add the variable to the list. If the variable name is already in the list, then it should not do anything. You can keep a global array containing all the variable names added, to make it easier to check, in the add variable function, which variable names have been added so far. After checking if the variable name has already been added or not, you can easily push a new variable name to the global array before or after adding the variable name to the ul.







<h2>Question #3</h2>

You have a server‐side script that cannot handle any ampersand (&amp;) and pipe character (|) in the form data. So we need to convert all the ampersand characters to “and” and pipe characters to “or” at the client side. Write a script to do these conversions in the form field when the field loses <strong>focus</strong> element (<strong>blu</strong>r).

<ol>

 <li>Your script (<strong>js</strong>) contains one (01) variable and two (02) functions:

  <ol>

   <li>Global variable: dom.</li>

   <li>The function <strong>getElementAmpersandPipe()</strong> first reads the field element by using the existing function <em><u>getElementById()</u></em> to access the element using its id (″field″) specified in your HTML file. Then it uses the <u>addEventListener</u>() function to register the event handler. <u>addEventListener</u>() takes (03) arguments : (a) the name of event as a string literal (here use “<strong>blur</strong>“), (b) the handler function convertAmpersandPipe, and (c) the Boolean value false.</li>

   <li>The function “<strong>convertAmpersandPipe()</strong>” that converts all the ampersands in the form field to ” and ” and all the pipe characters to “or”, when the field loses focus (“<strong>blur</strong>“).</li>

   <li>The html document called “AmpersandPipe<em>.html</em>“, which includes the “AmpersandPipe.js” in the head section.</li>

  </ol></li>

 <li>At the end of the JavaScript file, finish with this line to fire the load event when a resource and its dependent resources have finished loading: window.addEventListener( “load”, getElementAmpersandPipe, false );</li>

</ol>

<u>Here is a sample input and output to illustrate the expected behavior of your program:</u>

<h1>Question #4</h1>

Copy and paste the following HTML code into a new document:




&lt;!DOCTYPE html&gt;

&lt;html&gt;

&lt;head&gt;

&lt;title&gt;Q4&lt;/title&gt;

&lt;/head&gt;

&lt;body&gt;

&lt;div id=”container”&gt;

&lt;h2&gt;Create Your Own flower Bouqute&lt;/h2&gt;

&lt;form action=””  id=”frm”&gt;

&lt;fieldset&gt;

&lt;table border=”0″&gt;

&lt;tr&gt;

&lt;th&gt;Item&lt;/th&gt;

&lt;th&gt;Unit&lt;/th&gt;

&lt;th&gt;Price&lt;/th&gt;

&lt;/tr&gt;

&lt;tr&gt;

&lt;td&gt;Red Roses&lt;/td&gt;

&lt;td&gt;&lt;input type=”text” size=”3″ id=”rose” /&gt;&lt;/td&gt;

&lt;td&gt;$5.5&lt;/td&gt;

&lt;/tr&gt;

&lt;tr&gt;

&lt;td&gt;Yellow Lily&lt;/td&gt;

&lt;td&gt;&lt;input type=”text” size=”3″ id=”lily” /&gt;&lt;/td&gt;

&lt;td&gt;$7.5&lt;/td&gt;

&lt;/tr&gt;

&lt;tr&gt;

&lt;td&gt;White Mini Calla&lt;/td&gt;

&lt;td&gt;&lt;input type=”text” size=”3″ id=”scalla” /&gt;&lt;/td&gt;

&lt;td&gt;$4.00&lt;/td&gt;

&lt;/tr&gt;

&lt;tr&gt;

&lt;td&gt;Pink Orchid&lt;/td&gt;

&lt;td&gt;&lt;input type=”text” size=”3″ id=”orchid” /&gt;&lt;/td&gt;

&lt;td&gt;$8.00&lt;/td&gt;

&lt;/tr&gt;

&lt;/tr&gt;

&lt;tr&gt;

&lt;td&gt;Orange Daisy&lt;/td&gt;

&lt;td&gt;&lt;input type=”text” size=”3″ id=”daisy” /&gt;&lt;/td&gt;

&lt;td&gt;$7.00&lt;/td&gt;

&lt;/tr&gt;

&lt;/table&gt;

&lt;br /&gt;&lt;br /&gt;

&lt;label&gt; Choose your delivery method &lt;/label&gt; &lt;br/&gt;&lt;br/&gt;

&lt;input type =”radio” name=”delivery”/&gt; Standard ($2)

&lt;input type =”radio” name=”delivery”/&gt; Premium ($6)

&lt;br/&gt;&lt;br/&gt;

&lt;input type=”button” value=”Place Order” id=”sub” onclick=”calculateTotal();”/&gt;

&lt;/fieldset&gt;

&lt;/form&gt;

&lt;/div&gt;

&lt;script type=”text/javascript” src=”Q4.js”&gt;&lt;/script&gt;

&lt;/body&gt;

&lt;/html&gt;

<ol start="4">

 <li>Write JavaScript code (Q4.js) that is executed when the place order button is pressed and it calculates the cost of each item (based on quantity specified) entered the online form and the overall total cost. The results should be displayed on the same page under the form submission button.</li>

</ol>

All JavaScript code must be external. If any fields are left blank or do not contain a number, an alert box should display an appropriate error message upon form submission.

<ol>

 <li>The following style rules must be implemented using an external CSS. Ensure that the stylesheet is properly referenced in the HTML code

  <ul>

   <li>All text in the page must be displayed in <em>MediumBlue</em>.</li>

   <li>The background color of the form is <em>DarkOrange</em>.</li>

   <li>The input form should have a fixed width of 540 pixels.</li>

   <li>The input form should be surrounded by a <em>blue </em>border and the distance from the content to the border should be 10 pixels.</li>

  </ul></li>

</ol>

The resulted page looks like as the following.













<h2>Question #5</h2>

The running problem to build a website for the Hotel Room Reservation (To be continued in

Assignment 4). We resume the Hotel Reservation Web site in Assignment 1.

Please create another section called “Expert suggestion” after the section of “What you are looking for”. Style it properly and make it invisible at first. Once the user’s selections meet the following criteria, use JavaScript to insert the suggested text into this section and make it visible.

 If the Number of price range is $50 to $100 and the selected location is Downtown, show the expert suggestion: “It is very difficult to find a hotel room in this price range at

Downtown




<ol>

 <li>a) Initial form b) after filling the form and hitting the search button</li>

</ol>






















<h1></h1>