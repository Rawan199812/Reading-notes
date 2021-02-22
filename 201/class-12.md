Drawing a line chart
To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. < canvas id=”buyers” width=”600” height=”400”></ canvas >
we need to write a script that will retrieve the context of the canvas < script> var buyers = document.getElementById(‘buyers’).getContext(‘2d’); new Chart(buyers).Line(buyerData); </ script>
Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart
data var buyerData = { labels : [“January”,”February”,”March”,”April”,”May”,”June”], datasets : [ { fillColor : “rgba(172,194,132,0.4)”, strokeColor : “#ACC26D”, pointColor : “#fff”, pointStrokeColor : “#9DB86D”, data : [203,156,99,251,305,247] } ] }
Drawing a pie chart
< canvas id=”countries” width=”600” height=”400”>< /canvas>
var countries= document.getElementById(“countries”).getContext(“2d”); new Chart(countries).Pie(pieData, pieOptions)
data var pieData = [ { value: 20, color:”#878BB6” }, { value : 40, color : “#4ACAB4” }, { value : 10, color : “#FF8153” }, { value : 30, color : “#FFEA88” } ];
Drawing a bar chart


< canvas id=”income” width=”600” height=”400”>< /canvas>

var income = document.getElementById(“income”).getContext(“2d”); new Chart(income).Bar(barData);
data var barData = { labels : [“January”,”February”,”March”,”April”,”May”,”June”], datasets : [ { fillColor : “#48A497”, strokeColor : “#48A4D1”, data : [456,479,324,569,702,600] }, { fillColor : “rgba(73,188,170,0.4)”, strokeColor : “rgba(72,174,209,0.4)”, data : [364,504,605,400,345,320] }
] }
CANVAS
Basic usage of canvas < canvas id=”tutorial” width=”150” height=”150”>< /canvas> At first sight a < canvas> looks like the < img> element, with the only clear difference being that it doesn’t have the src and alt attributes
Fallback content he 
Required < /canvas> tag As a consequence of the way fallback is provided, unlike the < img> element, the < canvas> element requires the closing tag (< /canvas>)
Drawing shapes with canvas 
Drawing shapes with canvas
 The grid
 Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default
 Drawing rectangles
 Unlike SVG, < canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes
 First let's look at the rectangle. There are three functions that draw rectangles on the canvas
1. fillRect(x, y, width, height) --> Draws a filled rectangle.
2. strokeRect(x, y, width, height) --> Draws a rectangular outline.
3. clearRect(x, y, width, height) --> Clears the specified rectangular area, making it fully transparent.
 Drawing paths
 Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps
1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.
 Here are the functions used to perform these steps
1. beginPath() --> Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
2. Path methods -->Methods to set different paths for objects.
3. closePath() --> Adds a straight line to the path, going to the start of the current sub-path.
4. stroke() --> Draws the shape by stroking its outline.
5. fill()-->Draws a solid shape by filling the path's content area.
 The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes
The second step is calling the methods that actually specify the paths to be drawn. We'll see these shortly
 The third, and an optional step, is to call closePath(). This method tries to close the shape by drawing a straight line from the current point to the start. If the shape has already been closed or there's only one point in the list, this function does nothing
 Basic usage of canvas
 At first sight a < canvas> looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the < canvas> element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted