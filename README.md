sprits-it! — Awesome Speed-Reading
==================================

`sprits-it!` is an open source web application which allows speed-reading of arbitrary web pages in a browser.

The speed reading technique is currently based on the ideas of [Spritz](http://www.spritzinc.com/) described in their [blog](http://www.spritzinc.com/blog). At the time of this writing [Spritz](http://www.spritzinc.com/) had virtually nothing to offer to `iOs` device users to play with :confused:. So this project is targeted specifically on usability in mobile Safari and Chrome on `iOs`, yet the chances are it would work in other browsers as well.

To read a web page at ``page_url`` use the following API (_temporarily_ hosted at [CodePen](http://codepen.io)):
```
      http://codepen.io/the-happy-hippo/full/aDHrl?url=page_url
```

For example:

> http://codepen.io/the-happy-hippo/full/aDHrl?url=http%3A%2F%2Fwww.spritzinc.com%2Fthe-science

Alternatively, you migh just grab a _bookmarklet_ from the bottom of my [Pen](http://codepen.io/the-happy-hippo/full/aDHrl) page, or create yours manually by pasting the javascript code below in your bookmark:
```javascript
javascript:function iptxt()%7Bvar d%3Ddocument%3Btry%7Bif(!d.body)throw(0)%3Bwindow.location%3D"http%3A%2F%2Fcodepen.io%2Fthe-happy-hippo%2Ffull%2FaDHrl%3Furl%3D"%2BencodeURIComponent(d.location.href)%3B%7Dcatch(e)%7Balert("Please wait until the page has loaded.")%3B%7D%7Diptxt()%3Bvoid(0)
```

## Contributors

The bootstrap code was imported from a [CodePen](http://codepen.io) snippet at http://codepen.io/the-happy-hippo/pen/aDHrl which in turn had been forked from a great Pen by [Charlotte Dann](http://codepen.io/pouretrebelle) at http://codepen.io/pouretrebelle/pen/reGKw with javascript cherrypicking for [Readability](https://www.readability.com) text extraction from [OpenSpritz](https://github.com/Miserlou/OpenSpritz) project by [Rich Jones](https://github.com/Miserlou)(@miserlou).

Up-to-date Gist from codepen can be found at https://gist.github.com/the-happy-hippo/9474002.

Here is the description from [Charlotte Dann](http://codepen.io/pouretrebelle) for her original [Pen](http://codepen.io/pouretrebelle/pen/reGKw):
> Use [Spritz](http://www.spritzinc.com/) right now! Options for speed, localStorage saving, jog forward/backward, text size and dark/light theme, also with keyboard controls and progress bar. You'll never need to read conventionally again. 
> localStorage implementation by [Keith Wyland](http://codepen.io/keithwyland/), thanks Keith!

### Contributing Projects

* [OpenSpritz](https://github.com/Miserlou/OpenSpritz) - OpenSpritz project by [@miserlou](https://github.com/miserlou)
* [Spritz Speed Reading V2](http://codepen.io/pouretrebelle/pen/reGKw) - Codepen Spritz project by [@Charlotte Dann](http://codepen.io/pouretrebelle)
* [Spray](https://github.com/chaimpeck/spray) - OpenSpritz Bootstrap extension by [@chaimpeck](https://github.com/chaimpeck)
