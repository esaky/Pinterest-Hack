# Pinterest-Hack
Pinterest Hack for Bloggers and Designers by AnimHuT

This pinterest code will add a "pin it" button instead of Three Different Pinterest Buttons. You can use WordPress Plugin for each one.
For an article WordPress many plugins use a default featured images to pin. In case if you add more buttons - like one for pinning images found in the article and another one for showing Pinterest Vote Count to your readers. Here you can use this code to enable all the features in a page.

" How to enable new Pinterest button which “Pin-it” or bookmark all images with number of Vote counter is a new factor for every bloggers and pinterest fans seeking to implement for their blog or website. This technique will pin all the images + show the number of votes you got for each article and instead of one default thumbnail images for an article or post which contain 100+ images and we are sure you won’t like to pin only one default thumbnail. So let’s get to pin more and drive traffic to your blog."

Now readers can pick which pinterest vote type they want to implement in their blog
Default Types:
One Image - Any Image - Hover Image

Note: For Google Analytics or Adsense using Async is good, so we are going to use Async Javascript for Pinterest Code.

Add this code to your Header.php file:
<center><script type=”text/javascript”>// < ![CDATA[<br />
(function(d){<br />
  var f = d.getElementsByTagName(‘SCRIPT’)[0], p = d.createElement(‘SCRIPT’);<br />
  p.type = ‘text/javascript';<br />
  p.setAttribute(‘data-pin-hover’, true);
  p.async = true;<br />
  p.src = ‘//assets.pinterest.com/js/pinit.js';<br />
  f.parentNode.insertBefore(p, f);<br />
}(document));<br />
// ]]></script></center>

Add these Pinterest code in your WordPress Theme – Single.php

<a href=”//www.pinterest.com/pin/create/button/” class=”pin-it-button” count-layout=”vertical” >Pin It</a>

Here we have added class="pin-it-button" count-layout="vertical" -> which means you can add a "pin-it" button and Pinterest style button like horizontal or vertical. So when you add the 
 p.setAttribute(‘data-pin-hover’, true); -> this will enable pinterest hover button.
