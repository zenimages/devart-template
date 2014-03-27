I was thinking about color names for weeks. I've learned that there are so many colors, so just _greenish-yellow_ or _yellowish-green_ is nothing about the color due to [chromatic adaptation](http://en.wikipedia.org/wiki/Chromatic_adaptation). Two hues can simply be the same color for human, since our brain don't normally think about colors in terms of numbers. 

I've found that there are some palettes already available, and the first prominent one was Pantone TCX, because it contains not only 2100 color codes but also the names for them. I was playing with apps that can show RGB values for these colors (plenty of them are available in Google Play) and the idea to create ZenImages just came like a shot.

I've quickly started from a local HTML file and GVIM editor, step-by-step incorporating the widget, the scroll and the JavaScript logic, built around the Google Images interface:

![GVIM](../project_images/gvim.png?raw=true)

I've used [Inkscape](http://www.inkscape.org/) to draw a [circle pointer](https://github.com/zenimages/devart-template/blob/master/project_code/selectedColor.png) and then embedded it as data-URL, because the script must be standalone.

Develompent is done as [Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) extension in Firefox and in Google Chrome, while later is used to find _redundant_ elements in the Google interface with DevTools:

![DevTools](../project_images/devtools.png?raw=true)

These elements are then removed by the widget to build a simple and minimalistic interface. It also detects the current color from a search query and places the circle pointer onto it. 

Of course, the [Makefile](https://github.com/zenimages/devart-template/blob/master/project_code/Makefile) quickly evolves.

GVIM is a very handy tool in automatic processing of files and it was easy to format [tpxColors](https://github.com/zenimages/devart-template/blob/master/project_code/tpxColors) and then convert it to [HTML](https://github.com/zenimages/devart-template/blob/master/project_code/tpxColors.html). Those who are not very good with [vim](http://www.vim.org/) or other powerful text editor tend to write code for parsing text files, but I find it an absolutete overhead since it's a one-time task and the code will be non-reusable anyway.

A bug was found, I've figured out that some colors have quotes, so it resulted a syntax error in JavaScript code. More testing is done, Makefile is updating, the code is compressed with [Closure Compiler](http://closure-compiler.appspot.com/home) and I start to feel the release point.
