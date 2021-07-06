# HTML Chapter 16: Images
- you can specify the dimensions of images using CSS
  - helpful when you use the same sized images on several pages of your site
- images can be aligned horizontally and vertically using CSS
- you can use a background image behing the boz created by any element on a page
- background images can appear just once or be repeated across the background of the box
- you can create image rollover effects by moving the background position of an image
- to reduce the number of images your browser has to load, you can create image sprites

# HTML Chapter 19: Practical Information
- search engine optimization (SEO) helps visitors find your sites when using searching engines (Google, Bing, Yahoo, Firefox, Edge)
- analytics tools like Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there
- to put your name on the web, you'll need to obtain a domain name and web hosting
- file transfer protocol (FTP) programs allow you to transfer files from your local computer to your web server
- Many comapnies provide platforms for blogging, email newsletters e-commerce and other popular website tools (to save you writing them from scratch).

# Video and Audio APIs: MDN Article
- HTML5 has elements for embedding rick media in documents - video and audio - which come with their own APIs for controlling playback, seeking, etc. 
```html
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```
- Media Element Player
 ```html
<div class="player">
  <video controls>
    <source src="video/sintel-short.mp4" type="video/mp4">
    <source src="video/sintel-short.webm" type="video/webm">
    <!-- fallback content here -->
  </video>
  <div class="controls">
    <button class="play" data-icon="P" aria-label="play pause toggle"></button>
    <button class="stop" data-icon="S" aria-label="stop"></button>
    <div class="timer">
      <div></div>
      <span aria-label="timer">00:00</span>
    </div>
    <button class="rwd" data-icon="B" aria-label="rewind"></button>
    <button class="fwd" data-icon="F" aria-label="fast forward"></button>
  </div>
</div>
```
``` css
.controls {
  visibility: hidden;
  opacity: 0.5;
  width: 400px;
  border-radius: 10px;
  position: absolute;
  bottom: 20px;
  left: 50%;
  margin-left: -200px;
  background-color: black;
  box-shadow: 3px 3px 5px black;
  transition: 1s all;
  display: flex;
}

.player:hover .controls, player:focus .controls {
  opacity: 1;
}
@font-face {
   font-family: 'HeydingsControlsRegular';
   src: url('fonts/heydings_controls-webfont.eot');
   src: url('fonts/heydings_controls-webfont.eot?#iefix') format('embedded-opentype'),
        url('fonts/heydings_controls-webfont.woff') format('woff'),
        url('fonts/heydings_controls-webfont.ttf') format('truetype');
   font-weight: normal;
   font-style: normal;
}

button:before {
  font-family: HeydingsControlsRegular;
  font-size: 20px;
  position: relative;
  content: attr(data-icon);
  color: #aaa;
  text-shadow: 1px 1px 0px black;
}
```
- HTMLMediaELement API makes a lot of functionalities available for creating simple video and audio players
