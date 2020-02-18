
# Chart.js

## Notes
- canvas element has support in all browsers and will render on screen but the canvas content will not be accessible to screen readers.
- By default the chart's canvas will use a 1:1 pixel ratio, unless the physical display has a higher pixel ratio
- Scriptable options also accept a function which is called for each of the underlying data values and that takes the unique argument context representing contextual information 
- Indexable options also accept an array in which each item corresponds to the element at the same index.
- Chart.js charts are rendered on canvas elements, which makes rendering quite fast.
- The onProgress and onComplete callbacks are useful for synchronizing an external draw to the chart animation. 
- If this value is a number, it is applied to all sides of the chart (left, top, right, bottom). If this value is an object, the left property defines the left padding. Similarly the right, top and bottom properties can also be specified.
- Axes are an integral part of a chart. They are used to determine how data maps to a pixel value on the chart. In a cartesian chart, there is 1 or more X axis and 1 or more Y axis to map points onto the 2 dimensional canvas.
- When adding new axes, it is important to ensure that you specify the type of the new axes as default types are not used in this case.
- The linear scale is use to chart numerical data. It can be placed on either the x or y axis.
- logarithmic interpolation is used to determine where a value lies on the axis.
- Radial axes are used specifically for the radar and polar area chart types.

## Vocab
- Responsive defines responsive chart options that apply to all charts.
- Device Pixel Ratio defines the ratio between display pixels and rendered pixels.
- Interactions defines options that reflect how hovering chart elements works.
- Options scriptable and indexable options syntax.
- Colors defines acceptable color values.
- Font defines various font options.
- Performance gives tips for performance-sensitive applications.

# Basic usage

## Notes
- The <canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.

# Drawing shapes with canvas

## Notes
- <canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths
- Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.
- A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. 

#### Steps to make shapes
1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.

#### Functions for the steps
1. beginPath()
- Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
2. Path methods
- Methods to set different paths for objects.
3. closePath()
- Adds a straight line to the path, going to the start of the current sub-path.
4. stroke()
- Draws the shape by stroking its outline.
5. fill()
- Draws a solid shape by filling the path's content area.



# Applying styles and colors

## Notes
- drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

#### Styles Lines
1. lineWidth = value
- Sets the width of lines drawn in the future.
2. lineCap = type
- Sets the appearance of the ends of lines.
3. lineJoin = type
- Sets the appearance of the "corners" where lines meet.
4. miterLimit = value
- Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
5. getLineDash()
- Returns the current line dash pattern array containing an even number of non-negative numbers.
6. setLineDash(segments)
- Sets the current line dash pattern.
7. lineDashOffset = value
- Specifies where to start a dash array on a line.

- The lineJoin property determines how two connecting segments (of lines, arcs or curves) with non-zero lengths in a shape are joined together

#### Possible values for this property
1. round
- Rounds off the corners of a shape by filling an additional sector of disc centered at the common endpoint of connected segments. The radius for these rounded corners is equal to half the line width.
2. bevel
- Fills an additional triangular area between the common endpoint of connected segments, and the separate outside rectangular corners of each segment.
3. miter
- Connected segments are joined by extending their outside edges to connect at a single point, with the effect of filling an additional lozenge-shaped area.

- The miterLimit property determines how far the outside connection point can be placed from the inside connection point.

#### Types of patterns
1. repeat
- Tiles the image in both vertical and horizontal directions.
2. repeat-x
- Tiles the image horizontally but not vertically.
3. repeat-y
- Tiles the image vertically but not horizontally.
4. no-repeat
- Doesn't tile the image. It's used only once.

#### 4 properties of shadows
1. shadowOffsetX = float
- Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
2. shadowOffsetY = float
- Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
3. shadowBlur = float
- Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
4. shadowColor = color
- A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.

# Drawing text

## Notes
#### 2 methods to drawing text
1. fillText(text, x, y [, maxWidth])
- Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
2. strokeText(text, x, y [, maxWidth])
- Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

#### styleing text(not the only ones)
1. font = value
- The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
2. textAlign = value
- Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
3. textBaseline = value
- Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
4. direction = value
- Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

#### Measuring text
1. measureText()
- Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.
