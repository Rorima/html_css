# Notes

[Course link](https://www.youtube.com/watch?v=cyuzt1Dp8X8&ab_channel=BroCode)

Where I stopped: 4:17:00

[HTML best practices](https://www.youtube.com/watch?v=e3jhKg1ozvw&ab_channel=TheCodingWays)

These are all of the notes I took while studying the HTML5 & CSS3 course made by [Bro Code](https://www.youtube.com/@BroCodez). I have to learn this first before going further on a Django course. Keep in mind that these notes are for ME. I did not make them with someone else in mind that might use this for their learning, so there will be things in here that only I will understand.

Inside each folder there will be studying files, which are files that I wrote following the teacher, and practice files, which are files that I wrote after I studied, trying to apply what I've learned. Most of the time, in practice files, I just try to repeat what I learned, but without looking at the original code.

### What is HTML?
* HTML is an acronym for: Hypertext Markup Language.
* It is a declarative language, not computational (Python, PHP, Javascript)
* It is used to declare what should exist on a web page
* Your web browser will take an .html file, read it, and display it as a web page

#### HTML advantages
* Easy to learn!
* Easy to use!
* Easy to write!
* Web developer jobs are high in demand (You'll want to learn CSS and Javascript)

#### HTML disadvantages
* HTML by itself is ugly, no style (CSS)
* Static nature, no animations (Javascript)
* Unpredictable behavior across web browsers
* Little to no jobs if you ONLY know HTML

#### Where to start?
For beginner front end developers, you should start with HTML, then go to CSS and after that go to JavaScript. Each of these languages has a specialty and they work well together.

Think of building a website as being similar to constructing a house. HTML acts as the foundation, as the skeletal framework of our house, including walls, doors, roofing and etc. But we would want to eventually decorate our house when we are done building it. That's when CSS comes in. CSS would be us painting, decorating and furnishing our house. Lastly, JavaScript adds dynamic life to our webpages. In our house analogy, this would be similar to us adding electricity, gas, lighting and plumbing. It adds functionality to our website.

#### What you will need:
1. Web browser
  * Google Chrome
  * Firefox
  * Safari
  * Microsoft Edge
  * DO NOT USE INTERNET EXPLORER

2. Text Editor
  * Sublime Text
  * Atom
  * Visual Studio
  * Notepad++

#### Writing your first file
Create a file called `index.html` and write whatever you want inside of it. Save it wherever you want and open it with one of the web browsers listed above. You'll see your text displayed in your browser.

One thing you may want to do is to have your text editor and your web browser side by side, so you can easily make any changes to your HTML file and see them by refreshing the web page.

This `index.html` file can be named whatever you want, but it is good that your main file be named `index.html` because that's what your browser will firstly search for in the folder of your web page. So keep in mind that you can have files with other names inside the folder of your web page.

#### Tags
In HTML we use a series of tags that describe how we want our website to look and what content we want on it. Different tags have different effects on our website.

What we are going to be doing here is creating a skeletal structure of our website. Think of it as all of the support beams of our house in our previous example.

Type this at the first line of your `index.html` file:

`<!DOCTYPE html>`

This defines the document as being of the current version, which is currently HTML5. It tells the web browser that this is an HTML document.

---

Now, you are going to write the HTML tags. Generally (not always), every tag has its pair. One is used for opening and the other for closing. This lets the browser know where the effects of the tag begin and where they end. The one used for closing has a forward slash before its name. Type this on the following lines of your file:

```
<!DOCTYPE html>

<html>

</html>
```

These html tags are going to act as a container that will hold all of our tags and text for our web page. This means that we always want to have some room between these two html tags.

---

The next set of tags we'll need is the head tags. You'll write them inside the html tags. Make sure to indent your tags if they're inside another set of tags. Indenting doesn't make any difference in how the browser will read your file, but it helps you read the code with more ease.

```
<!DOCTYPE html>

<html>

    <head>
    </head>

</html>
```

This head element contains meta information about this document. It describes information about this document to the web browser. Think of it like the settings of this document.

---

If we have a head element, we will also want to have a body element, so we're going to put that withing the HTML tags, but after the head tags.

```
<!DOCTYPE html>

<html>

    <head>
    </head>

    <body>
    </body>

</html>
```

All of our content will go into the body tags. So, anything you want to add to your web page, you'll want to put within the body tag so it can be displayed.

---

Inside the head we can have title tags that will give our website the title we want it to have.

```
<!DOCTYPE html>

<html>

    <head>
        <title>THE BEST WEBSITE</title>
    </head>

    <body>
    </body>

</html>
```

---

This is the skeletal structure of our website. They are the minimum requirements to build a solid foundation for our website. If you want to add text into your web page, you can type it inside the body tags. These are all of the tags we learned so far:

```
<!DOCTYPE html>

<html>

    <head>
        <title>THE BEST WEBSITE</title>
    </head>

    <body>
        Look! I'm coding! I'm a super duper coder! * emoji using sunglases *
    </body>

</html>
```

#### Comments
Comments are useful if you need to insert some sort of note for yourself or for somebody else that's looking over your HTML document. When you insert a comment, it won't actually appear in your web page, but it will appear in your HTML document.

`<!-- This is how you make a comment -->`

```
<!-- 
This comment 
can go over 
multiple lines too!
-->
```

#### Headings
Heading tags are used to show the structure of a document by transforming text to become headings such as titles, category markers or sections. By default there are six sizes of headings that you can apply to text. They're h1 through h6, where h1 is the largest heading, and h6 is the smallest.

Code example:

`<h1>This is the main heading</h1>`

Complete code example:

```
<!DOCTYPE html>

<head>
    <title>My Website</title>
</head>

<body>

    <h1>Largest Heading</h1>
    <h2>Slightly smaller heading</h2>
    text

</body>

</html>
```

Whatever text is enclosed within these tags, will be displayed by the respective tag.

#### Paragraphs
Sometimes you'll want some text displayed in your website just to test how it will be displayed to the user. Using VS Code, you can type the word lorem and press ENTER. This will give you a full paragraph written in Latin. It is used a lot in web programming.

If you want to separate some text and have it become its separate paragraph, just use the paragraph tag. This will split up the text and turn it into a paragraph.

Code example:

```
<p>
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugit culpa provident architecto maxime nisi hic itaque natus obcaecati. Ex cumque labore sequi laudantium atque totam assumenda! Blanditiis neque impedit sit.
</p>
```

#### Spacings
After some time you're going to notice that the empty lines in your document do not appear in your webpage. So if you want to add blank lines to your web page, use the `<br>` tag. You don't need a closing to this tag. It's one of the few exceptions where you don't need to add an ending to it.

---

The tag `<hr>` is used to separate the page with a straight line, also known as horizontal ruler. It is useful if you want to mark something off, like section by section for example. This is also an empty tag, so you don't need a closing for this one.

```
<h1>Heading 1</h1>
<hr>
<h2>Heading 2</h2>
<hr>
<h3>Heading 3</h3>
<hr>
<h4>Heading 4</h4>
<hr>
<h5>Heading 5</h5>
<hr>
<h6>Heading 6</h6>
```

---

You might have noticed that your whitespaces are not shown. No matter how many whitespaces you add between two words, it will not show. So if you want to add a few spaces, you need to use the non-breaking-space, or shortened `&nbsp;`.

```
<p>
    Lorem, &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ipsum dolor sit amet consectetur adipisicing elit. Fugit culpa provident
    architecto maxime nisi hic
    itaque natus obcaecati. Ex cumque labore sequi laudantium atque totam assumenda! Blanditiis neque impedit sit.
</p>
```

You can also use the non-breaking-space to indent paragraphs. Just add four `&nbsp;` above the text and the first line of your paragraph will be indented.

```
<p>
    &nbsp;&nbsp;&nbsp;&nbsp;
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates nam voluptas corporis
    ex optio vel maiores
    similique beatae doloremque. Consequatur sequi, voluptatem expedita ut fugit facere est aliquam illo
    consectetur.
</p>
```

#### How should you name your HTML files?
* Try not to use special characters. For best results, use only letters, numbers, underscores, periods and hyphens;
* Don't use spaces. They can be read by your computer, but web pages can't handle them;
* Start your file name with a letter. Some programming languages give numbers a special notice, and might not treat a file starting with a number as you intended;
* Use all lowercase letters. Your computer might see uppercase and lowercase file names as the same, but web servers are case sensitive;
* Keep your file names short. Less than four words and between 30 to 50 characters are ideal. It is good to indicate their content or purpose with a meaningful title;
* Remember to add the HTML file extention;

#### Text formatting
Remember to open and close these tags. Add the text you want to be affected between them.

|Code|Effect|
|:---:|:---:|
|`<b></b>`|Bold text|
|`<i></i>`|Italic text|
|`<sub></sub>`|Subscript text|
|`<sup></sup>`|Superscript text|
|`<small></small>`|Small text|
|`<big></big>`|Big text|
|`<ins></ins>`|Inserted text (underlined)|
|`<del></del>`|Deleted text (crossed horizontally)|
|`<mark></mark>`|Marked text (highlighted)|

#### Links and images
Before we begin this lesson, you'll want to be sure to download a couple of images. Four is a good number. Place these images in the same folder your HTML file is in. 

To include links and images in our web pages, we first need to understand what are attributes. All elements in HTML have attributes. Attributes provide additional information about an element that contains an attribute. They're used in the opening tags of an element and come in name-value pairs.

They're useful because we can provide links to web pages, we can include images, and even specify the styling of an element, but we'll learn that in the future.

##### HTML links
A link is defined with the `<a>` tag, and you need a closing tag for that too. Now you're gonna need some text that will function as the link. For example, let's say that we want to create a link that will take us to Google's homepage.

Code example:

`<a>Go to Google's homepage.</a>`

If you click on the link, nothing will happen. You have to give an attribute to the `<a>` tag. This tag makes any text that is sorrounded by it become a hyperlink that can link this text to another web page that you specify. In order to specify the web page, you're going to use the `href` attribute. This is an acronym for Hypertext Reference. We set this equal to whatever website we want to link this hyperlink to. Make sure to put the website inside double quotes.

`<a href="http://www.google.com">Go to Google's homepage.</a>`

Open hyperlink in a new tab:

`<a href="http://www.google.com" , target="_blank">Go to Google's homepage.</a>`

##### Download link
It works almot the same as the previous code. We just need to add the path to our file into the href's double quotes, or only the name of the file if the file is in the same folder as the HTML file. After writing the name of the file, write `download` as the second argument and set it equal to the name you want your image to have when it's been downloaded.

Code example:

`<a href="angel.png" , download="Angel">Download a machine generated image.</a>`

##### Add a picture to your web page
You can use the `<img>` tag to add pictures to your web page. This tag is self closing, so you don't need to add another tag to close it. Inside this tag you're going to write `src` which is short for source, and inside the quotes you add the path to your image. It can be a path in your machine, or a web address, or just the name of the file, if it's in the same folder as your HTML file.

Code example:

`<img src="church.png>"`

---

In order to add images from other folders in your computer, you'll have to get the absolute path to that image. You can see the absolute path of that image in its properties (right clicking it and then clicking in "properties"). Put that path into the `src` and the image will be displayed.

Code example:

`<img src="C:\Users\Micro\Desktop\Tudo\desenhos\coragem.png">`

---

Theres a height and width attribute that we can include within the tag to resize the image.

`<img src="church.png" , height="250" , width="250">`

---

You might notice that depending on the resolution of your image, you can get a stretched image, and that's rarely what you want to display to your user. To avoid that, you can pass percentages instead of pixels to `height` and `width`:

`<img src="church.png" , height="20%" , width="20%">`

One advantage of using the percentage system is that the image will be resized according to the zoom of the page.

---

And if for some reason the image is not displayed, you can add an alternate text to be displayed instead with the `alt=""` argument:

`<img src="church.png" , height="20%" , width="20%" , alt="Image of a golden church">`

##### Image hyperlink
You can have an image also function as a hyperlink when you click on it. First choose your image and display it on the screen, then surround it with the `<a>` tag:

`<a href="http://www.google.com" , target="_blank"><img src="japan.png" , height="50%" , width="50%" , alt="Picture of japan atificially generated"></a>`

#### Lists
In this lesson, you're going to learn four types of lists in HTML. They are:

* Unordered List `<ul></ul>`
* Ordered List `<ol></ol>`
* Description List `<dl></dl>`
* Nested Lists

##### Unordered list
This is useful if you want to create a list and the order doesn't really matter. A grocery shopping list is a good example. The unordered list uses the tags `<ul></ul>`. In order to list your items inside this list, you'll have to use the list item tag `<li></li>` for each item.

Code example:

```
<h3>Grocery List</h3>
<ul>
    <li>Bread Dough</li>
    <li>Tomato Sauce</li>
    <li>Chesse</li>
    <li>Peppers</li>
</ul>
```

---

If you want to change the bullet points of the list, you have a few options if you use CSS. On the starting `<ul>` tag, write the following argument:

`<ul style="list-style-type:">`

And then choose one of these types:
* circle
* square
* none
* disc (default bullet point)

##### Ordered lists
You can use the `<ol></ol>` tags to create ordered lists. The process is very similar to the previous list. The items will be ordered as you add them to your list.

Code example:

```
<h3>My To-Do-List:</h3>
<ol>
    <li>Study Programming</li>
    <li>Study Music</li>
    <li>Read the Bible</li>
</ol>
```

---

And you can also change the style of your ordered list:

`<ol type="">`

You can choose the following styles:

* A (Display items with uppercase alphabet letters)
* a (Display items with lowercase alphabet letters)
* I (Display items with uppercase Roman numerals)
* i (Display items with lowercase Roman numerals)
* 1 (Display items with numbers)

---

You can choose on which number your list will start:

```
<h3>Starting from 100:</h3>
<ol start="100">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
```

You can apply that to Roman numerals or other styles.

##### Description lists
The description list is also referred to definition list. It is a list of terms or items with a descriptions for each specific item. You have to use the `<dl></dl>` tags to make a description list. Now, instead of writing `<li>` for "list item", you'll have to type `<dt></dt>` for "description term", or "definition term".

Code example:

```
<h3>Web Development Languages</h3>
<dl>
    <dt>HTML</dt>
    <dt>CSS</dt>
    <dt>JavaScript</dt>
</dl>
```

In order to add descriptions details you'll have to use another tag called `<dd></dd>` right after the item.

```
<h3>Web Development Languages</h3>
<dl>
    <dt>HTML</dt>
    <dd>Adds structure to a web page</dd>

    <dt>CSS</dt>
    <dd>Adds style to a web page</dd>

    <dt>JavaScript</dt>
    <dd>Adds functionality to a web page</dd>
</dl>
```

##### Nested list
You can create a whole new list inside the "list item" tags, and then you can add your subitems. You can use any type of list you want to make nested lists.

```
<h3>Grocery List 2.0:</h3>
<ul>
    <li>Bread Dough</li>
    <li>Tomato Sauce</li>
    <li>Cheese</li>
    <li>Toppings
        <ul>
            <li>Peppers</li>
            <li>Pepperoni</li>
            <li>Mushrooms</li>
        </ul>
    </li>
</ul>
```

#### Tables
Tables are used to display information. It's useful if you want to organize information in rows and columns. In order to create tables, you'll need a pair of table tags: `<table></table>`.

In order to create rows, you'll use the table row tag: `<tr></tr>`. Anything inside these tags will be in the first table row.

If you want this first row to be the heading, inside it write the pair of tags `<th></th>`. If you want just to display data, use the table data tag pair: `<td></td>`.

Code example:

```
<h2>Personal Finances</h2>
<table>  <!--Creating the tab.-->
    <tr>  <!--Creating the first table row.-->
        <th>Month:</th>  <!--Creating the first heading.-->
        <th>January</th>
        <th>February</th>
        <th>March</th>
        <th>April</th>
    </tr>
</table>
```

All of these table headings are in the same row.

If you want to create another row, make sure to add another `<tr>` outside the one you created.

Code example:

```
<h2>Personal Finances</h2>
<table>
    <tr>
        <th>Month:</th>
        <th>January</th>
        <th>February</th>
        <th>March</th>
        <th>April</th>
    </tr>

    <tr>
        <th>Income:</th>
        <td>$123</td>  <!--Table data that will be displayed.-->
        <td>$123</td>
        <td>$123</td>
        <td>$123</td>
    </tr>
</table>
```

One thing to notice with tables is that table headings are bold and centered, while table data is not bold, and it's aligned to the left.

##### Adding borders to tables
You might notice that the table is getting harder and harder to read. One thing you can do is add borders around each individual cell. That will greatly help in the reading. Inside the opening table tag you can use the border attribute. You can set it equal to any number you want for the thickness (in pixels) of your border.

Code example:

`<table border="2px">`

---

##### Adding colors to tables
At the opening tag of the table row write `bgcolor=""` and set it equal to whatever color you want.

Code example:

```
<tr bgcolor="gray"">  <!--This whole row will be gray.-->
    <th>Month:</th>
    <th>January</th>
    <th>February</th>
    <th>March</th>
    <th>April</th>
</tr>
```

---

You can also change the background color of your whole table. Write the same attribute in the table tag instead of the table row tag.

Code example:

`<table , bgcolor="black" , border="2px">`

---

You can use hex colors instead of names if you want more precise colors:

`<tr bgcolor="#8be76a">`

##### Changing cell size
You can set width and height to each individual cell in your table with the `height=""` and `width=""` attributes.

Code example: 

`<th height="10" , width="75">Month:</th>`

You'll notice that the dimensions of the cells of the same column will also change to be equal to the dimensions of the first cell in the column.

---

You can apply the `height=""` and `width=""` attributes to the table as a whole:

`<table height="300" , width="500" , bgcolor="black" , border="2px">`

---

You are not limited to pixels. You can also set the width and height to a percentage. The percentage applies to the room available on the page.

`<table height="30%" , width="50%" , bgcolor="black" , border="2px">`

##### Aligning text
You can align text in the space that's available to it. Use the tag `<align="">`. The values you can set it qual to is "left", "center", "right" and "justify". This will align the whole row if you place it in the `<tr>` tag.

`<th align="center" , height="10" , width="75">Month:</th>`

#### Audio
HTML5 only supports .mp3, .wav and .ogg. .wav and .ogg files don't work on all web browsers, but mp3 does. You'll need the audio tags in the body of your file if you want to add audio to your web page. Inside the opening tag, write `controls`, and it will display the audio controls in your web page.

Code example:

```
<audio controls>

</audio>
```

You'll need to list an audio file as a source. You can do that in two ways:

Using the `src=""` attribute:

```
<audio controls , src="mixkit-retro-game-notification-212.wav">

</audio>
```

Or using the source tag with the `src=""` attribute:

```
<audio controls>
    <source src="mixkit-retro-game-notification-212.wav">
</audio>
```

##### Message in case audio doesn't work
Not all web browsers support audio, so it's good to write a message between your audio tags in case the browser doesn't support it.

```
<audio controls>
    <source src="mixkit-retro-game-notification-212.wav">
    Your web browser do not support audio.
</audio>
```

##### Options:
There are a couple of options you can use:

`loop` (if you want to loop the audio)
`muted` (if you want the audio to be muted by default)
`autoplay` (play as soon as the web page is loaded. Not recommended. Might not work on all browsers and mobile devices)

You have to place them inside the opening audio tag.

Code example:

```
<audio controls loop muted>
    <source src="mixkit-retro-game-notification-212.wav">
    Your web browser do not support audio.
</audio>
```

Remember not to add commas between the attributes. It doesn't seem to work on Chrome.

#### Video
Before we begin you'll going to want to download a video. HTML5 only supports .mp4, .webM and .ogg files. Place the video within the same folder that contains your HTML file.

This process works the same as adding audio into your web page. So below you're only going to see the complete code on how to add videos to your web page.

```
<video controls src="SampleVideo_1280x720_1mb.mp4">Sample Video</video>
```

##### Width and height of the video
Using the `width=""` and `height=""` attributes, you can increase and decrease the amount of space your video is going to take on the screen. If you want a dynamic way to deal with space, use just width (for videos taken horizontally) and use percentages.

`<video controls width="100%" src="SampleVideo_1280x720_1mb.mp4">Sample Video</video>`

##### Video attributes:
The same attributes available to audio are available to video as well. They are: `mute`, `autoplay`, `loop`, `controls`. You can remove the controls if you want the video just to be playing in the background without the user having the ability to pause it. I don't know why you would do this, though.

#### Buttons
Use the `<button></button>` tags to create the buttons. Add any text between these tags and it will appear in the button. Note that the button tags should be inside the body. You can add a name and a type inside the opening tag. This will help when you add functionality to this button in the future.

```
<button name="simple_button" type="button">
    Click Me!
</button>
```

We need a programming language like PHP or JavaScript to add functionality to this button.

##### Types of buttons
There are three types of buttons: the plain vanilla button, the submit button and the reset button. You can also add a value, that will be useful to the programming languages.

Code example:

```
<button name="simple_button" type="button">
    Simple button!
</button>

<button name="submit_button" type="submit" value="Submit">
    Submit!
</button>

<button name="reset_button" type="reset" value="Reset">
    Reset!
</button>
```

##### Other attributes for buttons
There are a couple of attributes you can add to your buttons. They are: `disabled`, `autofocus` and `onclick="alert('your message')"`. You can also create a link button. See the code below.

```
<!--Displaying a disabled button-->
<button disabled>
    Disabled
</button>

<!--When the page is loaded, this button will be highlighted-->
<button autofocus>
    Autofocus
</button>

<!--A pop-up will show up on the screen with the message you typed-->
<button onclick="alert('type your message here')">
    Onclick
</button>

<!--Link button-->
<a href="https://www.youtube.com">
    <button>
        Go to YouTube button
    </button>
</a>
```

##### Styled button with CSS

```
<!--Styled button with CSS-->
<button style="background-color:#97f7cc; color:white; font-size:30px; font-family:monospace;">
    CSS Style
</button>
```

Remember that all of those attributes are inside the `style=""` double quotes. Each should end with a semicolon.

#### Forms
The form element is used to collect user input from a visitor to your site. It can be user information, payment info, surveys and etc. There are several form input elements, such as: text fields,  radio buttons, drop down lists, checkboxes and more. Use the `<form></form>` tags.

Usually in a HTML form there's an `action=""` attribute that you may find in the opening form tag, and it defines the action to be performed when the form is submitted. The data from the form may be sent to a page on the server. When the user clicks on the submit button, there might be a script within the action attribute that the form sends data to. We will talk about it in the future, when we talk about programming languages that go with HTML and CSS.

##### Creating a text box
Using the `<input>` tag, which is a self closing tag, you can create input for the user. You'll have to use the `type="text"` inside it to display a text box to the user.

Code example:

```
<form>
    <input type="text">
</form>
```

And you can also add a text before the text box to display to the user why the text box is there for:

```
<form>
    First Name:
    <input type="text">
</form>
```

Notice that because there isn't a `<br>` between `First Name:` and the input tag, both will be displayed in the same line.

##### Labeling the text before the text box
You can link a text and a text box together to act as one. Doing this, when you click on the text before the text box, the text box itself will be highlighted, and you'll be able to type in it. You'll need to surround your text with the `<label></label>` tags.

```
<form>
    <label>First Name:</label>
    <input type="text">
</form>
```

You'll have to use an attribute to give an ID to this label. This ID will be what will link your text to your text box. You can choose any name you want, just make sure it starts with a letter, and use underscores instead of spaces. The name of the attribute is `for=""`.

```
<form>
    <label for="first_name">First Name:</label>
    <input type="text">
</form>
```

Now, we have to use the `<id="">` attribute inside the input tag, and the name of the id will be the same as the value set for the `for=""` attribute above.

```
<form>
    <label for="first_name">First Name:</label>
    <input type="text" id="first_name">
</form>
```

Now, if you click on the label, it's going to place your cursor inside the text box. This id attribute is the cliend-side identifier. It is mostly used for CSS and JavaScript to uniquely identify this specific element.

##### The name attribute
It is common to set the name attribute to be the same as the id attribute. It is used during form submission to post or get the values that one is submitting. This is only used when a server side language is used, like PHP. These attributes won't be really usefull for this particular tutorial, at least not right now, but it's good to get used to them.

```
<form>
    <label for="first_name">First Name:</label>
    <input type="text" id="first_name" name="first_name">
</form>
```

##### Placeholder
You can set a placeholder for the user to know what to type inside your text boxes. This placeholder text is going to be displayed gray, as a tip to what the user should type. Use the `placeholder=""` attribute inside the input tag to set what it will be.

```
<form>
    <label for="telephone_number">Telephone Number</label>
    <input type="text" id="telephone_number" name="telephone_number" placeholder="(999) 999-9999">
</form>
```

##### Form buttons
There's another way to create buttons, and to do that, we use the input tags. We can set it to two different button values: reset and submit. Let's see the reset button first:

`<input type="reset">`

The reset button is going to clear all your text boxes.

The submit button can be implemented in the same way, but it will not work if you have not set a value for the `action=""` attribute placed in the opening form tag. We talked about it in the beginning of this lesson.

`<input type="submit">`

#### Advanced form
Here you're going to learn a couple more attributes and tags that you can use in your forms. Remember that both the label and the input should be inside the `<form></form>` tags

##### Radio buttons: input attribute
Radio buttons, also called option buttons, let users select one option from a collection of two or more mutually exclusive, but related, options.

`<input type="radio">`

In order to make it mutually exclusive, you'll have to set the name attribute to be the same in all of the radio buttons. The id should be set to the same value as the for attribute.

```
<label for="title">Title:</label>

<br>

<input type="radio" name="title" id="mr">
<label for="mr">Mr.</label>
<br>
<input type="radio" name="title" id="mrs">
<label for="mrs">Mrs.</label>
<br>
<input type="radio" name="title" id="miss">
<label for="miss">Miss</label>
<br>
<input type="radio" name="title" id="phd">
<label for="phd">PhD</label>
```

In this case, all of their names is set to `"title"`. This means that we can select only one of them at a time.

##### Select tag
The select tag will display a drop down menu. You have to use the option tag to add an option to the drop down menu. Both tags are not self closing, so you have to close them. The option tag has a value attribute. You can set it the same value you would set a name attribute.

```
<label for="payment">Payment Method</label>

<select name="payment" id="payment">
    <option value="visa">Visa</option>
    <option value="mastercard">Mastercard</option>
    <option value="gift_card">Gift Card</option>
    <option value="check">Check</option>
</select>
```

##### Email: input attribute
This attribute is almost the same as the text attribute. The main difference is that it doesn't let the user submit an email that doesn't have an @ sign.

```
<label for="email">Email</label>
<input type="email" placeholder="your.email@email.com">
```

##### Birthday: input attribute
This will give the user a little GUI with a drop down menu to choose their birthday.

```
<label for="birthday">Birthday:</label>
<input type="date" id="birthday" name="birthday">
```

You can use a couple of attributes to limit the minimum and maximum date:

```
<label for="birthday">Birthday:</label>
<input type="date" id="birthday" name="birthday" min="2000-01-01" max="2001-01-01">
```

The date format for these two attributes is yyyy/mm/dd.

##### Number: input attribute
This will display a little box where the user can only input numbers. You can also limit the minimum and maximum amount.

```
<label for="quantity">Quantity:</label>
<input type="number" id="quantity" name="quantity" min="0" max="10">
```

---

Using the `value=""` attribute you can set a default quantity:

```
<label for="quantity">Quantity:</label>
<input type="number" id="quantity" name="quantity" min="0" max="10" value="5">
```

##### Telephone: input attribute

```
<label for="phone">Phone Number:</label>
<input type="tel" name="phone" id="phone">
```

##### Password: input attribute
This will display a password box. You can add the `minlengh=""` and `maxlengh=""` attributes.

```
<label for="pass">Password:</label>
<input type="password" name="pass" id="pass" minlength="3" maxlength="12">
```

##### Range: input attribute
This creates a sliding bar.

```
<label for="slider">Range:</label>
<input type="range" name="slider" id="slider">
```

You can add steps using the `<step="">` attribute. It is preferable that you choose a value that is divisible by 100.

```
<label for="slider">Range:</label>
<input type="range" name="slider" id="slider" step="25">
```

The number 0 is also counted as a value, so the sliding bar will have 5 different positions with this setting. This means that if you made the value 20 instead of 25, you would end up with 6 different positions instead of just 5.

---

You can set a default value:

```
<label for="slider">Range:</label>
<input type="range" name="slider" id="slider" step="25" value="100">
```

##### Check boxes: input attribute

```
<label for="check">Check:</label>
<input type="checkbox" name="check" id="check">
```

##### Upload files: input attribute

```
<label for="myfile">Upload a File:</label>
<input type="file" name="myfile" id="myfile">
```

---

To limit which file extensions will be accepted use the `accept=""` attribute. Separate each file extension with a comma.

```
<label for="myfile">Upload a File:</label>
<input type="file" name="myfile" id="myfile" accept=".txt,.pdf">
```

#### Meta tags
Meta tags are used for meta data, which is information about data. Think of it as data about data. We place meta tags within the head of our HTML document. Meta data has some use for search engines and web browsers. They let these entities and the web browser know what your web page is about and what kind of content it contains.

There are other uses of meta tags too that allow us to control the viewport which is the visible area of a web page when you switch devices such as if you're viewing a page in a mobile device or a tablet, a laptop and so on.

The meta tag is self-closing. All the things you're going to add to it are attributes. You can have several meta tags in one file.

##### Charset
This will let the web browser know what character set we're using. There are many, such as ASCII, ASNII, UTF-8 and so on. You'll always want to set this to unicode, which is UTF-8. It has almost all characters you might want to display in your web page. But you can search and leanr more about each charset.

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Meta Tags</title>
</head>
<body>
</body>
</html>
```

##### Name
You can use this attribute for many things in your web page. Here's a few things you can do with it.

###### keywords
You can set the name attribute equal to "keywords", and you'll be able to define some keywords about your web page for search engines like Google or Bing to identify. To set the keywords you have to use the content attribute. Inside the content attribute you can describe your web page using a few keywords.

`<meta name="keywords" content="HTML,tutorial,Bro Code,YouTube">`

These are keyword search terms, and depending on what you place in here, it will help in the ranking of your website.

###### description
Set the name to "description" and with the content attribute, you can add a short description about your web page. Search engines can pick up this description and learn what your web page is about.

`<meta name="description" content="Bro Code HTML tutorial for beginners">`

###### author
You can also set an author for your web page.

`<meta name="author" content="Me">`

###### viewport
There will be a little explanation for this one. We're going to set the viewport for our website. The viewport is the visible area of a web page, depending on which device is being used to access the page. If the user is using a mobile phone or a tablet, you want to be sure that the dimensions will fit on the device, so that the dimensions and the scaling will adjust to accomodate that specific device.

Type this in the meta tag.

`<meta name="viewport" content="width=device-width,initial-scale=1.0">`

These are instructions to the web browser to change the scaling and dimensions to match the divce you're using to view that page. The initial scale is set to 1, and that will set the zoom level when the page is first loaded. So if you want your page to be displayed better in mobile devices, you have to include this tag.

###### http-equiv
This attribute will make your page refresh after the set amount of seconds. You can set the amount of seconds with the content attribute. This is not really recommended unless you have a very good reason for using it, but here it is for demonstration purposes.

`<meta http-equiv="refresh" content="3">`

##### Example of meta tags being used:
This is more or less how your HTML document should look like:

```
<!DOCTYPE html>

<html>

<head>
    <meta charset="UTF-8">
    <meta name="keywords" content="HTML,tutorial,Bro Code,YouTube">
    <meta name="description" content="Bro Code HTML tutorial for beginners">
    <meta name="author" content="Me">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <meta http-equiv="refresh" content="3">
    <title>Meta Tags</title>
</head>

<body>
    <h1>Test</h1>
    <p>Hello, Hello!</p>
</body>

</html>
```

#### Colors
In this lesson we're going to cover some basic coloring techniques using the style attribute. This attribute contains some information about how to style a whole or part of a web page. This is part of CSS. There are a lot more things you can do with the style attribute, but for now, let's just learn some basic colors. 

We can apply an inline style attribute to nearly any HTML element. Here are a couple of color attributes you might want to use in your web pages:

##### background-color
You should type this in the opening body tag of your file. You can use hex values, RGB or just type the name of the color. We're going to use hex values for this lesson.

`<body style="background-color:#9c86e4;">`

##### color
Because you can use this inline style attribute in a lot of elements, you can use them inside the paragraph tags as well to set the font color:

`<p style="color:#dadada;">Your paragraph</p>`

---

You can also have other color attributes inside the same style. Just make sure to separate them with a semicolon:

`<p style="color:#dadada;background-color:#2d2d2d;">Your paragraph</p>`

#### Span and div tags
The span and div tags define a section or division on a HTML page. Typically we use a pair of these tags as a container for HTML elements, so that we can style something specific with CSS or perform some sort of procedure with JavaScript with anything marked with these tags.

##### span
We can target an element or a portion of our web page that we want to style. It depends on where we place our span tags. Let's say that we want to change the color of a single sentence in a paragraph. Just add a span tag around whatever you want to target and add the attributes you want this part to have.

Painting the first sentence red:

```
<p><span style="color:red;">Lorem ipsum dolor sit amet consectetur adipisicing elit.</span> Tempore fuga dolorum facilis recusandae quia autem dolorem. Explicabo impedit consequatur delectus provident ipsam facilis eveniet voluptatem mollitia beatae velit, expedita autem.</p>
```

##### div 
This tag is almost identical to the span tag, however, anything inside the div tags is considered a block level element. This means that whatever is put within these tags will become a block in your web page. So if you use it in a text, the part that is within the div tags will be separated from the paragraph by a new line. This happens because the division will take the whole width of your web page.

```
<p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. <div style="color:blue;">Nihil aliquam non qui molestiae exercitationem voluptatum ad adipisci eius temporibus tempore nobis magni quis</div>, placeat commodi, totam sunt rerum culpa quisquam.</p>
```

### What is CSS?
CSS is an acronym for Cascading Style Sheets. The purpose of CSS is to customize the elements and layout of a web page. We can use it to style multiple pages at once by linking separate, independed HTML files to a single style sheet.

There are three ways to include CSS in a web page.

* Inline
 We have already some experience with this using the style attribute. It's useful for adding few custom elements.
* Internal
 We create a pair of style elements in the head of our HTML document. It is useful for a single page website.
* External
 We can link a CSS file to our HTML file to style one or all pages of our website. It is useful if you make a website with many pages.

#### Declaring CSS properties
There is a set of rules for declaring CSS properties. First, you'll want to identify the HTML element that you want to costumize.

```
h1{color:green;}
```

h1: element
color: property
value: green

This won't work for inline.

#### Inline customization
We already learned this in the HTML tutorials. Type the style attribute inside the opening tags of what you want to customize and choose a value. You can add several properties, just make sure to separate each with semicolons.

`<h1 style="background-color: green; color: white;">CSS Demo</h1>`

This will only affect this exact pair of h1 tags. If you have more, they'll not be affected. That's because when you use inline CSS styling, it will only affect what is inside of.

#### Internal customization
With internal CSS styling, we can target all instances of a certain tag that is used. Write a pair of style tags between the head tags. This is not a self-closing tag.

Now you need to list the HTML elements you want to target with CSS. Let's say that we want to target any instances of paragraph tags. Type the name of the tag without the angle brackets, then type a set of curly brackets and inside them, type all the customizations you want to make.

```
<head>
    <style>
        p{
            color:red;
            background-color: green;
        }
    </style>

    <title>Introduction to CSS</title>
</head>
```

##### Targeting ids
You can target HTML elements that have a particular id that you gave to it. Type the hash symbol (#) and after it, type the name of the id.

```
<head>
    <style>
        p{
            color:red;
            background-color: green;
        }

        #paragraph4{
            color:aqua;
            background-color: blueviolet;
        }
    </style>

    <title>Introduction to CSS</title>
</head>
```

##### Targeting classes
There's a similar attribute to id, which is called class. It is reserved to a unique grouping for parts of your web page. Firstly, write the class attribute inside the opening tags of the elements you want to change:

```
<p class="top-content">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>

<p class="top-content">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
```

Then target it at the top of your file. The process is very similar to the id target, but instead of using the hash symbol, you're going to use the dot (.) and then the name of the class.

```
<head>
    <style>
        .top-content{
            color: azure;
            background-color: burlywood;
        }
    </style>

    <title>Introduction to CSS</title>
</head>
```

###### Targeting tags that are grouped in classes
You can target specific tags that are grouped in your classes. This means that if you have several tags grouped in one class, you can target one specific tag to change while the others will not be affected. Instead of using just the dot, use the name of the tag plus the dot to target a specific tag.

```
h2.top-content{
    color: aliceblue;
    background-color: brown;
}
```

This means that all instances of h2 tags that have the class "top-content" will be changed to those colors. Other h2 tags will not be affected, nor other tags that have the "top-content" class.

##### Targeting several tags at once
Type the tags and separate them by a comma.

```
p,h1,h2,h3{
    color:red;
    background-color: green;
}
```

#### External customization
The external method of CSS styling is extremely useful because all you would need to do is have a single CSS file, and all you would need is to include the link to the web page you want to style with the CSS properties. So if you have a website with 50 different pages, you wouldn't have to type every single customization to each page. You could just link your CSS file to the 50 pages.

Create your HTML file normally, and create another file in the same folder with the ".css" extension. It can be called whatever you want. You can work on this CSS file in the same way you worked between the style tags in your HTML file. The main difference is that you don't need the style tags in here.

Code inside the "style.css" file:

```
h1{
    color: blueviolet;
}
```

You'll notice that nothing will happen to your web if you type these things inside the CSS file. That's because we have to link this CSS file to our HTML file. Use the `<link>` tag to do that.

##### Link tag
This tag should be placed between the head tags of your HTML file. It is a self-closing tag. There are a couple of attributes you can place inside the link tag. 

###### rel
The attribute `rel=""` indicates the relationship between files. Inside the double quotes you should type "stylesheet".

```
<link rel="stylesheet">
```

###### type
The second attribute is the `type=""`. It's not required, but it's considered good practice to include it. Its value is "text/css".

```
<link rel="stylesheet" type="text/css">
```

###### href
This attribute stands for Hypertext Reference. We place either the file name, the file path, or the URL of the CSS file that we want to link here.

```
<link rel="stylesheet" type="text/css" href="style.css">
```

As soon as you run your page again, it should be styled.

#### Fonts
Fonts are a set of characters of a particular style. There are two categories of fonts. There are Serif and Sans-serif. Serif is a typography term for small lines or embelishments on certain areas of individual characters. They are like little edges that stick out. Sans-serif means without serif. Do search online for images if you don't know what serifs are. Generally, Sans-serif fonts tend to be better to read on a computer screen, but you are free to choose whatever you want.

##### font-family
You can list a few different fonts that you want to use. You have to list fonts because if for some reason the browser of the user doesn't recognize the font, it will jump to the next one in the list of fonts you provided. For that reason, it is important to choose as your last fonts, the ones that are supported by all browsers, which are the ones that are known the most.

One thing to keep in mind is that you have to write the name of the font without quotes, unless the name of the font has a space, then you have to type it between quotes.

A couple of fonts you can use:

* "Ink Free"
* Helvetica
* Times
* "Times New Roman"
* "Gil Sans"
* Georgia
* sans-serif (as last resource, because it works in pretty much any browser)

Code example:

```
#p1{
    font-family: "Ink Free", "MV Boli", sans-serif;
}
```

Make sure to separate each with a comma.

##### font-style
You can set this to:

* normal
* oblique
* italic

Code example:

```
#p2{
    font-family: sans-serif;
    font-style: italic;
}
```

##### font-weight
You can set this to `normal`, `bold`, `bolder`, or a value that you want between 0 and 1000. This will add weight to your font, making it bold.

Code example:

```
#p2{
    font-family: sans-serif;
    font-style: italic;
    font-weight: 600;
}
```

##### font-size
The default value for font-size is 16px. There is another unity of measure called `em`, and the default is 1 (which is equal to 16px).

Code examples:

`#p2{font-size: 2em;} <!--This is the same as 32px-->`

`#p2{font-size: 20px;}`

##### text-decoration
You can choose several decorations and styles for these decorations.

Decorations:

* line-through
* underline
* overline
* normal

Styles:

* underline wavy;
* underline double;
* underline dotted;
* underline dashed;
* underline solid;
* underline none;

And you can choose a color for the line as well:

* overline wavy red;

Code example:

`#p3{text-decoration: underline dotted;}`

##### Getting new fonts
You can use the Google Fonts API to get more fonts. Go to the website [fonts.google.com](fonts.google.com) and choose your font. After you choose your font, roll down the page and find a button called "Select" and after the select you will see the name of the font you choose. Then, after selecting, search for the button on the top of the page that says "View Selected Families". There you'll find two links, one for the HTML head and other for the CSS property. The link for the HTML file is written between angle brackets, and the property is just `font-family: 'font-name'`, where "font-name" is the name of the font you chose.

Code example in HTML head:

```
<link href="https://fonts.googleapis.com/css2?family=Aldrich&display=swap" rel="stylesheet">
```

Code example in CSS:

`#p3{font-family: 'Aldrich';}`

#### Borders
There are different styles of border, and you'll want to specify what kind of border you want. Using the attribute `border-style=""`. You can find online all styles available. We are only going to cover a few.

##### border-style
Here are the values you can choose:

* dashed
* dotted
* solid
* double
* groove
* hidden
* ridge
* inset
* outset

```
p{
    border-style: solid;
}
```

##### padding
You can add some space between the text and the border.

```
p{
    padding: 5px;
    border-style: solid;
}
```

##### border-width

```
p{
    border-style: outset;
    padding: 50px;
    border-width: 30px;
}
```

You can have a different thickness for each side of your border if you asign it four values instead of just one. The first value applies to the northern border, the second to the eastern, the third to the southern and the last to the western border. You cannot use commas to separate the values.

```
p{
    border-style: outset;
    padding: 50px;
    border-width: 30px 15px 30px 15px;
}
```

##### border-color

```
p{
    border-style: outset;
    padding: 50px;
    border-width: 30px 15px 30px 15px;
    border-color: blueviolet;
}
```

##### border-radius
This will give rounded corners for your borders.

```
p{
    border-style: outset;
    padding: 50px;
    border-width: 30px 15px 30px 15px;
    border-color: blueviolet;
    border-radius: 1000px;
}
```

The value doesn't need to be so high. It can also be in percentage. Experiment.

##### Targeting certain parts of the border

```
h1{
    border-bottom-style: dotted;
    border-top-style: solid;
    border-left-style: solid;
    border-left-color: blue;
    border-right-style: solid;
    border-right-width: 100px;
}
```

#### Backgrounds
Generally, if you want to change the background color of your page, you target the body. You can also target the whole HTML file by using the HTML tag inside the CSS file.

##### linear-gradient
A gradient is a gradual change from one color to another. In order to use this, type the name of the first color inside the parenthesis, and then the name of the second color.

```
html{
    background: linear-gradient(grey, black)
}
```

The gradient will only extent to where there is content in the page. If there's only a header in the page, there will be several sections of gradients that start and end. This is what you can do to make the gradient go from the beginning to the end of the page:

```
html{
    background: linear-gradient(grey, black);
    background-repeat: no-repeat; /* The gradient will not repeat */
    background-position: center;
    background-size: cover;
    background-attachment: fixed; /* Bg won't move when the page is scrolled */
}
```

---

You can have the colors flow in a different direction.

`background: linear-gradient(to right, grey, black);`

The gradient will flow to the right. The available positions are: top, right, left. To bottom is default.

##### Image
Below you have the syntax for how to add images if it is in the same folder as your document. You can do the same thing you did with the liner-gradient.

```
html{
    background-image: url("image-name.png/jgp");
}
```

##### Other tags
You can apply this same process to other tags, like `h1` and `p`.

```
p{
    background-image: url("bg-img.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    background-attachment: fixed;
}
```

#### Margins
Margins are used to create space around an element. It can be easy to mix up margins with padding because they both perform a similar task. Let's first create some content in our page and surround it with borders.

```
h1{
    border: 1px solid;
    width: 300px;
}

p{
    border: 1px solid;
    width: 250px;
}
```

The main difference between padding and margins is that padding is the distance between an item within an element and its border. Margin is the distance between HTML elements or the edge of the browser window.

```
p{
    border: 1px solid;
    width: 250px;
    margin: 25px;
}
```

You can also use percentages instead of pixels so that the page element will adjust to the page size.

##### Margin orientation

```
p{
    border: 1px solid;
    width: 250px;
    margin-top: 25px;
    margin-bottom: 25px;
    margin-left: 25px;
    margin-right: 25px;
}
```

###### Negative values

```
p{
    border: 1px solid;
    width: 400px;
    padding: 25px;
    margin-top: -25px;
}
```

###### Shorthand
This is a shorthand way of writing by stating all four values. The order is: top, right, bottom, left.

```
p{
    margin-top: 25px 75px 25px 75px;
}
```

###### Center the margin

```
#p4{
    margin: auto;
}
```

This will place your element in the center of the page no matter the size of the browser page.

#### Shadows
There are different kinds of shadow properties. They are text shadows, and box shadows. There are four values you can use inside the shadow respectively: horizontal, vertical, blur and color. In the horizontal displacement, if you give it a positive value, it will displace your item to the right, while if you give it a negative value, it will displace your item to the left. The same applies to the vertical displacement. Positive, go down; negative, go up.

##### Text shadows
Shadow do the right: `h1{text-shadow: 5px 0px;}`

Shadow to the left: `h1{text-shadow: -5px 0px;}`

Shadow downwards: `text-shadow: 0px 5px;`

Shadow upwards: `text-shadow: 0px -5px;`

Shadow diagonal: `text-shadow: 5px 5px;`

###### Blur and color

The magnitude of the blur effect is in pixels.

`text-shadow: 10px 10px 5px;`

Just type the name of the color after blur:

`text-shadow: 3px 3px 5px yellow;`

You can also type the name of the color without having any blur:

`text-shadow: 10px 10px yellow;`

If both vertical and horizontal values are 0 and you apply a color, it will seem like the text is glowing.

`text-shadow: 0px 0px 3px #00ff11;`

###### Two text shadows
You can make a fire effect by adding two different shadows to your text. In order to do this, place a comma after all values and then, add the values you want for the next shadow, following the same strucutre shown in the beginning of this lesson.

`text-shadow: 0px 0px 10px yellow, 0px -5px 10px red;`

##### Box shadows
This works the same as text shadows. The main difference is that box shadows change entire elements.

`box-shadow: 10px 10px 5px gray;`

Whole code example:

```
h1{
    margin: auto;
    border: 1px solid;
    width: 155px;
    padding: 25px;
    background-color: black;
    color: aliceblue;
    border-color: red;
    border-radius: 10px;

    text-shadow: 0px 0px 10px yellow, 0px -5px 10px red;
    box-shadow: 10px 10px 5px gray;
}
```

#### Pseudo-classes
Think of a pseudo-class as a special keyword that is used to define a special state of an element. It can do things like change the appearance of a button when users hover over it, make drop-down menues appear, style certain items in a list and etc.

For this lesson, we're going to create a link, a button and an unordered list. We will only change colors, but rememeber that you can change a lot of other things, like the opacity, add borders, change size, font, and etc.

##### Changing links
Type the name of the element, a colon and then the pseudoclass.

Changing the color for the link that hasn't been clicked yet:

```
a:link{
    color: #21dc00;
}
```

When the link has been clicked:

```
a:visited{
    color: blueviolet;
}
```

##### Changing buttons

When the user hovers the mouse over the button:

```
button:hover{
    background-color: red;
}
```

When the user clicks the button:

```
button:active{
    background-color: #d20000;
}
```

##### Changing lists

Changing the first item:

```
li:first-child{
    background-color: greenyellow;
}
```

Changing the last item:

```
li:last-child{
    background-color: greenyellow;
}
```

##### nth-child
You can change a specific item in a list:

```
li:nth-child(5){
    background-color: greenyellow;
}
```

Or change all odd numbers (you can change even numbers as well):

```
li:nth-child(odd){
    background-color: greenyellow;
}
```

You can also create a custom formula to target very specific items. You have to place this inside the parenthesis: `an+b`. You will substitute these letters with the values you want.

`a`: Cycle size. How many times do you want this to repeat;
`n`: Counter. It starts at 0;
`b`: Offset value.

Let's say that we want to target every third item within our list. So for our cycle size, we put 3. The n can be n, because it starts with 0. There will be no offset, so we will set it to 0.

```
li:nth-child(3n+0){
    /*
        nth-child(an+b)
        a = cycle size
        n = counter
        b = offset value
    */

    background-image: linear-gradient(to right, yellow, white);
}
```

#### Positionning

##### Text alignment
We can use the text alignment property to place text to the left, to the center or to the right of our screen. By default, text is aligned to the left.

```
#p1{text-align: left;}

#p2{text-align: center;}

#p3{text-align: right;}
```

##### Float property
An element that uses the float property will have all other elements or text flow around it, like in a lake. It will allow elements to be side by side. You can chose the side (left or right).

```
#float-p1{
    float: left;
    width: 250px;
}
```

This means that the first paragraph will be in the left, and other paragraphs will be around it.

##### Position property
There are five different values we can place inside the position property. This property is used to position an element some place in your web page. These are the values: fixed, relative, sticky, absolute and static position.

###### fixed
This value will fix the element to the screen, no matter if the user scrolls or not. It's going to be like a water mark. In the example below, a text is being displayed at the bottom right of the screen.

```
#bottom-right{
    position: fixed;
    bottom: 0px;
    right: 0px;
}
```

###### relative
The relative value will place the element based on its normal positioning. For example, an h1 is placed at the top and on the left side, so if you give the value "relative", it will be placed relative to that position (upper corner, left side).

```
#more-or-less-center{
    position: relative;
    left: 200px;
}
```

###### sticky
An element that is sticky will stick to the viewport when you're scrolling. It is very useful for a navigation bar, for example, where you want it to always be stuck to the top, even when the user scrolls down.

```
#sticky-p{
    position: sticky;
    bottom: 0px;
}
```

###### static
Everything that is static is what it normally is by default. So if you ever need to reset the position of something, set it to static.

`#statick-p{position: static;}`

###### absolute
The absolute value makes the element's position relative to its outer container. In other words, you make the inner box independent of the outer box, because you can move it outside of the outer box if you want. You can set the position of your absolute box using the top, bottom, left and right properties.

Code example:

```
#outer-div{
    position: relative;
    border: 1px solid;
    background-color: lightgray;
    width: 200px;
    height: 200px;

    margin-left: auto;
    margin-right: auto;
}

#inner-div{
    position: absolute;
    width: 100px;
    height: 100px;
    background-color: gray;

    top: 50px;
    left: 50px;
}
```

#### Transformations
Transform is a CSS property that can be used to apply a two-dimensional or three-dimensional transformation on a base element. We can transform elements by making them rotate, move, skew them, or increase/decrease the scaling of its dimensions.

##### translate
Moves the element. The first value is the x, the second is the y.

`#p2{transform: translate(50px, 0px);}`

This will mave my #p2 move 50px to the right.

##### rotate
Makes the element rotate on its axis.
`#p2{transform: rotate(10deg);}`

You can also use `rotateY(0deg)` to make it rotate on its y axis, and `rotateX(0deg)` to make it rotate on its X axis. By default it rotates on its z axis.

##### scale
Changes the size or scaling of the element.

`#scale{transform: scale(2,1);}`

The first value represents width, and the second represents height. One is the normal amount. If you want to squish it, give a floating point value under 1.

##### skew
Skews the element. The first value represents the width, and the second, the height.

`#skew{transform: skew(10deg,10deg);}`

##### matrix
This takes six values. Here's a list with all of them:

1. scalex()
2. skewY()
3. skewX()
4. scaleY()
5. translateX()
6. translateY()

If you want your element to at least appear, scaleX and scaleY have to be greater than 0.

#### Navigation Bar
Create an unordered list, and for each item, set a link to which file you want the page to go to.

Here's how the HTML looks like:

```
<ul>
    <li><a href="">Home</a></li>
    <li><a href="">About</a></li>
    <li><a href="">Services</a></li>
    <li><a href="">Contact Us</a></li>
</ul>
```

Then, on the CSS file, write this:

```
/* Modifying the undordered list */
ul{
    list-style-type: none; /* Remove the dots before each item */
    padding: 0px; /* Bring the list to the left corner */
    margin: 0px; /* This also brings the list to the left corner */
    overflow: hidden; /* Cut the content in case it goes past the screen */
    background-color: darkgray; /* The color of the bar */
}

/* Modifying each link element (a) inside all list items (li) */
li a{
    float: left; /* Bring all links to the same line */
    display: block; /* Turn the element into a block instead of an inline element */
    padding: 10px 15px; /* Add some space between each link, bottom and top. */
    text-align: center; /* Align the text to the center */
    text-decoration: none; /* Remove the underline from the link */
    border-right: 1px solid black; /* Add a nice border to separate each word */
    min-width: 60px; /* Increase the space between each word */
    color: #e8e8e8; /* Change the color of the text */
}

li a:hover{
    background-color: gray; /* Pseudo-class that changes background color of each word when someone hovers their mouse over it*/
}
```

Doing the same bar without using unordered lists:

HTML:

```
<div id="bar">
    <a href="">Home</a><a href="">About</a><a href="">Explore</a><a href="">Login</a>
</div>
```
