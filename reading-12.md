# reading 12
### 17 march 2020

# Read [this article(https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/){:target="_blank"} on the Chart.js API.
broken link, sends me to 404 page.

# Chart.js docs: You’ll be needing these!
chart.js is available under an MIT liscence. all that is required to create a chart is to include the script and a <canvas> tag in the html to render chart.

# Basic usage
<canvas> is like <img> except it does not have an src or alt attribute, only width and height. without width and height it will default ot 300x 150px if not specified. unlike the <img> tag, <canvas> requires a closing </canvas> tag, if no closing tag, content will not be displayed.

# Drawing shapes with canvas
depending on the dimentions given in teh tag, hte canvas will have coordinates. 0 , 0 is the top left most corner of the canvas grid, and X will control the location of the top left corner of the square. a path is a list of points connected by segments that can be different colors and shapes. beginPath() creates a new path, then path methods are passed in for direction. closePath() adds a straight line to the path to the start of the current sub path. stroke()draws the surrent shape by stroking its outline. and fill() draws a solid shape by filling in the paths contnt area. there are ways to make triangles, arcs, curves, quote and thought bubble shapes, hearts, and ways to compine all of these options.

# Applying styles and colors
fill style color is used to fill in shapes and stroke style color is used to set the style for the outlines. you can set transparencey with alpha and set a global alpha. you can also set line styles and width. you can also change the line cap how you want the end of the line to look, like a rounded edge or a hard squared edge. you can set dottes lines and gradients, as well as define what kind of gradient you  are looking for. you can also set patterns and shadows.

# Drawing text
drawing text lets you manipulate the appearance of the text on your page, weather you eant it solid and filled in or a hollow outlined character. you can style the text with different fonts, like cursive or characters from other languages. 

# code
#### bar chart
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
            yAxes: [{
                ticks: {
                    beginAtZero: true
                }
            }]
        }
    }
});
</script>

#### drawing rectangle on canvas
fillRect(x, y, width, height)
    Draws a filled rectangle.
strokeRect(x, y, width, height)
    Draws a rectangular outline.
clearRect(x, y, width, height)
    Clears the specified rectangular area, making it fully transparent.

