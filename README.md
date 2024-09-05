# drawer
An app for drawing, importing and exporting doodles

# general
Note: This project is mainly intended for practicing and experimenting with architectural concerns of small projects.

# main elements

# initialization/ setup
- Import createDrawer function
- Create an instance of Drawer by using createDrawer(<Id of Dom Element>)
- Instances of Drawer provide following functions which are intended to serve as   

# classes (overview for dev purposes)

## Drawer
Representation of Drawer. Serves as API. Functions can be used as callbacks for eventHandlers on control elements like cuttons etc.
- setDrawingModeCreateFreehandLine
- setDrawingModeCreateSquare
- setDrawingModeCreateRectangle
- setDrawingModeCreateCircle
- setDrawingModeRemoveLatest
- exportSVG
- importSVG

## Board
Main User Interface.
- switchToFreehandlineMode
- switchToAddShapeMode
- switchToMoveShapeMode
- switchToRotateShapeMode
- drawSVG
- handleMouseDown
- handleMouseMove
- handleMouseUp

## Geometry
Manages drawn elements.
- addElement
- removeLatestElement

## SVGSerializer
Serializes Geometry Information to SVGCode
- serializeGeometryToSVG

## SVGParser
Generates Geometry Information from SVGCode

## DrawingModeFreehandLine
## DrawingModeSquare
## DrawingModeRectangle
## DrawingModeCircle
- name (str)
- handleControlDown
- handleControlUp
- handleControlMove

## FreehandLineFactory
## SquareFactory
## RectangleFactory
## CircleFactory
- make

## FrehandLine
- verticesCoordinates (arr)
- extend

## Rectangle
- baseCoordinates (num, num)
- width (num)
- height (num)
- rotation (num)
- setWidth
- setHeight
- setRotation
