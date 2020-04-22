<!DOCTYPE html>
<html> 
  <head>
    <title>Processing.JS inside Webpages: Template</title> 
  </head>
  <body>
	
    <canvas id="mycanvas"></canvas> 
  </body>
 

 
  <script src="https://cdn.jsdelivr.net/processing.js/1.4.8/processing.min.js"></script> 
  <script>
  var programCode = function(processingInstance) {
    with (processingInstance) {
      size(400, 400); 
      frameRate(30);
        
      
      fill(255, 255, 0);
      ellipse(200, 200, 200, 200);
      noFill();
      stroke(0, 0, 0);
      strokeWeight(2);
      arc(200, 200, 150, 100, 0, PI);
      fill(0, 0, 0);
      ellipse(250, 200, 10, 10);
      ellipse(153, 200, 10, 10);
    }};

 
  var canvas = document.getElementById("mycanvas"); 
  
  var processingInstance = new Processing(canvas, programCode); 
  </script>
</html>
