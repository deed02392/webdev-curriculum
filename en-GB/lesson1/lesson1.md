---
title: The Web
level: Lesson 1
language: en-GB
embeds: "*.png"
materials: "code and images"
stylesheet: web
...

# Introduction { .intro}

Today we are learning what HTML is and how tags can be used to create simple web pages.

# Classwork: Let's Recap { .activity}

## HTML
Websites are written using __HTML__, which stands for __HyperText Mark-up Language__.

HTML is a __mark-up__ language - it means that it is used to describe what things are. 

The description is used by a web browser, to tell it how best to display things.

The things we use to make up these descriptions in HTML are called `tags`. 

## Tags

Tags look like this:
- `<p>This is some text.</p>`
- `<p>` is short for __paragraph__.

There is an opening tag, `<p>` and a matching closing one with a forward slash (`/`): `</p>`

The browser knows that anything inbetween the two tags is a paragraph of text.

We saw the `<h1>` and `<img>` tags being used on the board:

- `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>` - headings, from biggest to smallest
- `<img>` - a special element, which unlike others doesn't have a closing tag. We use it for putting the images in.

## Attributes

As we saw on the board, the `<img>` tag had an attribute, which was the web address of the school's logo. Other tags have attributes too. A popular tag with an attribute is the __anchor__ tag. You almost never see it without an attribute.

Let's have a look at the __anchor__ tag:
```HTML
<a href="http://codeclub.org.uk">Visit CodeClub website</a>
```
`<a>` stands for __anchor__, which is what links used to be called, because once upon a time they would only be used to jump you around one big page - to different __anchor points__ on the page.

The __anchor__ tag has the opening tag `<a>` and the closing tag `</a>`, but we added an attribute to the opening tag:
```HTML
<a href="http://codeclub.org.uk">
```
This is the bit that decides where on the Internet clicking on the anchor text will take us.

We never add attributes to the closing tag.

`href` is the attribute __name__, and `http://codeclub.org.uk` is its __value__.

So attributes always look like `name="value"`.

`href` stands for __hyper-text reference__. A text that linked to other texts was once named __hyper-text__, because it could have images, and sounds, and could link to other texts. That made it a little bit different to plain text.
`href` tells the browser where the link should take you, and the text in between the tags is the text that will be visible as a link, often blue and underlined.

There are lots and lots of tags. Here are some more common ones:

- `<ol>` - ordered list, when you want to have a list that goes in order by number
- `<ul>` - unordered list, when you just want to list some things with bullet points and the order doesn't matter
- `<li>` - list item, this tag goes inside a list tag and contains the text of the item you want to add
- `<hr>` - horizontal rule (puts a line across the web page like you might do with a pencil in your workbooks)
- `<div>` - a special box that you can't see, but the web browser uses keeping things grouped together

There are some tags that we will _always_ use in HTML documents. They are:
- `<html>` - tells the browser where we put our code
- `<head>` - inside `<head>` we put more tags, which may be useful to the browser. No text inside the `<head>` will appear on the page. In this example we put a `<title>` there, which then shows up in the window bar or tab.
- `<body>` - this is where we put the things we want to appear on the page. Notice we've got `head` and `body`. Sometimes people add a footer to their web pages. This can go in a `<footer>` tag, but because you want it to appear on the page it must still go inside the `<body>` tag.

## Activity Checklist { .check}

1. Open up a web browser and go to `http://goo.gl/fHTu4U`.
2. Have a look around the page. On the left you can see the HTML that makes up the web page on the right. Can you recognise all the tags listed above?
3. Are there any new tags on this page? See if you can figure out what the different tag names stand for.


	| Tag           | What does it do?                                      |
	| ------------- | ----------------------------------------------------- |
	| _____________ |  ____________________________________________________ | # doctype
	| _____________ |  ____________________________________________________ | # strong
	| _____________ |  ____________________________________________________ | # em
	| _____________ |  ____________________________________________________ | # u
	| _____________ |  ____________________________________________________ | # code
	| _____________ |  ____________________________________________________ | # <!-- -->
	| _____________ |  ____________________________________________________ | # spare in case they re-identify one

4. What about attributes? Which other tags can you spot using attributes and what do they do? 

	| Tag & Attribute   | What does it do?                                      |
	| ----------------- | ----------------------------------------------------- |
	| _________________ | _____________________________________________________ | # <p class>
	| _________________ | _____________________________________________________ | # <div id>
	| _________________ | _____________________________________________________ | # <img width>
	| _________________ | _____________________________________________________ | # <img height>
	| _________________ | _____________________________________________________ | # <img alt>

## Extension Activity Checklist { .check}

+ How many __nested__ tags did you spot? We have the `<a>` tag, which is inside a `<p>` tag, which in turn is inside `<div>`, which is placed inside `<body>`.

Whenever this happens, we say that the tag that is being wrapped is the __child__ and the tag that does the wrapping is the __parent__ element. It's just like a family tree!

+ Normally the browser treats all tags the same. If you want to mark them out you can use `classes` and `ID`s.
For example, some of your paragraphs might be introductions, so you could give them a class `introduction`. See if you can spot some classes inside the example web page.

+ IDs are used to mark unique items on your page. See if you can spot the `div` tag with an `id` attribute of `kitten` in the page. Now that you've told the browser where this tag is, you could make just the text in that tag look different, even if there are other `div` tags on the page.

+ What will happen if you move things around? Let's go back to the code editor. Find an `<ol>` tag in the code and select it with all its got inside, like so:

```HTML
<ol>
	<li>Kittens</li>
	<li>Cake</li>
	<li>Lie-ins</li>
	<li>Playing games</li>
</ol>
```

Now copy it and move it somewhere else. Watch how the output on the right changes. How does the order of the code affect the order in which things are displayed in the browser? What about the individual `<li>` tags in this ordered list?

# Homework: HTML at home { .activity}

## Activity Checklist { .check}

1. Open a __text editor__. 
2. Create a new document. 
3. Write something! For example:
`Hello! My name is …`
4. Save the file. Call it `hello.txt`.
5. Now find the file and open it again. It opens up in a text editor, which is not that much fun.
6. Change the extension (the bit after the dot) to `.html`, so now the file is called `hello.html`. (If you can't see the .txt extension, put https://support.microsoft.com/kb/865219 in your browser. It will explain how to show file name extensions, so you can change them). 
7. Open the file again.

What program was used to open the file this time? The web browser is a special program that knows how to interpret text files written using __HTML language__. We haven't added any __HTML__ yet, we simply put in some text, but the browser doesn't care! As long as you give it an `.html` file, it will do its best to show you the file as best as it can understand it. 

This is very useful: even when a website contains errors, the browser will try to figure out how to show it to you anyway. 

#### Have you got developer tools?
If you use a recent Internet Exlporer, or Google Chrome, you can bring up a developer box.
1. Move around the page. Right click anything interesting, and then click `Inspect element`. A panel will open up which will show you any web pages code!
2. Move your mouse over different pieces of code. The part of the page that the code represents will light up, so you can see what code does what.
3. There will be lots of new tags to you on complex websites. Can you figure out what the different tag names stand for?
4. What happens when you try things like changing `class=""` attributes? Don't worry about messing the page up, just refresh and everything will reset.

## Things to try { .try}

* Create your own paragraph of text.
* Make a link that points to another part of page (hint: it is something to do with the ID attribute - look out for the link that takes you to the kitten in the page we used in class).
* Add your own headings where you think they might be useful. What happens if you change the heading numbers, for example from `<h3>` to `<h4>`?
* What would you have to do to link to a different page?
* If you are using developer tools, once you bring up the panel with the code try double-clicking on the code that looks interesting. See if you can change it. Now you get a live preview without having to move between the browser and the code editor.
* Now refresh the page. What happened? When you edit code like this it doesn't get saved, so you can preview what would happen without messing up your file. Experiment with your changes like this before updating your `.html` file.

## How do websites work on the Internet?
 
When you type in the address in your browser, your request gets passed along to a computer which is always turned on and configured to allow you to see the pages that live inside it. This computer is called a server. When it receives a request from your computer, it looks for all the necessary files, then creates the `.html` file before sending it to you, with anything else that the page needs, like images and videos.

![screenshot](diagram_screenshot.png)
