# HTML Chapter 5: Images
- make sure to use non-copyrighted images for public webpages
  - use folder "img" to store all images for webpage
  - Adding images:

![Screen Shot 2021-06-11 at 2 45 31 AM](https://user-images.githubusercontent.com/53208269/121667408-181a1b00-ca5f-11eb-949c-f51e79092311.png)
`-` HTML Duckett book, pg 99
  - also manage height and width
  - `align = 'right/left'`
  - `align = 'top/middle/bottom'`
- Rules for creating images:

![Screen Shot 2021-06-11 at 2 51 17 AM](https://user-images.githubusercontent.com/53208269/121668183-e5bced80-ca5f-11eb-8c26-0ca0f2e7d4ae.png)
`-` HTML Duckett book, pg 1-7



# HTML Chapter 11: Color
- Color info:
  - color options: rgb, hex code, color names
``` css
body {
  color: DarkCyan;
  background-color: #ee3e90/ hsla(0, 100%, 100%, .5) /* hue, saturation, lightness, alpha (transparency)*/
  opacity: .5;
}
```

# HTML Chapter 12: Text
- Type info:
``` css
body {
  font-family: Arial, Verdana, sans-serif
  font-size: 12px = 75%
  font-weight: bold;
  font-style: italic/oblique;
  text-transform: uppercase/lowercase/capitalize;
  text-decoration: underline/overline/line-through/blink;
  line-height: 1.4em;
  letter-spacing: .2em;
  text-align: left/right/justify;
  vertical-align: text-top/text-bottom/baseline;
  ```

  ![Screen Shot 2021-06-11 at 2 37 56 AM](https://user-images.githubusercontent.com/53208269/121666381-08e69d80-ca5e-11eb-9f6c-4623a39faec0.png)
  - HTML Duckett book, pg 288

``` css  
}
@font-face { /*allows you to use a font that isn't installed on the user's computer*/
  font-family: 'ChunkFiveRegular';
  src: url('fonts/chunkfive.eot'); 
}
```
- you can have pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link
