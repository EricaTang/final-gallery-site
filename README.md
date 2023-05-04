Documentation of my process
- Initial ideas about the theme of the website – a digital gallery that serves as an extension to the photography section of my portfolio site
- Drawing wireframes to further decide on the design and the navigation of the gallery
- Gathering photos and putting them into different categories
- Watching tutorials online and reviewing some of the class notes
- Creating the landing page
- Creating the home page
- Creating the page for each photo collection
- Including pop-up modals for “about” and “contact”
- Adding a loader to some of the pages
- Media queries

Explanation of some of my source code
- The image slider
  - I used the swiper-bundle.js for this
  - disableOnInteraction: false --> make it loop through the images constantly even if I clicked the swiper or the pagination
- The page loader 
  - jQuery
  - $(window).on("load",function() {
			$(".loader-wrapper").fadeOut("slow");
		});
	- When all the content in the webpage finish loading, it select an element with the class "loader-wrapper", and then class the fadeOut() method. This method would make the elements gradually decrease in opacity until completely transparent. 
  - @keyframes loader {
	0% {transform: rotate(0deg);}
	25% {transform: rotate(180deg);}
	50% {transform: rotate(180deg);}
	75% {transform: rotate(360deg);}
	100% {transform: rotate(360deg);}
}
	- This is one of CSS codes I found interesting. It is bascially keyframing the motion of the loader and assign specific rotation angles.  

Issues I encountered
- The page loader
  - I wanted to make the duration longer if the content on the page loads really fast
- The modals
  - Once I finished making two pop-up modals in the landing page, it flashes every time I refresh the page. I used the loader to hide that flash but still didn’t figure out how to fix that. 
- Media queries were time-consuming
- Content in divs exceeds the body
  - I couldn’t fix that by making HTML & body's height = 100%. But I end up resolving this issue by directly setting the image as the background image in CSS instead of inserting an image inside a wrapper div in HTML.

What I learned in order to accomplish my project
- More HTML & CSS
- Some JavaScript
- Html forms
- Pop-up modal

Next steps
- Adding a music player to each page - TweenMax.js for the design of the music player
- GreenSock animation
- More JavaScript – create smooth scrolling and cooler hovering effects
- A more complicated landing/ loading animation
- etc.
