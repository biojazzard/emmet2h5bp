Emmet Snippet that renders html5-boilerplate 
==============

html5-boilerplate requires no presentation: [http://html5boilerplate.com/]

Please introduce yourself to the beauty of Emmet[http://emmet.io/]

##How to

* Install Emmet in your favourite text editor.
* Check 'snippets.json' to have custom IF IE support,cmf+f: ie6, sou you can find where, and the add this lines:
* (Or substitute your snippets.json with provided one.)

<pre>
  "html": {
    "filters": "html",
    "profile": "html",
    "snippets": {
      ...
      <strong>"cc:ie7": "&lt;!--[if IE 7]&gt;>\n\t${child}|\n&lt;![endif]--&gt;!",</strong>
      <strong>"cc:ie7l": "&lt;!--[if lt IE 7]&gt;>\n\t${child}|\n&lt;![endif]--&gt;!",</strong>
      <strong>"cc:ie7": "&lt;!--[if IE 7]&gt;>\n\t${child}|\n&lt;![endif]--&gt;!",</strong>
      <strong>"cc:ie7g": "&lt;!--[if gt IE 7]&gt;>\n\t${child}|\n&lt;![endif]--&gt;!",</strong>
      <strong>"cc:ie8l": "&lt;!--[if lt IE 8]&gt;>\n\t${child}|\n&lt;![endif]--&gt;!",</strong>
      <strong>"cc:ie8": "&lt;!--[if IE 8]&gt;>\n\t${child}|\n&lt;![endif]--&gt;!",</strong>
      <strong>"cc:ie8g": "&lt;!--[if gt IE 8]&gt;>\n\t${child}|\n&lt;![endif]--&gt;!",</strong>
      ...
    },
</pre>
*Copy following code and hit [TAB], as always in Emmet.

<pre>
!!!+(cc:ie7l>html.no-js.lt-ie9.lt-ie8.lt-ie7)+(cc:ie7>html.no-js.lt-ie9.lt-ie8)+(cc:ie8>html.no-js.lt-ie9)+(cc:ie8>html.no-js)>html>(head>meta[charset=UTF-8]+meta:compat[content='IE=edge,chrome=1']+title{${1:h5bp}}+meta[description='']+meta:vp+c{Place favicon.ico and apple-touch-icon.png in the root directory}+link:css[href='css/normalize.css']+link:css[href='css/main.css']+script[src='js/vendor/modernizr-2.6.2.min.js'])+body>(cc:ie7l>p.chromeframe>({You are using an}>strong{outdated}+{browser. Please}>(a:link[href='http://browsehappy.com/']>{upgrade your browser})+{ or }>a:link[href='http://www.google.com/chromeframe/?redirect=true']>{activate Google Chrome Frame}+{ to improve your experience.}))+c{Add your site or application content here}+p>{Hello world! This is HTML5 Boilerplate.}+script[src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"]+script[src="js/plugins.js"]+script[src="js/main.js"]+c{Google Analytics: change UA-XXXXX-X to be your site's ID}+script{var _gaq=[['_setAccount','UA-XXXXX-X'],['_trackPageview']];(function(d,t){var g=d.createElement(t),s=d.getElementsByTagName(t)[0];g.src='//www.google-analytics.com/ga.js';s.parentNode.insertBefore(g,s)}(document,'script'));}
</pre>

With Love.

@biojazzard[https://twitter.com/biojazzard] aka Alfredo Llanos[alfredo@tallerdelsoho.es]