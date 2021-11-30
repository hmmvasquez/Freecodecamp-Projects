# HTML Basico y HTML5

#### HTML 
Is a markup language that uses a special syntax or notation to describe the structure of a webpage to the browser. 

## Say Hello to HTML Elements
Most HTML elements have an opening tag and a closing tag.

`<h1>Hello World</h1>`

## Headline with the h2 element
This element tells your website about the structure of your website. h1 elements are often used for main headings, while h2 elements are generally used for subheadings. There are also h3, h4, h5 and h6 elements to indicate different levels of subheadings.
```
 <h1>Hello World</h1>
 <h2>CatphotoApp</h2>
```
## Inform with the paragraph element
p elements are the preferred element for paragraph text on websites.

*As a convention, all HTML tags are written in lowercase.*

`<p>I'm a p tag!</p>`
```
 <h1>Hello World</h1>
 <h2>CatphotoApp</h2>
 <p>Hello Paragraph</p>
```
## Fill in the black with placeholder text
Web developers traditionally use *lorem ipsum text* as placeholder text. 
```
 <h1>Hello World</h1>
 <h2>CatphotoApp</h2>
 <p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
```
## Uncomment HTML
Commenting is a way that you can leave comments for other developers within your code without affecting the resulting output that is display to the end user.

Comments in HTML
`<!-- -->`

## Comment out HTML
Remember that in order to start a comment, you need to use <!-- and to end a comment, you need to use -->
```
<!--
<h1>Hello World</h1>
-->
<h2>CatPhotoApp</h2>
<!--
<p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
-->
```

## Introduction to HTML5 elements
HTML5 introduces more descriptive HTML tags. These includes main, header, footer, nav, video, article, section and others.

These tags give a descriptive strucuture to your HTML, make your HTML easier to read, and help with Search Engine Optimization (SEO) and accessibility.
```
<h2>CatPhotoApp</h2>
<main>
<p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
<p>Purr jump eat the grass rip the couch scratched sunbathe, shed everywhere rip the couch sleep in the sink fluffy fur catnip scratched.</p>
</main>
```
## Add images to your website
You can add images to your website by using the img element, and point to a specific image's URL using the src attribute.

`<img src="https://www.freecatphotoapp.com/your-image.jpg">`

note that img elements are self-closing.

All img elements must have an alt attribute. The text inside an alt attribute is used for screen readers to improve accessibility and is displayed if the image fails to load.

## Link to external pages with anchor elements
You can use a (anchor) elements to link to content outside of your web page.

a elements need a destination web address called an href attribute. They also need anchor text. Here's an example:

`<a href="https://www.freecodecamp.org">this links to freecodecamp.org</a>`

## Link to Internal Sections of a Page with Anchor ElementsPassed
a (anchor) elements can also be used to create internal links to jump to different sections within a webpage.

To create an internal link, you assign a link's href attribute to a hash symbol # plus the value of the id attribute for the element that you want to internally link to, usually further down the page. You then need to add the same id attribute to the element you are linking to. An id is an attribute that uniquely describes an element.

Below is an example of an internal anchor link and its target element:

``` 
<a href="#contacts-header">Contacts</a>
...
<h2 id="contacts-header">Contacts</h2>
```

## Nest an Anchor Element within a Paragraph
You can nest links within other text elements.
```
<p>
  Here's a <a target="_blank" href="https://www.freecodecamp.org"> link to www.freecodecamp.org</a> for you to follow.
</p>
```
target is an anchor tag attribute that specifies where to open the link. The value _blank specifies to open the link in a new tab. The href is an anchor tag attribute that contains the URL address of the link:

`<a href="https://www.freecodecamp.org" target="_blank"> ... </a>`

## Make Dead Links Using the Hash SymbolPassed
Sometimes you want to add a elements to your website before you know where they will link.

This is also handy when you're changing the behavior of a link using JavaScript, which we'll learn about later.

`href="#"`

## Turn an Image into a Link
You can make elements into links by nesting them within an a element.

Nest your image within an a element. Here's an example:

`<a href="#"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="Three kittens running towards the camera."></a>`

## Create a Bulleted Unordered List
HTML has a special element for creating unordered lists, or bullet point style lists.

Unordered lists start with an opening `<ul>` element, followed by any number of `<li>` elements. Finally, unordered lists close with a `</ul>`.

For example:

```
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```
## Create an Ordered ListPassed
HTML has another special element for creating ordered lists, or numbered lists.

Ordered lists start with an opening `<ol>` element, followed by any number of `<li>` elements. Finally, ordered lists are closed with the `</ol>` tag.

For example:
```
<ol>
  <li>Garfield</li>
  <li>Sylvester</li>
</ol>
```
## Create a Text Field
Now let's create a web form.

input elements are a convenient way to get input from your user.

You can create a text input like this:

`<input type="text">`

## Add Placeholder Text to a Text FieldPassed
Placeholder text is what is displayed in your input element before your user has inputted anything.

You can create placeholder text like so:

`<input type="text" placeholder="this is placeholder text">`

## Create a Form Element
You can build web forms that actually submit data to a server using nothing more than pure HTML. You can do this by specifying an action attribute on your form element.

For example:
```
<form action="/url-where-you-want-to-submit-form-data">
  <input>
</form>
```
## Add a Submit Button to a Form
Let's add a submit button to your form. Clicking this button will send the data from your form to the URL you specified with your form's action attribute.

Here's an example submit button:

`<button type="submit">this button submits the form</button>`

## Use HTML5 to Require a Field
You can require specific form fields so that your user will not be able to submit your form until he or she has filled them out.

For example, if you wanted to make a text input field required, you can just add the attribute required within your input element, like this: 

`<input type="text" required>`

## Create a Set of Radio Buttons
You can use radio buttons for questions where you want the user to only give you one answer out of multiple options.

Radio buttons are a type of input.

Each of your radio buttons can be nested within its own label element. By wrapping an input element inside of a label element it will automatically associate the radio button input with the label element surrounding it.

All related radio buttons should have the same name attribute to create a radio button group. By creating a radio group, selecting any single radio button will automatically deselect the other buttons within the same group ensuring only one answer is provided by the user.

Here's an example of a radio button:

```
<label> 
  <input type="radio" name="indoor-outdoor">Indoo 
</label>
```
## Create a Set of Checkboxes
Forms commonly use checkboxes for questions that may have more than one answer.

Checkboxes are a type of input.

Each of your checkboxes can be nested within its own label element. By wrapping an input element inside of a label element it will automatically associate the checkbox input with the label element surrounding it.

All related checkbox inputs should have the same name attribute.

It is considered best practice to explicitly define the relationship between a checkbox input and its corresponding label by setting the for attribute on the label element to match the id attribute of the associated input element.

Here's an example of a checkbox:

`<label for="loving"><input id="loving" type="checkbox" name="personality"> Loving</label>`

## Use the value attribute with Radio Buttons and Checkboxes
When a form gets submitted, the data is sent to the server and includes entries for the options selected. Inputs of type radio and checkbox report their values from the value attribute.

For example:

```
<label for="indoor">
  <input id="indoor" value="indoor" type="radio" name="indoor-outdoor">Indoor
</label>
<label for="outdoor">
  <input id="outdoor" value="outdoor" type="radio" name="indoor-outdoor">Outdoor
</label>
```
## Check Radio Buttons and Checkboxes by Default
You can set a checkbox or radio button to be checked by default using the checked attribute.

To do this, just add the word checked to the inside of an input element. For example:

`<input type="radio" name="test-name" checked>`

## Nest Many Elements within a Single div Element
The div element, also known as a division element, is a general purpose container for other elements.

The div element is probably the most commonly used HTML element of all.

Just like any other non-self-closing element, you can open a div element with `<div>` and close it on another line with `</div>`.

## Declare the Doctype of an HTML Document
At the top of your document, you need to tell the browser which version of HTML your page is using. HTML is an evolving language, and is updated regularly. Most major browsers support the latest specification, which is HTML5. However, older web pages may use previous versions of the language.

You tell the browser this information by adding the `<!DOCTYPE ...>` tag on the first line, where the ... part is the version of HTML. For HTML5, you use `<!DOCTYPE html>`.

The ! and uppercase DOCTYPE is important, especially for older browsers. The html is not case sensitive.

Next, the rest of your HTML code needs to be wrapped in html tags. The opening `<html>` goes directly below the `<!DOCTYPE html>` line, and the closing `</html>` goes at the end of the page.

Here's an example of the page structure. Your HTML code would go in the space between the two html tags.

```
<!DOCTYPE html>
<html>

</html>
```

## Define the head and body of an HTML Document
You can add another level of organization in your HTML document within the html tags with the head and body elements. Any markup with information about your page would go into the head tag. Then any markup with the content of the page (what displays for a user) would go into the body tag.

Metadata elements, such as link, meta, title, and style, typically go inside the head element.

Here's an example of a page's layout:
```
<!DOCTYPE html>
<html>
  <head>
    <meta />
  </head>
  <body>
    <div>
    </div>
  </body>
</html>
```