# What happens to the layout when you resize the screen to less than 550 px.
Here are the things I immediately observe:
* There number of `iphone.png` images changes from 2 to 1.
* The `hero-heading` moves to the top of the page.
* The `a.button.button-primary` element sits under the `hero-heading`.
* The number of columns in the all of the `div` elements goes from 3 to 1.
* The placeholder images are resized according to the width and height of the screen.
* The padding between the images and text also increases when the screen is wider.

# How do you think that works?
I think when the screen is resized to less than 550 px on the [responsive site demo](http://getskeleton.com/examples/landing/) page, the page is rendered based on:
* All of the framework's `skeleton.css` found [here](https://github.com/dhg/Skeleton/blob/master/css/skeleton.css)
* All of the framework's `normalize.css` found [here](https://github.com/dhg/Skeleton/blob/gh-pages/dist/css/normalize.css), and
* Lines 1 to 68 of the responsive demo page's `custom.css` found [here](https://github.com/dhg/Skeleton/blob/gh-pages/examples/landing/css/custom.css)

What I am now understanding is that it can take a combination of source CSS files to dictate the style, behaviour, and functionality of a webpage. It is up to the web developer that the browser knows which CSS pages it can use, when, and how.

What's really enlightening from reading this framework is that I found what is really meant by designing for "mobile by _default_":
* Start with building the web page from the mobile page from the start of your framework.
* As the screen size gets bigger, build your site so that it responds to having more room to render its contents.

This totally blew away my thinking about web site design and development: I assumed a really pretty page design started from thinking big and then going small. Nope: intuitive, responsive, flexible, and meaningful web page design starts small and goes big.

Awesome :)