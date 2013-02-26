<h1>HERE'S THE DIRTY TRUTH ABOUT RESPONSIVE EMAILS</h1>
<hr>

This whole thing is based off this simple structure:<br>
<strong>js fiddle -</strong> http://jsfiddle.net/sollenne/HE8LY/ <br>
<strong>live example -</strong>  http://sollenne.com/projects/responsive-email/mycode.html

<strong>Here is a live example of template 1 - </strong> http://sollenne.com/projects/responsive-email<br>
<strong>Here is a live example of template 2 - </strong> http://sollenne.com/projects/responsive-email/index2.html<br>

<hr>

<strong>If you happen to test in another email environment or have an update or question, email me at rich@sollenne.com</strong> 

<hr>
<br>
<br>
<br>
<br>

<h2>Some of the things I've learned</h2>

<strong>1.</strong> Quickly familiarize yourself with tables.
	
<strong>2.</strong> Not every email client supports <code>@media</code>

<strong>3.</strong> Do not show/hide multiple divs with the same content intending to switch them out with media queries. Some emails will render both and you will look crazy. On the same note, don't have one complete email template for one size and another template for a different size expecting one to show and one to hide. Again, some emails will render both and you will look even crazier. Code as if everything you write will show up in an email, eving if you dont intend it to. 

<strong>4.</strong> Almost all styles need to be inline. The only exception is width and MAYBE a few others if you see they are working. 

<strong>5.</strong> The more media queries you use, the more complicated it gets. I only have two and that was confusing enough. 

<strong>6.</strong> Images must be publicly hosted. Otherwise, Some email clients will render an error and some will just ignore images and display... NOTHINGNESS.

<strong>7.</strong> I use http://placehold.it for my placeholders I stongly recommend it. 

<strong>8.</strong> use doctype:<br>
<code><!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd"></code><br>
The page will most likely delete or replace your fancy html5 <code><!doctype html></code> or any doctype for that matter.

<strong>9.</strong> Don't use html5, css3, js, jq, less, external stylesheets or anything fun or cool. (except <code>@media</code>)

<strong>10.</strong> Don't use Margins, Yahoo! and Hotmail don't like them. Don't use div's unless it's strictly for semantics (styles), just use a span tag in this case<br> (practice what I preach, not what I do).

<strong>11.</strong> Style linked images with <code>style="border:none;"</code>

<strong>12.</strong> <code>width="100%"</code> works fine but some email clients align this to the left. You should declare a width on each table. Either way, you should be consistent. Make them all the same.

<br>
<br>
<br>
<br>
<hr>

<h2>HOW TO TEST</h2>
<strong>So far, the easiest way is to use Safari and press Command+I. This will open a new email in your default email client.</strong>

<hr>

<h3>I've Successfully Tested In:</h3>
- Apple Mail for desktop - Snow Leopard & Mountain Lion<br>
- Apple Mail for iPad & iPad mini - iOS6, iOS5<br>
- Apple Mail for iPhone - iOS6, iOS5<br>
- Android Mail - v4<br>
- Gmail app for Android<br>
- Gmail app for iPhone<br>
- Gmail.com for desktop<br>
- Gmail.com for mobile
- Hotmail.com for desktop<br>
- Hotmail.com for mobile<br>
- MS Outlook 2003, 2007<br>
- mail.AOL.com for desktop<br>
- mail.AOL.com for mobile<br>
- mail.Yahoo.com for desktop<br>
- mail.Yahoo.com for mobile<br>
- Yahoo! Mail iPhone app<br><br>

<h3>Still Needed:</h3>
- MS Outlook, 2010, 2013<br>
- Yahoo app for Android<br>
- Hotmail app for Android<br>
- Windows phone<br>
- Microsoft Surface<br>
- Android tablets<br>
- Kindle Fire<br><br>

<h3>@media Not Available (Renders Desktop Version Only):</h3>
- Gmail app for iPhone<br>
- Gmail app for Android<br>
- Gmail.com<br>
- Hotmail.com<br>
- Hotmail.com on iPhone<br>
- Yahoo app for iPhone<br>
- mail.Yahoo.com for desktop<br>
- mail.Yahoo.com for mobile<br>
- mail.AOL.com for desktop<br>
- mail.AOL.com for mobile<br><br>

<h3>Images Not Displayed Until Told To Do So:</h3>
- all Gmail<br>
- all AOL <br>
- MS Outook 2007<br><br>

<h3>Known Issues</h3>
- MS Outlook 2003 defaults to a wider font, may cause widowed words or links.<br>
- MS Outlook 2007 adds inconsistent horizontal spacing between tables. Content functions the same.<br><br>

<h3>Complete Failures</h3>
- Hotmail iPhone app completely fails to properly render the most basic email. <br><br>
<br>
<br>
