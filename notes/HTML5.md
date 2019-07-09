<dl>
  <dt>HTML Canvas Reference</dt>
  <dd><code>canvas</code> is an HTML element which can be used to draw graphics via JavaScript. This can, for instance, be used to draw graphs, combine photos, or create animations.</dd>

  <dt>Colors, Styles, and Shadows</dt>
  <dd>

|  Property    |	Description                                                                 |
|:-------------|:-------------------------------------------------------------------------------|
|fillStyle	   | Sets or returns the color, gradient, or pattern used to fill the drawing       |
|strokeStyle   | Sets or returns the color, gradient, or pattern used for strokes               |
|shadowColor   | Sets or returns the color to use for shadows                                   |
|shadowBlur	   | Sets or returns the blur level for shadows                                     |
|shadowOffsetX | Sets or returns the horizontal distance of the shadow from the shape           |
|shadowOffsetY | Sets or returns the vertical distance of the shadow from the shape             |

  </dd>

  <dt>Line Styles</dt>
  <dd>

|Property	 |  Description                                                   |
|:-----------|:---------------------------------------------------------------|
|lineCap	 |Sets or returns the style of the end caps for a line            |
|lineJoin	 |Sets or returns the type of corner created, when two lines meet |
|lineWidth	 |Sets or returns the current line width                          |
|miterLimit	 |Sets or returns the maximum miter length                        |

  </dd>

  <dt>Rectangles</dt>
  <dd>
  
|Method	        |Description                                          |
|:--------------|:----------------------------------------------------|
|rect()	        |Creates a rectangle                                  |
|fillRect()	    |Draws a "filled" rectangle                           |
|strokeRect()	|Draws a rectangle (no fill)                          |
|clearRect()	|Clears the specified pixels within a given rectangle |
   
  </dd>

  <dt>Paths</dt>
  <dd>
  
| Method	      |   Description                                                                                 |
|:----------------|:--------------------------------------------------------------------------------------------- |
|fill()	          |Fills the current drawing (path)                                                               |
|stroke()	      |Actually draws the path you have defined                                                       |
|beginPath()	  |Begins a path, or resets the current path                                                      |
|moveTo()	      |Moves the path to the specified point in the canvas, without creating a line                   |
|closePath()	  |Creates a path from the current point back to the starting point                               |
|lineTo()	      |Adds a new point and creates a line to that point from the last specified point in the canvas  |
|clip()	          |Clips a region of any shape and size from the original canvas                                  |
|arc()	          |Creates an arc/curve (used to create circles, or parts of circles)                             |
|arcTo()	      |Creates an arc/curve between two tangents                                                      |
  
  </dd>

  <dt>Transformations</dt>
  <dd>
    
|Method	        |Description                                                                |
|:--------------|:------------------------------------------------------------------------- |
|scale()	    |Scales the current drawing bigger or smaller                               |
|rotate()	    |Rotates the current drawing                                                |
|translate()	|Remaps the (0,0) position on the canvas                                    |
|transform()	|Replaces the current transformation matrix for the drawing                 |
|setTransform()	|Resets the current transform to the identity matrix. Then runs transform() |
  
  </dd>

  <dt>Text</dt>
  <dd>
    
|Property	    |Description                                                       |
|:--------------|:---------------------------------------------------------------- |
|font	        |Sets or returns the current font properties for text content      |
|textAlign	    |Sets or returns the current alignment for text content            |
|textBaseline	|Sets or returns the current text baseline used when drawing text  |
|fillText()	    |Draws "filled" text on the canvas                                 |
|strokeText()	|Draws text on the canvas (no fill)                                |
|measureText()	|Returns an object that contains the width of the specified text   |

  </dd>
</dl>
