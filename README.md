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
        - This code is a jQuery script that listens to the "load" event on the window object
        - which is triggered when all the resources of a webpage have finished loading.
        - When the "load" event is fired, the script selects an element with the class "loader-wrapper"
        - and then calls the fadeOut() method on it with the argument "slow"
        - This method is used to gradually decrease the opacity of the selected element until it becomes completely transparent.
        - Therefore, this code fades out the element with the class "loader-wrapper" slowly
        - indicating to the user that the page has finished loading and it is now ready to be displayed.

Issues I encountered
- The page loader - didn’t figure out how to make the duration longer if the content on the page loads really fast
- The modals
  - Once I finished making two pop-up modals in the landing page, it flashes every time I refresh the page
  - I used the loader to hide that flash but still didn’t figure out how to fix that
- Media queries were time-consuming
- The content in the div on the home page exceeds the boundaries of the body
  - I couldn’t fix that by making HTML & body 100% height
  - I end up figuring out that it is my image added to the background that caused this, so I changed to directly set it as the background image in CSS instead of inserting an image inside a wrapper div in HTML.

What I learned in order to accomplish my project
- More familiar with HTML & CSS
- Some JavaScript
- Html forms
- Pop-up modal

Next steps
- Adding a music player to each page - TweenMax.js for the design of the music player
- GreenSock animation
- More JavaScript – create smooth scrolling and cooler hovering effects
- A more complicated landing/ loading animation
