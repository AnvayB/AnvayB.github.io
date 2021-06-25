# CSS Animations

## Transformers
- 2D rotate: spinning horizontally along the y axis when mouse hovers over a figure
- Scale, Multiple Scaling: resizes the figure
- Translate: move the figure
- Skew: angle rotate/shift the figure
- Combining Tranforms:
```html
.box-1 {
  transform: rotate(25deg) scale(.75)
```
- 2D Cube
```html
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>
<figure class="box-3">Box 3</figure>
<figure class="box-4">Box 3</figure>
```
```css
.box-1 {
  transform: rotate(15deg);
  transform-origin: 0 0;
}
.box-2 {
  transform: scale(.5);
  transform-origin: 100% 100%;
}
.box-3 {
  transform: skewX(20deg);
  transform-origin: top left;
}
.box-4 {
  transform: scale(.75) translate(-10px, -10px);
  transform-origin: 20px 50px;
}
```
## Animations
- Changing colors
- Property Transition (Square to Circle)
  - set Transition Durations
  - set Delay
- Animation of Button Click
- Card flip

## [8 Simple CSS Transitions](http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)
- Fade in
- Change color
- Grow & Shrink
- Rotate Elements
- Square to Circle
- 3D Shadow
- Swing (Vibrate Side-to-Side)
- Inset Border

## (6 Buttons Animated)[http://codepen.io/retyui/pen/ByoaXV]

## (Bouncing Ball Animation Loop)[http://codepen.io/akshaychauhan/pen/oAfae]

## 
