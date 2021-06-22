# Easily create stunning animations with Chart.js
- JS plugin to make charts and draw graphs on a page
- Line chart `new Chart(buyers).Line(buyerData);`
  - uses labels, colors, and data points to make an animated line graph
- Pie Chart `new Chart(countries).Pie(pieData, pieOptions);`
  - uses separate values and colors to mark parts of the pie chart
- Bar chart `new Chart(income).Bar(barData);`
  - uses labels, colors, and data points for separate sections of the bar chart 

# Chartjs.org
- creating a chart
```html
<canvas id="myChart" width="400" height="400"></canvas>
<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            y: {
                beginAtZero: true
            }
        }
    }
});
</script>
```

# Canvas API
- `<canvas>` element:
  - similar to `<img>` element, except it only has width and height attributes (300px X 150px)
  - uses ^^ dimensions to draw shapes on grid
    - Rectangle shape example
    ```js
    function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
      var ctx = canvas.getContext('2d');

      ctx.fillRect(25, 25, 100, 100);
      ctx.clearRect(45, 45, 60, 60);
      ctx.strokeRect(50, 50, 50, 50);
      }
    }
    ```
  - [Drawing Lines and Triangles](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
- Styles and Colors
  - Red to Green blocky transition:
  ```js
  function draw() {
    var ctx = document.getElementById('canvas').getContext('2d');
    for (var i = 0; i < 6; i++) {
      for (var j = 0; j < 6; j++) {
        ctx.fillStyle = 'rgb(' + Math.floor(255 - 42.5 * i) + ', ' +
                         Math.floor(255 - 42.5 * j) + ', 0)';
        ctx.fillRect(j * 25, i * 25, 25, 25);
      }
    }
  }
  ```
  - [More Transitions, strokeStyle, gloablAlpha, rgba()](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
- Drawing Text
  - Styling fonts
  - `fillText(text, x, y [, maxWidth])`
  - `strokeText(text, x, y [, maxWidth])`
  ```js
  function draw() {
    var ctx = document.getElementById('canvas').getContext('2d');
    ctx.font = '48px serif';
    ctx.strokeText('Hello world', 10, 50);
  } 
  ```
