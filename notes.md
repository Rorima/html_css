# Notes

[Course link](https://www.youtube.com/watch?v=cyuzt1Dp8X8&ab_channel=BroCode)

Where I stopped: 29:20

These are all of the notes I took while studying the HTML5 & CSS3 course made by [Bro Code](https://www.youtube.com/@BroCodez). I have to learn this first before going further on a Django course. Keep in mind that these notes are for ME. I did not make them with someone else in mind that might use this for their learning, so there will be things in here that only I will understand.

Inside each folder there will be studying files, which are files that I wrote following the teacher, and practice files, which are files that I wrote after I studied, trying to apply what I've learned. Most of the time, in practice files, I just try to repeat what I learned, but without looking at the original code.

#### What is HTML?
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

