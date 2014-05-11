---
title: Your Own Website
level: Lesson 2
language: en-GB
embeds: "*.png"
materials: "code and images"
stylesheet: web
...

## Introduction { .intro}

You know a few __HTML__ tags, so it's time to make your first web page!

# Classwork: Our First Webpage { .activity}

## Text Editor

A text editor is a program that lets you write, edit and save simple files containing text.

Text is just a fancy computer term for letters and words.

All computers have text editors, such as Notepad in Windows.

We're going to use `Notepad++` which is a bit better for writing HTML than basic Notepad, because it recognises HTML and uses colours that help you avoid mistakes.

## File Extensions

A file extension is what helps a computer understand what is within a file. It's called a file extension because it is the bit after the file name, i.e. extending the name of a file after the bit us humans are interested in.

We separate the file name from the extension with a dot (`.`).

Some examples of file names with an extension are:

- `homework.doc` - the file name is `homework` and the extension is `.doc` which is short for Document and tells the computer to open it in Microsoft Word or similar.
- `hello.txt` - the file name is `hello` and the extension is `.txt` which means Text. It could be opened in Word, but the computer will usually just open it in the simplest program that will understand it, for example Notepad.
- `homepage.html` - the file name is `homepage` and the extension is `.html` which you should recognise by now! The computer will open it in the program that makes most sense for a web page, which is a web browser. But you could ask it to open it in a text editor like `Notepad++` because you want to edit it, not look at it. You're a coder now!
- `homepage.htm` - sometimes there's more than one extension for the same thing. Most computers treat `.htm` the same as `.html`. Once upon a time you were only allowed three letters for a file extension and this is what `.html` got shortened to. You can use whichever you prefer.

Because all files really look the same to a computer - just lots of text - we use file extensions to hint what program we'd like to open things in. You can open _any_ file in Notepad if you like, but you might find it silly what you see!

## Activity Checklist { .check}

1. Open the `Notepad++` text editor. 
2. Click the __Open__ icon in `Notepad++` and find the `about_me.html` file, then open it. It contains only a little bit of HTML code to get you started.
3. Go to the `about_me.html` file and double-click it to open `Internet Explorer`, too. Each time you make a change in `Notepad++`, click save, then refresh `Internet Explorer` (by pressing F5 on the keyboard, or clicking the recycle icon in the address bar) to see your changes.
4. Keep going until you're happy with your web page! Add pictures of your hobbies and interests using the tags you learned in Lesson 1 and the rules on directory structure you learned today.

## Mistakes

Mistakes often happen. It's very easy to make them in HTML/coding because you have to spell everything perfectly. Even a single miss-press of the keyboard can cause the page to look totally different to what you expected! Recognising common mistakes will help you find and fix them quicker.

### Missing Closing Tags
One of the most common mistakes is forgetting the __closing tag__, so let's remove the `</ul>` to see how it affects the page. Save the file and refresh it in the browser.

What happened? Some things below the list moved a little bit to the right. Because we removed the closing tag the browser simply doesn't know the list of items has ended, so it treats everything like part of the list. That's why it all gets indented. Add the closing `</ul>` tag back in and save it. Now when you refresh the page the rest of tags aren't inside `<ul>` anymore.

### Tag Spelling
Tags need to be spelled correctly for the browser to understand them. What would happen if we misspelled something? 

Find the `<h1>` tag. Let's change it to `<d1>`. Save the document and refresh it in the browser. 

What happened? Since the browser doesn't know what you mean by this tag it can no longer tell that it's a heading and so it doesn't use a larger text to show how important this piece of text is.

### Missing Quotes
Find one of the `<img>` tags. We've just tried misspelling the tag name and the browser wasn't sure what to do with it. But what if we misspell the attribute?

Inside `<img>` tag we have the `href` and `alt` attributes:

Remove the second quote (`"`) from `alt` attribute of this image: the one after the text, so you end up with this:

```HTML
<img href="kitten.jpg" alt="This is a kitten. />
```

Save it and refresh in the browser.

The next tag disappeared. Why? The browser will think that everything after `alt="` and before the next quote (`"`) is the additional text for this image, including the end of the image tag and the next opening tag.

We've made some common mistakes together, and seen that even a tiny error can make the browser struggle to understand what we mean. But most of the time it will try to show us something anyway, so when we've changed the header tag to something else it didn't understand this piece of text was a heading, but it still showed us the text. Smarter text editors like `Notepad++` are best to use, as they will highlight the HTML to show you text between quotes are special.

## Extension Activity Checklist { .check}

+ Open up developer tools to play around with the HTML on your web page. Just right-click anywhere and click `Inspect element`.
+ Move your mouse over different pieces of code. The part of the page that the code represents will light up, so you can see what code does what.
+ Pick a favourite website of yours to go and inspect with developer tools. See what you can change on these websites!

# Next Week Preview: Adding and Linking Content { .activity}

In order to make your web pages more exciting you will want to link to other pages and add content such as images. You have to think about file and folder structure in order to understand how this works. In the provided folder we have two files and one folder inside.

This is called a directory tree:

```
.
├── about_me.html
├── about_me_page_2.html
└── images
    ├── bunny.png
    ├── cat.png
    ├── dog.jpg
    ├── goldfish.png
    ├── hamster.png
    ├── kitten.jpeg
    ├── parrot.png
    ├── spacecat.jpg
    └── tortoise.png
```

When we are making links in the `about_me.html` file, we can refer to `about_me_page_2.html` directly because it's at the same _level_ in the tree.

But our pictures are inside another folder, deeper within the tree. We have to tell the browser this by naming the folder and using a forward slash (`/`). So a link to the image from `about_me.html` needs to look like this:

```HTML
<img src="images/bunny.png" />
```

Now the browser knows to go from the `about_me.html` page level, into `images` and then pick up the `bunny.png` file to display. Aww!

You can use this knowledge to create and link together lots of pages. We'll go through this in detail next lesson.
