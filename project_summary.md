# ZenImages 

***“An art is the beautiful representation of nature for the purpose of giving disinterested pleasure”*** (Ernest Govett, _Art Principles_, 1919)

## Authors
Ivan Khvostishkov, http://github.com/zenimages

## Description
ZenImages is an art project with an extension to Google Images to refine the user interface by searching only selected color names.

The motivation of this project is to convey the mood, created by the beauty of color. It proves that we perceive the colors not as just physical combinations of seven hues of the rainbow. The beauty of nature is in its enchanting colorfulness inherent to the real-world objects and ZenImages makes it able to demonstrate this with the means of Google search API. 

## Link to Prototype

Compiled version is available to install from [userscripts.org](http://userscripts.org/scripts/show/405936) (non-minified — [GitHub](https://github.com/zenimages/devart-template/blob/master/project_code/zenimages.user.js)).

## Example Code
Just to give an idea, how it works, the core of the extension is a database of color entries, like this:
```javascript
cpw_rgb['16-0847']='rgb(173,141,48)';
cpw_name['16-0847']='Olive Oil';
cpw_idx['Olive Oil']='16-0847';
```
Color names are taken from the indexed color palette, which contains as many colors as possible (so far, prototype is using 2000+ from [Pantone](http://pantone.com/)). 

## Links to External Libraries
Tampermonkey extension ([Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)) ([official site](http://tampermonkey.net/)) for Google Chrome is required for an easy installation of the prototype (though it can be still installed in a standard way).

Greasemonkey ([Firefox add-on](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/)) is required to install the prototype into Mozilla Firefox ([GitHub](https://github.com/greasemonkey/greasemonkey/)).

## Images & Videos
Having the extension installed and while searching in Google Images, the color palette appears at the top and the search results then are displayed on a correspondent background of the selected color:

![Olive Oil Screenshot](project_images/olive_oil_screenshot.png?raw=true)

A set of 500+ screenshots is available as a video presentation (no sound): 

http://www.youtube.com/watch?v=Jdtv5mGx1l8&hd=1
