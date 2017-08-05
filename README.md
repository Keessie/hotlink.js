hotlink.js
==========

hotlink.js makes it possible to hide referrer information for hotlinked images. It is an
easy-to-use drop-in script that requires very few changes to your webpages.

Demo
----

You can try out the [online demo][1] to see hotlink.js in action.

Supported Browsers
------------------

* Chrome 12+
* Edge
* Firefox
* Safari 5.1+
* Internet Explorer 11+

Unlisted browsers may still be supported. Unsupported browsers will fall back
to a normal image without a hidden referrer.

Getting Started
---------------

1. [Download hotlink.js][2] ([unminified][3]).
2. Replace `<img src="...">` with `<img data-src="...">` for every image that you want
   to hotlink on your site.
3. Include `<script type="application/ecmascript" async="" src="hotlink.js"></script>`
   right before `</body>`.

API
---

    void hotlink(HTMLImageElement image)

If you are using dynamically inserted images, you'll want to use the API to hotlink them.

### Example

    var image = new Image(300, 100);
    image.setAttribute("data-src", "http://example.com/image.png");
    document.documentElement.appendChild(image);
    hotlink(image);

Disclaimer
----------

This library is only to be used for research purposes and I am not responsible for anything
you make with this library.

![Tracking image](https://in.getclicky.com/212712ns.gif)

  [1]: http://eligrey.com/demos/hotlink.js/
  [2]: https://raw.github.com/eligrey/hotlink.js/master/hotlink.min.js
  [3]: https://raw.github.com/eligrey/hotlink.js/master/hotlink.js
