---
layout: post
title:  "Pre-compiling CSS for the first time"
author: Niall Thurrat
---
***
A CSS preprocessor is a program that lets you generate CSS from that preprocessor's own unique syntax and it offers much more functionality than simply writing your own CSS stylesheet.  I’ve been using the well know SASS preprocessor to help me style this website.

#### Pros compared to regular CSS:

- Regular CSS stylesheets often have a lot of repeated code to apply the same styles to different parts of a document. The SASS preprocessor addresses this problem in a number of ways. It is really easy to create variables which hold CSS styling, meaning you can simply refer to a named variable, instead of writing the same properties and values over and over again.  This has the added benefit of making it really easy to change the value of all styling which points to that variable. We can also use @extend to add previously written styles to other elements (inheritance) by simply adding the predefined name of the styling to be extended.
- Regular CSS can often be hard on the eyes when you’re scrolling through a list of dozens of slightly different ‘nav li ul a’ stylings. Preprocessors combat this by enabling selector nesting meaning we no longer have to write the ‘nav’ 20 times! 
- SASS also builds on the regular CSS @import option, and compiles your CSS files into one, so that only one file is sent to the server and additional HTTP requests are avoided. Partial files in preprocessors also help us to modularize our CSS and structure its content more clearly.
- Regular CSS does not recognize the use of operators and this can, for example, mean doing calculations yourself when it comes to the sizing and spacing of the elements on your page. Preprocessors allow us to use operators and do those calculations in the file itself.

#### Cons compared to regular CSS

- One disadvantage of preprocessors is that they are harder to debug in the browser.  Regular CSS makes HTTP requests for each CSS file and errors can therefore be linked to specific line numbers. This is not true for preprocessed CSS.
- There is a certain simplicity to adding CSS files to your website which is lost when using preprocessors. Instead of simply writing you stylesheet and linking it in your HTML doc, now you will need to more tools and more effort to set things up.  As a knock on effect, it takes longer to build in the beginning.
 
#### Which techniques did I use?

This website makes use of the many advantages of the SASS CSS preprocessor. It uses a main minima.scss file where all variables are defined, making it a kind of main control panel for adjusting main styling values such as color and fonts.  It also imports 3 partials, 2 of which I pulled into my root directory for amendment: _base.scss and _layout.scss. Each partial file uses clear nesting, and @export is used to avoid repetition of code.

#### What do I think of pre-compiling CSS?

To create this website I’ve used a Jekyll boilerplate and decided to adapt the default minima theme.  As a result I have benefited from the carefully and clearly structured code in the theme which uses the SASS .scss files. I therefore have avoided the hard work of creating the main minima.scss file and its 3 imported partial files which organize the styling structure. All I had to do was tailor the values of the previously created variables, copy and paste a few @extends and create a few variables of my own. I have found the code easier to read than CSS, better structured, easier tailored, more logical and more capable.  For these reasons, I think CSS preprocessors are great.

***