# drawer
An app for drawing, importing and exporting doodles

# general
Note: This project is mainly intended for practicing and experimenting with architectural concerns of small projects.

# main elements

# initialization/ setup
- Import createDrawer function
- Create an instance of Drawer by using createDrawer(<Id of Dom Element>)
- Instances of Drawer provide following functions which are intended to serve as callbacks for Event Handlers for Control Elements:
  - setDrawingModeCreateFreehandLine
  - setDrawingModeCreateSquare
  - setDrawingModeCreateRectangle
  - setDrawingModeCreateCircle
  - setDrawingModeRemoveLatest
  - exportSVG
  - importSVG

# classes (overview for dev purposes)
