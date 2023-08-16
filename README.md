The Scribble example shows how to reimplement some of QWidget's event handlers to receive the events generated for the application's widgets.

We reimplement the mouse event handlers to implement drawing, the paint event handler to update the application and the resize event handler to optimize the application's appearance. In addition we reimplement the close event handler to intercept the close events before terminating the application.

The example also demonstrates how to use QPainter to draw an image in real time, as well as to repaint widgets.

![image](https://github.com/ashish182229/Paint-Software/assets/66489551/39a9ee53-a0ad-4de9-a4a0-29c61408dadf)

With the Scribble application the users can draw an image. The File menu gives the users the possibility to open and edit an existing image file, save an image and exit the application. While drawing, the Options menu allows the users to choose the pen color and pen width, as well as clear the screen. In addition the Help menu provides the users with information about the Scribble example in particular, and about Qt in general.

The example consists of two classes:

ScribbleArea is a custom widget that displays a QImage and allows to the user to draw on it.
MainWindow provides a menu above the ScribbleArea.
We will start by reviewing the ScribbleArea class. Then we will review the MainWindow class, which uses ScribbleArea.

