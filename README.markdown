
<h1>Note</h1>
Jash is no longer maintained.  There are many mature, full-featured JavaScript consoles to choose from.  Jash was created during a time when IE6 debugging was almost impossible. 

<h1>What is Jash?</h1>
Jash is a JavaScript and CSS shell. It allows you to run arbitratry JavaScript or CSS on a web page.  The shell is implemented as a floating, resizable, repositionable DHTML window in the current HTML page.  Jash is invoked using a bookmarklet. 
 
<h1>Bookmarklet</h1>
Change the script src in the bookmarklet below so that it points to your hosted path for Jash. 
<pre>
javascript:(function(){document.body.appendChild(document.createElement('script')).src='path/to/Jash.js';})();
</pre>

<h1>Building Jash</h1>
The only prerequisite to building Jash is ruby >= 1.9.x.
<pre>
rake build
</pre>

<h1>More information</h1>
http://www.billyreisinger.com/jash
