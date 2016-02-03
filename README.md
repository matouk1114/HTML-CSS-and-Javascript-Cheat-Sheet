# HTML-CSS-and-Javascript-Cheat-Sheet
Cheet sheet for anyone to use-update as you'd like!
HTML
Basic Tags
<html></html> Creates an HTML document
<head></head> Sets off the title and other information that isn’t displayed on the web page itself
<body></body> Sets off the visible portion of the document
Body Attributes
<body bgcolor="green"> Sets the background color, using name or hex value
<body text="black"> Sets the text color, using name or hex value
<body link="blue"> Sets the color of links, using name or hex value
<body vlink="#ff0000"> Sets the color of followed links, using name or hex value
<body alink="#00ff00"> Sets the color of links on click
<body ondragstart="return false" onselectstart="return false"> Disallows text selection with the mouse and keyboard
Text Tags
<pre></pre> Creates preformatted text
<hl></hl> Creates the largest headline
<h6></h6> Creates the smallest headline
<b></b> Creates bold text
<i></i> Creates italic text
<tt></tt> Creates teletype, or typewriter-style text
<cite></cite> Creates a citation, usually italic
<em></em> Emphasizes a word (with italic or bold)
<strong></strong> Emphasizes a word (with italic or bold)
<font size="3"></font> Sets size of font, from 1 to 7
<font color="green"></font> Sets font color, using name or hex value
Links
<a href="URL"></a> Creates a hyperlink
<a href="mailto:EMAIL"></a> Creates a mailto link
<a href="URL"><img src="URL"> </a> Creates an image/link
<a name="NAME"></a> Creates a target location within a document
<a href="#NAME"></a> Links to that target location from elsewhere in the document
Formatting
<p></p> Creates a new paragraph
<p align="left"> Aligns a paragraph to the left (default), right, or center.
<br> Inserts a line break
<blockquote></blockquote> Indents text from both sides
<dl></dl> Creates a definition list
<dt> Precedes each definition term
<dd> Precedes each definition
<ol></ol> Creates a numbered list
<ul></ul> Creates a bulleted list
<li></li> Precedes each list item, and adds a number or symbol depending upon the type of list selected
<div align="left"> A generic tag used to format large blocks of HTML, also used for stylesheets
<img src="name"> Adds an image
<img src="name" align="left"> Aligns an image: left, right, center; bottom, top, middle
<img src="name" border="1"> Sets size of border around an image
<hr /> Inserts a horizontal rule
<hr size="3" /> Sets size (height) of rule
<hr width="80%" /> Sets width of rule, in percentage or absolute value
<hr noshade /> Creates a rule without a shadow
Tables
<table></table> Creates a table
<tr></tr> Sets off each row in a table
<td></td> Sets off each cell in a row
<th></th> Sets off the table header (a normal cell with bold, centered text)
Table Attributes
<table border="1"> Sets width of border around table cells
<table cellspacing="1"> Sets amount of space between table cells
<table cellpadding="1"> Sets amount of space between a cell’s border and its contents
<table width="500" or "80%"> Sets width of table, in pixels or as a percentage of document width
<tr align="left"> or <td align="left"> Sets alignment for cell(s) (left, center, or right)
<tr valign="top"> or <td valign="top"> Sets vertical alignment for cell(s) (top, middle, or bottom)
<td colspan="2"> Sets number of columns a cell should span (default=1)
<td rowspan="4"> Sets number of rows a cell should span (default=1)
<td nowrap> Prevents the lines within a cell from being broken to fit
Frames
<frameset></frameset> Replaces the <body> tag in a frames document; can also be nested in other framesets
<frameset rows="value,value"> Defines the rows within a frameset, using number in pixels, or percentage of width
<frameset cols="value,value"> Defines the columns within a frameset, using number in pixels, or percentage of width
<frame> Defines a single frame — or region — within a frameset
<noframes></noframes> Defines what will appear on browsers that don’t support frames
Frames Attributes
<frame src="URL"> Specifies which HTML document should be displayed
<frame name="name"> Names the frame, or region, so it may be targeted by other frames
<frame marginwidth="value"> Defines the left and right margins for the frame; must be equal to or greater than 1
<frame marginheight="value"> Defines the top and bottom margins for the frame; must be equal to or greater than 1
<frame scrolling="value"> Sets whether the frame has a scrollbar; value may equal “yes,” “no,” or “auto.” The default, as in ordinary documents, is auto.
<frame noresize="noresize"> Prevents the user from resizing a frame
Forms
For functional forms, you’ll have to run a script. The HTML just creates the appearance of a form.
<form></form> Creates all forms
<select multiple name="NAME" size=?></select> Creates a scrolling menu. Size sets the number of menu items visible before you need to scroll.
<option> Sets off each menu item
<select name="NAME"></select> Creates a pulldown menu
<option> Sets off each menu item
<textarea name="NAME" cols=40 rows=8></textarea name> Creates a text box area. Columns set the width; rows set the height.
<input type="checkbox" name="NAME"> Creates a checkbox. Text follows tag.
<input type="radio" name="NAME" value="x"> Creates a radio button. Text follows tag
<input type="text" name="NAME" size=20> Creates a one-line text area. Size sets length, in characters.
<input type="submit" value="NAME"> Creates a Submit button
<button type="submit">Submit</button> Creates an actual button that is clicked
<input type="image" border=0 name="NAME" src="name.gif"> Creates a Submit button using an image
<input type="reset"> Creates a Reset button
CSS
External File
<head>
<link rel="stylesheet" type="text/css" href="style.css" title="style">
</head>
Within HTML Header
<head>
<style type="text/css">
 h1 {
    color:red;
    }
</style>
</head>
Inline in HTML File
<p style="color:red;">Some red text</p>
Selectors

Universal Selector* {}
Type Selectorh1, h2 ,h3 {}
Child Selectorul > li {}
Descendant Selectorp a {}
Class Selector.class {}
ID Selector#id {}
Adjacent Sibling Selectorh1 + p {}
General Sibling Selectorh1 ~ p {}
Attribute Selector[attribute="SomeValue"] {}

Pseudo Selectors

Mouse Over Selectora:hover {}
Active Link Selectora:active {}
Focus Selectorinput:focus {}
Visited Links Selectora:visited {}
Link Selector.class:link {}
Checked elements selectorinput:checked {}
Disabled elements selectorinput:disabled {}
Enabled elements selectorinput:enabled {}
Not a Specified Element Selector:not(p) {}
First Line Selectorp::first-line {}
First Letter Selectorp::first-letter {}
First Child Selectorp:first-child {}
Last Child Selectorp:last-child {}
:nth-child Selectorp:nth-child() {}
First Element of its Parent Selectorp:first-of-type {}
Elements that have no Children Selector (including text nodes)p:empty {}
 
Font Styling

Font stylefont-style: normal | italic | oblique
Font Variantfont-variant: normal | small-caps
Font Weightfont-weight: normal | bold | bolder | lighter | 100 - 900
Vertical Alignmentvertical-align: baseline | 10px | sub | super | top | text-top | middle | bottom | text-bottom | initial
Font Sizefont-size: 12px | 0.8em | 80%
Text Transformtext-transform: capitalise | lowercase | uppercase
Space Between Charactersletter-spacing: normal | 4px
Line Heightline-height: normal | 3em | 34%
Horizontal Alignmenttext-align: left | right | center | justify
Text Decorationtext-decoration: none | underline | overline | line-through
Indent First Linetext-indent: 25px
Font Familyfont-family: 'Open Sans', sans-serif

 Position

Positionposition: static | relative | absolute | fixed | sticky
Left Positionleft: 10px | 10% | auto
Top Positiontop: 10px | 10% | auto
Float Elementfloat: left | right | none
Clear Floating Elementsclear: none | left | right | both
Z Indexz-index: 3 | auto | inherit

Background

Background Imagebackground-image: url()
Background Repeatbackground-repeat: repeat-x | repeat-y | repeat | space | round | no-repeat
Background Attachmentbackground-attachment: scroll | fixed | local | initial | inherit
Background Colorbackground-color: #2AA9E0
Background Positionbackground-position: top | right | bottom | left | center

Box properties

Marginmargin-top: 2pxmargin-right: 4px | automargin-bottom: 6pxmargin-left: 8px | automargin: 2px 4px 6px 8px | 0 auto
Paddingpadding-top: 2pxpadding-right: 4px | autopadding-bottom: 6pxpadding-left: 8px | autopadding: 2px 4px 6px 8px | 0 auto
Border Colorborder-color: #2AA9E0
Border Styleborder-style: none	| hidden | dotted | dashed | solid | double | groove | ridge | inset | outset
Border Widthborder-width: 10px

List Styling

List Typelist-style-type: disc | circle | square | none
List Positionlist-style-position: inside | outside
List Imagelist-style-image: url();
Javascript

Trivial expressions
blah
A plain word refers to a variable in the current environment.
"blah"
A quoted word is a string, a value containing piece of text.
12
A number value.
-12 1.5 3.4e10
Other ways to write numbers (negative, fractional, with exponent).
true
Boolean (yes/no) value. true for yes, false for no.
Operator expressions
a + b
Binary operator applied to two values. + to add, - to subtract, * to multiply, / to divide.
(a + b) * c
Parenthesis for explicit grouping.
a < b
Comparison operators ==, != (not equal), <, >, <= (less or equal), >=.
a = b
Assignment, set variable a to value b. Not to be confused with == comparison. a += b is a shorthand for a = a + b, also for -= etc.
a && b
Logical operators — && for AND, || for OR.
-a
Unary (one-operand) operator. - to negate, ! for boolean negation.
Composite expressions
a[b]
Subscript, fetch the field named by b from value a.
a.x
Shorthand for a["x"].
a(b)
Function call. Call the function value a with b as argument. Zero or more argument expressions can be given, separated by spaces. a(1, 2, 3, 4)
a.x(b)
Method call. Call the function found in field x of value a, and pass a as the thisargument.
[1, 2, 3, 4]
Array value with zero or more elements.
{a: 1, b: 2}
Object value with zero or more name: value field definitions.
function(arg1, arg2) { /* ... body ... */ }
Function value. Zero or more argument names. Any statements may appear in body.
Statements
a;
Any expression, followed by a semicolon, is a statement.
{a; b; c;}
A series of statements, wrapped in braces, form a composite statement.
var a = b;
Variable definition. The variable with name a is defined and given value b. Value is optional. var a; sets a to undefined.
function foo(arg1, arg2) { /* ... body ... */ }
Function definition. Defines variable foo to have a function value. Zero or more arguments, any statements may appear in body.
if (a) { /* ... */ } else { /* ... */ }
Conditional statement. If value a is true, the first statement, otherwise the else statement executes. Else part may be left off. Can be chained as in if (a) {} else if (b) {} else {}.
while (a) { /* ... */ }
A loop. The loop body statement will be executed as long as a produces a true value.
for (var a = 0; a < 10; a = a + 1) { /* ... */ }
Example for-loop statement. var a = 1 initializes the loop, a < 10 checks whether it has ended yet, and a = a + 1 moves to the next step.
return a;
Only valid inside a function. Returns value a as the result of the function call.
Useful functions
Number(v)
Converts v to a number. Number("5") gives 5.
String(v)
Converts v to a string.
alert("hello")
Show a dialog window saying 'hello'.
confirm("are you sure?")
Show a yes/no dialog. Returns a true/false value indicating whether the user clicked yes.
prompt("what is your name?", "")
Show a dialog asking for input. First argument is the message, second argument is the initial value of the input.
Useful string properties
"foo".length
The length (number of characters) of the string.
"foo".charAt(n)
Get the character at position n. (Zero is the first character.)
"foo".slice(from, to)
Get a piece of the string. "012345".slice(1, 4) gives "123".
"a b c".split(" ")
Split the string on a character, producing an array of strings (["a", "b", "c"]).
Useful array properties
a[i]
If i is an integer, this will access the element at that position.
a.length
The number of elements in the array.
a.push(b)
Add value b to the end of the array.
a.pop()
Remove the last element of the array, and return it.
a.slice(from, to)
Get a piece of the array, similar to the slice method on strings.
Useful math properties
Math.random()
Produce a random number between 0 and 1.
Math.round(x)
Round x to an integer.
Math.abs(x)
Returns the absolute (positive) value of x.
Math.max(a, b, c, ...) Math.min(a, b, c, ...)
Given any number of values, returns the greatest (max) or smallest (min) one.
Math.PI
The pi (π) constant.
Math.cos(x) Math.sin(x) Math.tan(x)
Trigonometric functions.
Math.acos(x) Math.asin(x) Math.atan(x)
Inverse trigonometric functions.
