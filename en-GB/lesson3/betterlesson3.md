## activity { .checklist}

+ Create another web page and make a link to it. Try starting with the `about_me_page_2.html` by opening it in `Notepad++`.
+ Download more images from other web sites and put them in your images folder, or even a new folder you created. Can you make links to them?

## Create a Second Page

Let's create another page. Open `about_me_page_2.html`. It has a little bit less code than the last page you were working with, but I'm sure you know all the tags well enough by now! You did do your homework, right?

__Some hints and ideas:__

* Add a heading that will serve as the title of this page.
* You could make this page about your pet, your favourite hobby or your friends and their hobbies.
* Add a list of things your pet, or friend likes, or a list of reasons why this is your favourite hobby.

__Are you done? Great! Let's now link the two pages you have created together.__

When we've been linking to parts of the same page, we could just point links to a specific `id` within a page, like this:
	
```HTML
<a href="#kitten">Click to see a kitten</a>
```

Which then took you to something like this:

```HTML
<div id="kitten">
	<img src="kitten.jpg" alt="This is a kitten." />
</div>
```

But to link to another page, we don't need to include the hash symbol (`#`) - instead we need to say which file we would like the link to take us to (and where it is, if it's within a different folder than the current HTML file).

So to link from `about_me_page_2.html` to `about_me.html` write it like this:

```HTML
<a href="about_me.html">Go to About Me page</a>
```

You can change the link text to something else, like the page title if you have changed it.

To link back from `about_me.html` to `about_me_page_2.html` you would have to write it like so:

```HTML
<a href="about_me_page_2.html">Go to my second page</a>
```

Congratulations, you have made your own website!

## Things to try { .try}

* How could you link to another page on the web? Try putting the text in the address bar of your favourite website within the `href=""` attribute of an `anchor` tag.
* Make a third page for your website containing links to your favourite other websites.
* Add a picture from somewhere on the web instead of from your computer. Try finding a picture with Google Images, then pressing on View Image so it takes you to a page of just that image. Now the address in the address bar is the link to use in the `src=""` attribute.
* Save the image file by right-clicking and choosing the save option. Put it in your images folder/directory, and link to it this way instead. This is better, as now your picture will work if the other website's servers break down.
