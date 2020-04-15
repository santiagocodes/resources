#HTML Page Structure

<!DOCTYPE html>
<html>
    <head>
    
    </head>
    <body>
    
    </body>
</html>

## Head Tag

The head tag defines the document properties using the following tags:

* title
    <title> ... </title>
* script
    <script defer src="file.js"></script>
    With modern HMLT it is prefered to add JavaScript into the page head tag and added 'defer' rather than including it at the bottom of the body tag.
    You may also use 'async' rather than 'defer', but that is recommended for when we integrate an independent third-party script into the page, such as counters, ads and so on. More information on this can be found [here](https://javascript.info/script-async-defer).
* noscript
    <noscript> <style> .some-css {...} </style> </noscript>
    -or-
    <noscript>Sorry! Your browser does not support JavaScript!</noscript>  
    While inside the head element, it should include a link tag, style tag, or meta tag. If in the body element then this is not necessary, plus it can include paragraph tags and other. 
* link
    <link href="file1.css" rel="stylesheet">
    <link href="file2.css" rel="stylesheet" media="print">
      The media attribute can be added when loading different stylesheets depending on the device capabilities. 
    <link rel="shortcut icon" href="assets/css/images/myPic.jpeg" />
      Link tag can also be used to add a favicon (that image that shows, for example, in the tab of the webpage). 
* style
    <style> .some-css {...} </style>
    -or-
    <style media="print"> .some-css {...} </style>
    Media attribute can be used so that CSS applies only on the specified medium. This is optional
* base
    <base href="https://www.w3schools.com/" target="_blank">
    <a href="tags/tag_base.asp">HTML base Tag</a> => this will open the following page in a new tap: https://www.w3schools.com/tags/tag_base.asp
    It is usesd to specify a default URL and/or a default target for all links on a page. 
* meta
    <meta name="description" content="A nice page">
    <meta charset="utf-8">
    <meta name="robots" content="noindex">
    <meta name="robots" content="nofollow">
    <meta name="robots" content="noindex, nofollow">
      The robots meta tag instructs the Search Engine bots.
      The default behavior is index, follow. You can use other properties, including nosnippet, noarchive, noimageindex and more.
    <meta name="viewport" content="width=device-width, initial-scale=1">
    -or-
     <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/>
      This is used on a typical mobile-optimized site. 
      The width property controls the size of the viewport. There are corresponding height and device-height values as well. 
      The initial-scale property controls the zoom level when the page is first loaded. The maximum-scale, minimum-scale, and user-scalable properties control how users are allowed to zoom the page in or out.
    <meta http-equiv="refresh" content="3;url=http://flaviocopes.com/another-page">
      This tells the browser to wait 3 seconds, then redirect to that other page.
      
## Body Element

### Tags

* paragraph 
    <p>Some text</p>
    It's a block element. Inside it, we can add any inline element we like, like 'span' or 'a'.
* span
    <p>A part of the text <span>and here another part</span></p>
    It's an inline tag that can be used to create a section in a paragraph that can be later targeted using CSS.
* br
    <p>Some text<br>A new line</p>
    It's an inline element that represents a line break.
* h
    <h1> ... </h1>
    -to-
    <h6> ... </h6>
    Headings, especially the heading organization, are essential for SEO.
* strong
    <strong> ... </strong>
    This is not a visual hint, but a semantic hint. Browsers by default make the text in this tag bold.
* em
    <em> ... </em> 
    This is not a visual hint, but a semantic hint. Browsers by default make the text in this italic.
* blockquote
    <blockquote cite="http://www.worldwildlife.org/who/index.html"> ... </blockquote>
    This is a block element.
* q
    <q> ... </q>
    This is an inline element. 
* hr
    <hr>
    Adds an horizontal line. Usually used to divide sections. It has no closing tag.
* code
    <code> ... </code>
    Basically only changes the text font to monospace.
* ul
    <ul> <li>item1</li> <li>item2</li> <li>item3</li> </ul>
    Unordered list
* ol
    <ol> <li>item1</li> <li>item2</li> <li>item3</li> </ol>
    Ordered list
* dl
    <dl> <dt>name</dt> <dd>The name</dd>
        <dt>surname</dt> <dd>The surname</dd> </dl>
    Definition list
 
Other possible tags with presentational purposes: mark tag, ins tag, del tag, sup tag, sub tag, small tag, i tag, and b tag.

### Links

Links can be used to go to and absolute URL <a href="https://blabla.com" target="_blank">click here</a>
-or-
to a relative URL <a href="/test" target="_blank">click here</a>

You can include other things, beside a text, like: <a href="https://blabla.com"><img src="test.jpg"></a>

### Container Tags

* article 
    The article tag identifies a thing that can be independent from other things in a page.
* section
    Represents a section of a document. 
* div 
    A generic container element.

### Tags related to page

* nav
    <nav> <ol><li><a href="/">Home</a></li><li><a href="/blog">Blog</a></li></ol> </nav>
* aside
    <aside> <p>A quote..</p> </aside>
    used to add a piece of content that is related to the main content.
* header
    <header> <h1>Article title</h1> </header>
* main
    <main> <p>....</p> </main>
* footer
    <footer> <p>....</p> </footer>
    
### Media

<audio src="file.mp3" controls autoplay loop muted>

<video src="file.mp4" controls autoplay loop>

<video src="file.mp4" poster="picture.png">

<img src="dog.png" alt="A picture of a dog" width="300" height="200">

<figure>
    <img src="dog.png"
         alt="A nice dog">
    <figcaption>A nice dog</figcaption>
</figure>

<img src="dog.png"
    alt="A picture of a dog"
    srcset="dog-500.png 500w,
               dog-800.png 800w,
             dog-1000.png 1000w,
             dog-1400.png 1400w">

<picture>
  <source media="(min-width: 500w)" srcset="dog-500.png" sizes="100vw">
  <source media="(min-width: 800w)" srcset="dog-800.png" sizes="100vw">
  <source media="(min-width: 1000w)" srcset="dog-1000.png"    sizes="800px">
  <source media="(min-width: 1400w)" srcset="dog-1400.png"    sizes="800px">
  <img src="dog.png" alt="A dog image">
</picture>


    
    
