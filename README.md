# css_bugless

<h1>Responsive web page with HTML/CSS</h1>
Very first try from the markup to polishing CSS. Did much as I can do it by myself, with googling. Also virtually discussing with the lecturer's way of markup and all. Then until really 'making' it, took me a month. But totally worth.<br>
Project summary : <a href=https://www.notion.so/Bugless-final-project-HTML-CSS-e815e0759b914db0b559d53f61369069>Summary in Notion</a> <br>
<br>
<h2>First days</h2>
<p>First of all, I want to build up (mark up) HTML with five sections according to mobile version of figma source. (My mind : Actually right now I'm confused how to make it mobile first and responsive it by codes, but anyway let's start with building up the basic structure)

I was so undetermined when to use "div" tag at first. It wasn't an only problem though. 

My process was like

1. divide the sections with "section" tag first, and divide "h1", "p", "span", "strong" first
2. checked where and how to use footer (yes, head-body-footer)
3. Keep collapsing between or beyond(...) flexbox and grid-system of bootstrap. 
4. Anyway I marked up with rules above in HTML, then started to do the CSS also following the divided tag and section.
5. Was wondering how am I going to write the codes as it is responsive and probably mobile-first, and desktop display is bit different (not only the size). → used to only watching others coding this sort of part. Anyway found out styles should apply to mobile devices first then add other ones via media queries to larger sizes.
6. keep wondering what is need? what has to be declared? Is position should be declared or display? what to declare in parent?
  The original design by kimbug, goormedu(the course was offered via this platform)</p>
  <h2>Second Round</h2>
  <p>First few days of April : Trying to check the entire code structure and see how I'm going to use common classes for style.
Yet also trying to figure out why some sections are displayed well and why some are broken...
why...
actually more than why, how I can fix that.

Status : 
→ Curriculum section and subscribe information section are collapsing
→ size of "img" tag and alignment of it seems not so stable (or should I rather use safe? anyway)

Hint
check HTML markup (for grid system)
[https://github.com/rohjs/bugless-101/blob/master/css-practice/final/index.html](https://github.com/rohjs/bugless-101/blob/master/css-practice/final/index.html)
Later to check the frequent error msg
[https://code.visualstudio.com/docs/supporting/faq#_resolving-shell-environment-is-slow-error-warning](https://code.visualstudio.com/docs/supporting/faq#_resolving-shell-environment-is-slow-error-warning)

<h3>Problems or new points I got on April 1st</h3>

<p>One, if there are declarations of width and height value in mobile or original style declaration, then the size will be sustained to the desktop version as well. So that I remove those and only left the padding value to make it responsive. Did grid help in this? (guess grid system row and things get flex property automatically)

Two, text-align:left was not working for section (graphically it was centered so I tried to change)

→ Now I check, I don't know what is working there for make the text elements to be centered, but default should be left align ([https://css-tricks.com/almanac/properties/t/text-align/](https://css-tricks.com/almanac/properties/t/text-align/)). 

→ Firstly removed "align-items-center" (or maybe it's in another name) class that was justified with row class.

Three, when alignment has to be row from column, it doesn't work

Four, <img> element is anyway out of the size (sort of bumping out...?) it is display: none in mobile though. What should I give for desktop version? 

(in this case for curriculum section, it was about giving "img" tag separate "div" class with col-12 col-md-6)

Still the image was too big, and I finally found that I also was giving all those properties to another div and div that was embedding <img>. So I changed and give those to div and the img tag directly.

Five, grid system must be convenient one to use, but I still don't know how I can use and apply.
  
  <strong> Have more records in Notion : <a href=https://www.notion.so/Bugless-final-project-HTML-CSS-e815e0759b914db0b559d53f61369069>Project Notes in Notion</a> </strong> <br/>
  <br/><em>The original design by <a href="https://github.com/rohjs">@rohjs</a>, kimbug at goormedu(the course was offered via this platform)</em>
