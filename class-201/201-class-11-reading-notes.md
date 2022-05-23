# Audio, Video, Images

- Duckett, J. (2011). Html &amp; Css. John Wiley &amp; Sons, Inc.

- [Video and Audio APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs)

## Images

- **Size** - use width and height properties in CSS. Set uniform small, medium, and large sizes within your CSS with:

        img.large {
          width: 500px;
          height: 500px;
        }

- **Align** - use the float property added to the class that was created to represent the size of the image

- **Centering** - make the image a block level element with the display property then either use the 'text-align' property on the containging element or on the image itself use the margin property and set the left and right to auto

- **Background Images** - use the 'backgraound-image' property under a containing element and set it to the URL of the photo

- **Repeating Images** - use 'background-repeat' with values 'repeat', 'repeat-x', 'repeat-y', or 'no-repeat'. Use 'background-attachment' with 'fixed'or 'scroll' to have the image stay put or move when the page is scrolled

- **Background Position** - use 'background-position' to specify where in the browser window the background image should be placed

- **Background Shorthand** - properties must be specified in this order: 'background-color', 'bachground-image', 'background-repeat', 'background-attachment', 'background-position'

- **Contrast of background images** - if you wnat to overlay text on a background image, the image must be low contrast in order for the text to be legible

- To reduce the number of images your browser has to load, you can create image sprites

## Practical Information

- **Search Engine Optimization (SEO)** - is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers

- **On-Page SEO** - 7 key places where keywords can appear in order to improve findability - PAge title, URL/web address, headings, text, link text, image alt text, page descriptions

- **Identify keywords** - 6 steps to help you identify the right keywords and phrases for your site: brainstorm, organize, research, compare, refine, and map

- **Analytics** - Use services like Google Analytics to analyze how people are coming to your site, where they came from, what they are looking at, when they leave..

- **FTP & third party tools** - to transfer your code and images from your computer to your hosting company, you use something known as File Transfer Protocol

- To put your site on the web, you will need to obtain a domain name and web hosting

## Video and Audio APIs

- Elements for embedding media in documents:

        <video>
        <audio>

- **Controls Attribute** - enables the default set of playback controls, you can hide the native controls by removing the 'controls' attribute and program your own with HTML, CSS, and JS

- **HTMLMediaElement API** - provides features to allow you to control video and audio players programmatically

- **CSS** - '.controls' styling can include: visibility, opacity, width, border-radius, position, botom, left, margin-left, background-color, box-shadow, transition, and display. Also use CSS to style button icons and the timer.

- **JavaScript** - Create a JS file in the same directory level as the index.html file. Include in your code constants to hold reference to all the objects you want to manipulate: 3 groups: The 'video' element and the controls bar, the play/pause + stop + rewind + fast forward buttons, and the outer timer wrapper 'div' + the digital timer readout 'span' + the inner 'div' that gets wider as the time elapses

        media.removeAttribute('controls');
        controls.style.visibility = 'visible';

- These two lines remove the default browser controls from the video and make the custom controls visible

- **Play/Pause** - Define playPauseMedia() function at the bottom of your code and dont forget to invoke it.

- **Stopping** - Define stopMedia() function below the previously stated function. Add a stop.addEventListener('click', stopMedia) and media.addEventListener('ended', stopMedia)

- **Seeking Back and Forth** - add rwd.addEventListener('click', mediaBackward) and fwd.addEventListener('click', mediaForward). Then create the event handler functions to define 'mediaBackward()' and 'mediaForward()'. Then define 'windBackward()' and 'windForward()' invoked in the setInterval() calls

- **Elapsed Time** - run a function to update the time displays every time the 'timeupdate' event is fired on the 'video' element. Add the media.addEventListener('timeupdate', setTime) then define the 'setTime()'

[Return home](https://khofstetter94.github.io/reading-notes/)
