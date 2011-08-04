hotlink.js
==========

hotlink.js makes it possible to undetectably hotlink images.

Demo
----

You can try out the [online demo][1] to see hotlink.js in action.

Supported Browsers
------------------

* Google Chrome 12+
* Safari 5.1+
* Opera 11.50+

†Firefox 5+ and Internet Explorer 9+ will fall back to a normal image without a
hidden referrer.

Getting Started
---------------

1. [Download hotlink.js][2] ([unminified][3]).
2. Replace `<img src="...">` with `<img data-src="...">` for every image that you want
   to hotlink on your site.
3. Include `<script type="application/ecmascript" async="" src="hotlink.js"></script>`
   right before `</body>`.

![Tracking image](//in.getclicky.com/212712ns.gif)

  [1]: http://eligrey.com/demos/hotlink.js/
  [2]: https://raw.github.com/eligrey/hotlink.js/master/hotlink.min.js
  [2]: https://raw.github.com/eligrey/hotlink.js/master/hotlink.js