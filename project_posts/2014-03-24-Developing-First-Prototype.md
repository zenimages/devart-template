I was thinking about color names for weeks. I learned that there are so many colors, so just _greenish-yellow_ or _yellowish-green_ tells nothing about the color due to [chromatic adaptation](http://en.wikipedia.org/wiki/Chromatic_adaptation). Two colors can simply be the same color for human, since our brain don't normally think about colors in numbers. 

I've found that there are some palettes already available, and the first prominent one was Pantone TCX, because it contains not only 2100 color codes but also the names for them. I was playing with apps that can show RGB values for these colors (plenty of them are available in Google Play) and an idea to create ZenImages just came like a shot.

I've started from a local HTML file and GVIM editor, step-by-step encorporating the widget scroll and the Javascript logic, built arount the Google Images interface:

![GVIM](../project_images/gvim.png?raw=true)

The script is developed and debugged as [Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) extension in Firefox and in Google Chrome, while later is used to find _redundant_ elements in the Google interface with DevTools:

![DevTools](../project_images/devtools.png?raw=true)

Of course, the [Makefile](https://github.com/zenimages/devart-template/blob/master/project_code/Makefile) quickly evolves.

GVIM is a very handy tool in automatic processing of files and it was easy to format [tpxColors](https://github.com/zenimages/devart-template/blob/master/project_code/tpxColors) and then convert it to [HTML](https://github.com/zenimages/devart-template/blob/master/project_code/tpxColors.html). Those are not very good with [vim](http://www.vim.org/) or other powerful text editor tend to write code for parsing text files, but I find it an absolutete overhead since it's a one-time task and the code will be non-reusable anyway.

A bug was found, I've figured out that some colors have quotes, so it resulted a syntax error in Javascript code. More testing is done, Makefile is updating, the code is comressed with [Closure Compiler](http://closure-compiler.appspot.com/home) and I start to feel the release point.
