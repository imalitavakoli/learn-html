# Learn HTML in simple terms
Decided to be a web designer or frontend developer today? You came to the right place.
**Here we're gonna learn HTML, simple and fast!**

You won't see me talk too much, but see codes a lot! And the only way to learn a coding language, is to get your hands dirty with it, **open up a text editor, and just start typing**! That's exactly what we're going to do. **If you don't understand everything at this moment** (e.g., why to write this or that symbol), **don't worry**! Simply watch my sample codes and then try to write the exact (or similar) codes yourself! Just do it! Right now, you don't have to know every little detail... You like to learn fast (and maybe earn some money as a web designer or frontend developer), right? So don't worry about theoretical stuff or history mystery at this stage! There's always time to study and learn such stuff... So here, we're just going to focus on the main stuff and aim to learn HTML a.s.a.p :rocket:




# For whom this tutorial is?
For anyone who is eager enough! But before coding, you need to setup your comfortable environment! Choose a text editor, learn some of its tips & tricks, and maybe install some CLI tools!

So please first take a look at the following **prerequisites for this tutorial**:
- ["Learn setting up a simple Frontend environment for beginners" tutorial](https://github.com/imalitavakoli/learn-frontend-env-setup) (9 min read)

So you're ready? Let's do it :thumbsup:




# Sample files?
Any sample codes that I write here in this tutorial, can be found in the "*Samples*" directory of the GitHub repository of the tutorial. [Click here](https://github.com/imalitavakoli/learn-html/archive/refs/heads/main.zip) to download them all.

**NOTE:** To learn coding and gain confidence, please do not just look at the samples! open up a text editor, write some similar codes yourself, save your files, and open them via a web browser to check out your results! This is the only way to be a coder!

**NOTE:** The sample HTML documents here, don't look so beautiful when you open them via a web browser? Well, that's because they are pure HTML! Your document don't look beautiful until you style it by CSS! So yes, CSS is the next thing that you have to learn later, after you have learnt the HTML basics.




# Table of contents to learn
- [What is HTML?](#what-is-html)
- [Basics](#basics)
- [Forms](#forms)
- [Lists](#lists)
- [Tables](#tables)




## What is HTML?
HTML stands for "*Hyper Text Markup Language*". It is **the standard markup language for creating Web pages**. It consists of a series of elements. Elements tell the browser how to display the content.

Imagine a human body... **HTML is the skeleton**! It sets up a webpage's structure, and makes internet webpages possible!


### How to produce an HTML file?
1. You **write HTML in a text editor** and save it with the extension of *.html* and *UTF-8* encoding. (e.g., index.html)
2. **Open it via a web browser**, such as Chrome, Edge, Firefox, Safari. (The purpose of a web browser is to read your HTML codes and render the results)
3. And you will see the results. **That's it**! Didn't imagine as simple as that producing a webpage can be? Well, it's just that simple :smile:

**NOTE:** In order to inspect currently-loaded HTML, CSS and JavaScript codes, or see which assets the page has requested and how long they took to load, and more... You can open your browser's developer tools! What are browser developer tools? Every modern web browser includes a powerful suite of developer tools that help you as the developer to code better, faster, and more efficiently in every aspect. You can find the devtools in most of the browsers under the browser's Menu bar > More tools > Developer tools. [Click here](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools) to learn more about the browser developer tools.


### A simple HTML document?
Here I wrote a simple HTML document.

**NOTE:** In my sample codes, I try to quickly explain some definitions by placing comments among the codes.

**NOTE:** What is a comment? You can write comments among your codes to explain your code, which can help you when you edit the source code at a later date. The comment tag is used to insert comments in HTML. Anything between the comment start tag `<!--` and comment end tag `-->` is not displayed in the browsers. e.g., `<!-- This is a comment -->`

```html
<!-- 01_simple.html -->

<!DOCTYPE html>               <!-- Defines that this document is an HTML5 document. HTML5 is the latest version of HTML. -->
<html>                        <!-- The root element of an HTML page. -->
  <head>                      <!-- Contains meta information about the HTML page. -->
    <title>Page Title</title> <!-- Specifies a title for the HTML page. (It is shown in the browser's title bar) -->
  </head>
  <body>                      <!-- Defines the document's body, and is a container for all the visible contents. -->
    <h1>First Heading</h1>    <!-- The <h1> to <h6> tags are used to define HTML headings. -->
    <p>First paragraph.</p>   <!-- Defines a paragraph. -->
  </body>
</html>
```


### What is an HTML Element?
An HTML element is defined by a start tag, some content, and an end tag:  
`<tagname> Content goes here... </tagname>`  
`<h1>First Heading</h1>`  
`<p>First paragraph.</p>`


### HTML Attributes?
HTML attributes provide additional information about HTML elements. All HTML elements can have attributes. Attributes are always specified in the start tag. Attributes usually come in name/value pairs like:  
`name="value"`  
`<img src="img.jpg" width="500" height="600">`




## Basics
A very simple HTML document, can look like this. As you can see in my sample code below, it's a good practice to also mention the language of the document `lang="en"` and the character encoding `charset="utf-8"`.

```html
<!-- 02_basics-01.html -->

<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>My Webpage</title>
  </head>
  <body>
    Content of my webpage is here...
  </body>
</html>
```


In sample below, I show you some of the most useful elements (such as header, section, etc.), and some other ones that I used to wrap this sample document up (such as blockquote, mark, etc.)

```html
<!-- 03_basics-02.html -->

<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>03</title>
  </head>
  <body>

    <!-- Defines a header for the document or a section. -->
    <header>
      HEADER
    </header>

    <!-- Defines content aside from the page content. -->
    <aside>
      I'm a sidebar! But you won't see me like that just yet! Because I need to be styled by CSS :)
    </aside>

    <!--
    Defines a section in the document. Section contains a content that is 
    related to the rest of the page most of the times.
    
    id attribute? It specifies a unique id for an HTML element. The value of the 
    id attribute must be unique within the HTML document. It can be used by CSS 
    (to point to a specific style declaration) or JavaScript (to access and 
    manipulate the element).
    -->
    <section id="mainSection">
      <!--
      The <blockquote> tag specifies a section that is quoted from another source.
      The <q> tag defines a short quotation.
      The <mark> tag defines text that should be marked or highlighted.
      The <cite> tag defines the title of a creative work (e.g. a book, a poem, a song, etc.).
      -->
      <blockquote>
        <q>That's it, I'm learning <mark>HTML</mark>!</q>
        <footer><a href="#" rel="author">Ali Tavakoli</a> - <cite>The Author of Cool tutorials</cite></footer>
      </blockquote>
    </section>

    <!--
    Defines an article in the document. Article contains a content that is 
    independent to the rest of the page most of the times.
    -->
    <article>
      <h1>
        <!--
        The <time> tag defines a specific time (or datetime).
        
        datetime attribute? It is used to translate the time into a 
        machine-readable format.

        pubdate attribute? Indicates that the date/time in the <time> element is
        the publication date of the document.
        -->
        My article, posted on <time datetime="2022-10-13T22:19:00-03:30" pubdate>Oct 13th, 2022 at 10:19 PM</time>
      </h1>
      <p>
        And here is my content.
      </p>
      <!--
      The <img> tag is used to embed an image.

      alt attribute? Specifies an alternate text for an image.
      -->
      <img src="hero.jpg" alt="Hero Image" width="512">
    </article>

    <section>
      <p>
        <!--
        The <a> tag defines a hyperlink, which is used to link from one page to another.
        
        href attribute? It's the most important attribute of the <a> element, 
        which indicates the link's destination.
        -->
        This the first <a href="#" title="first link" rel="start">hyperlink</a> in my page.
        go to <a href="https://github.com.com/" rel="external">github.com</a>
      </p>
    </section>

    <!-- Defines a footer for the document or a section. -->
    <footer>
      <p>
        Copyright 2022 - All rights reserved. <a href="#" rel="license">view Terms</a>.
      </p>
    </footer>

    <!--
    Defines a division or a section in an HTML document.

    Any sort of content can be put inside the <div> tag!  It is a general tag 
    that basically can be the container of any sort of content.

    So some other block-level elements such as header, section, article, and 
    footer can be replaced by a div element! (Block-level elements always start 
    on a new line, and the browsers automatically add some space before and 
    after them. A block-level element always takes up the full width available. 
    It stretches out to the left and right as far as it can)
    -->
    <div>
      Some other content here...
    </div>

  </body>
</html>
```


In sample below, I introduce you some more tags and some tips.

```html
<!-- 04_basics-03.html -->

<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">

    <!-- Some more meta tags -->
    <meta name="description" content="A description about your webpage for SEO">
    <meta name="keywords" content="HTML, HTML5, learning, tutorial">
    <meta name="author" content="Ali Tavakoli">

    <title>04</title>
  </head>
  <body>

    <h1 id="anchor">Anchor</h1>
    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.  
    <!--
    By using <a> tags, we can also link to different elements on the same page.
    If we would have a long article in our webpage, that's a perfect way to 
    reference to some main titles.
    -->
    <a href="#anchor">Click here to go to the "Anchor" heading</a>

    <!--
    Defines a thematic break. It is most often displayed as a horizontal rule 
    that is used to separate content. <hr> tag don't need to be closed.
    -->
    <hr>

    <!--
    The <iframe> tag specifies an inline frame. An inline frame is used to embed 
    another document within the current HTML document.
    -->
    <iframe src="02_basics-01.html" name="frame" frameborder="0" width="100%" height="100"></iframe>
    <a href="03_basics-02.html" target="frame">Click here</a> to open 03_basics-02.html in the inline frame above.

    <hr>

    <code>my code</code>
    <kbd>my keyboard input</kbd>
    <var>my variable</var>
    <pre>my preformatted text</pre>
    <samp>my sample output</samp>

    When I'd like to <mark>mark</mark> a text!
    When I love <del>delete a text</del> and <ins>insert another one</ins>.

    <hr>

    <!--
    The <br> tag inserts a single line break. It is useful for writing addresses 
    or poems. It is an empty tag which means that it has no end tag.
    -->
    <p>To force<br> line breaks<br> in a text,<br> use the br<br> element.</p>

    <hr>

    <!--
    Some characters are reserved in HTML.

    If you use the less than (<) or greater than (>) signs in your text, the 
    browser might mix them with tags.
    
    Character entities are used to display reserved characters in HTML.  
    A character entity looks like this: &entityName; OR &#entityNumber;
    -->
    Non-breaking Space: before spaces &nbsp;&nbsp;&nbsp; after speces...<br>
    copyRight: &copy;<br>
    trademark: &trade;<br>
    registered trademark: &reg;

  </body>
</html>
```




## Forms
Here I introduce some form related elements.

```html
<!-- 05_forms.html -->

<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>05</title>
  </head>
  <body>

    <!--
    The <form> tag is used to create an HTML form for user input.

    It can contain one or more of the following form elements: <input> 
    <textarea> <button> <select> <option> <optgroup> <fieldset> <label> <output>
    
    name attribute? Specifies the name of a form.

    action attribute? Specifies where to send the form-data when a form is 
    submitted. (it can be a URL to a PHP file so that the submitted data of the 
    form can be handled by a server-side coding language)

    method attribute? Specifies the HTTP method to use when sending form-data. 
    (it can be 'get' or 'post')  
    -->
    <form name="myform" action="#" method="get">
      <!--
      The <label> tag defines a label for <input> elements and some other form 
      related elements.

      <label> is useful for screen reader users. It's also helpful when users 
      like to toggle the label related element easily by clicking the label text 
      itself! Because sometimes the element itself is small (such as checkbox 
      input elements)

      for attribute? Specifies the id of the form element the label should be 
      bound to.
      -->
      <label for="fname">First Name</label>
      <!--
      The <input> tag specifies an input field where the user can enter data.
      The <input> element can be displayed in several ways, depending on the type attribute.

      The most used input types are the following: text, email, tel, password, 
      file, checkbox, radio, button, submit, reset.
      -->
      <input type="text" name="firstname" id="fname">

      <label for="lname">Last Name</label>
      <input type="text" name="lastname" id="lname">

      <label for="age">Age</label>
      <input type="number" name="age" id="age" step="1" min="18">

      <label for="pic">Profile Photo</label>
      <input type="file" name="profilephoto" id="pic">

      <input type="submit" value="Submit">
      <input type="reset" value="Clean">
    </form>

    <form action="#" method="post">
      Email <input type="email" name="email">
      pass <input type="password" name="pass">
      <br>
      Remember me <input type="checkbox" name="remember" value="remember">
      <br>
      <input type="submit" value="Sign in">
    </form>

    <strong>Sex:</strong>
    Male <input type="radio" name="sex" value="male">
    Female <input type="radio" name="sex" value="female">

    <strong>Vehicle:</strong>
    Car <input type="checkbox" name="vehicle" value="car">
    Bicycle <input type="checkbox" name="vehicle" value="bicycle">

    <form>
      <!-- The <fieldset> tag is used to group related elements in a form. -->
      <fieldset>
        <!-- The <legend> tag defines a caption for the <fieldset> element. -->
        <legend>Country</legend>
        <select name="country">
          <option value="USA">USA</option>
          <option value="UK" selected>UK</option>
          <option value="UAE">UAE</option>
        </select>
      </fieldset>

      <fieldset>
        <legend>Message</legend>
        <textarea rows="3" cols="20">The default value</textarea>
        <br>
        <input type="button" value="sample button">
      </fieldset>

      <fieldset>
        <legend>Electronic</legend>
        <select name="electronic">
          <optgroup label="computer">
            <option value="mouse">Mouse</option>
            <option value="keboard">Keyboard</option>
          </optgroup>
          <optgroup label="devices">
            <option value="tablet" selected>Tablet</option>
            <option value="mobile">Mobile</option>
          </optgroup>
        </select>
      </fieldset>
    </form>

  </body>
</html>
```




## Lists
Here I introduce some list related elements.

```html
<!-- 06_lists.html -->

<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>06</title>
  </head>
  <body>

    <!-- The <ul> tag defines an unordered (bulleted) list. -->
    <ul>
      <!--
      The <li> tag defines a list item.
      It is used inside ordered lists(<ol>) and unordered lists (<ul>).
      -->
      <li>List Item 01</li>
      <li>List Item 02</li>
    </ul>

    <!--
    The <ol> tag defines an ordered list. An ordered list can be numerical or alphabetical.

    type attribute? Specifies the kind of marker to use in the list. Its value 
    can be one of the following: 1, A, a, I, i

    start attribute? Specifies the start value of an ordered list.
    -->
    <ol type="i" start="1">
      <li>List Item 01</li>
      <li>List Item 02</li>
    </ol>

    <!--
    The <dl> tag defines a description list.
    It is used in conjunction with <dt> (defines terms/names) and <dd> (describes each term/name).
    -->
    <dl>
      <dt>title 01:</dt>
      <dd>Description 01.</dd>
      <dt>title 02:</dt>
      <dd>Description 02.</dd>
    </dl>

  </body>
</html>
```




## Tables
Here I introduce some table related elements.

```html
<!-- 07_tables.html -->

<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>07</title>
  </head>
  <body>

    <!--
    The <table> tag defines an HTML table.

    It consists one or more <tr>, <th>, and <td> elements, and maybe some more 
    elements such as <thead>, <tfoot>, and <tbody>.
    -->
    <table border="1">
      <caption>Table caption</caption>
      <tr id="table_header">            <!-- The <tr> tag defines a row. -->
        <th>01 header</th>              <!-- The <th> tag defines a header cell. -->
        <th>02 header</th>
        <th>03 header</th>
      </tr>
      <tr id="table_body">
        <td>01 column</td>              <!-- The <td> tag defines a standard data cell. -->
        <td>02 column</td>
        <td>03 column</td>
      </tr>
    </table>

    <table border="1">
      <caption>Table caption</caption>
      <tr>
        <th>01 header</th>
        <td>01 column</td>
      </tr>
      <tr>
      	<th>02 header</th>
        <td>02 column</td>
      </tr>
    </table>

    <table border="2">
      <caption>cell that spans three columns</caption>
      <tr>
      	<th>header 01</th>
        <th colspan="3">header 02</th>  <!-- colspan attribute? Defines the number of columns a cell should span. -->
      </tr>
      <tr>
      	<td>data 01</td>
        <td>data 02</td>
        <td>data 03</td>
        <td>data 04</td>
      </tr>
    </table>

    <table border="2">
      <caption>cell that spans three rows</caption>
      <tr>
        <th>header 01</th>
        <td>data 01</td>
      </tr>
      <tr>
        <th rowspan="3">header 02</th>  <!-- rowspan attribute? Defines the number of rows a cell should span. -->
        <td>data 02</td>
      </tr>
      <tr>
      	<td>data 03</td>
      </tr>
      <tr>
      	<td>data 04</td>
      </tr>
    </table>

    <!--
    The <thead> tag is used to group header content.
    The <tbody> tag is used to group body content.
    The <tfoot> tag is used to group footer content.

    Browsers can use these elements to enable scrolling of the table body 
    independently of the header and footer.
    -->
    <table border="1">
      <thead>
      	<tr>
          <th>Name</th>
          <th>Price</th>
        </tr>
      </thead>
      <tbody>
      	<tr>
          <td>Item 01</td>
          <td>$xxx</td>
        </tr>
        <tr>
          <td>Item 02</td>
          <td>$xxx</td>
        </tr>
      </tbody>
      <tfoot>
      	<tr>
          <td colspan="2">Price table</td>
        </tr>
      </tfoot>
    </table>

  </body>
</html>
```




# What's next?
In this tutorial we learnt what is HTML, where to write it, how to write it, and how to see its results. We also talked about what a very simple HTML document consists of, what are HTML Elements and attributes. And then we started to learn some of the most frequently used HTML elements and attributes to create different stuff such as sections, articles, forms, lists, and tables.

If you practiced with my sample codes along the way, you may be wondering now: I have learned the HTML basics, but why I still cannot create a reasonable or at least a little bit graphical webpage?! Well, I answered to this question of yours, right at the beginning of the tutorial:
> Your document don't look beautiful until you style it by CSS!

So don't worry if you still cannot give birth to a beautiful webpage! **You still need to learn and practice more**. Your next step to become a web designer or frontend developer is to also learn CSS. And CSS tutorial, is what I'm going to provide next :smile:

But before we go to learn CSS... Do you like to level up your HTML learnings? If so, you can checkout the following resources:

* [W3schools HTML Tutorial](https://www.w3schools.com/html/default.asp)
