This package demonstrates segmentation methods using 2D/3D data streams.  Segmentation is the process by which foreground objects are separated from the background or the method by which objects of interest are grouped.  The following sections describe specific demos and provide instructions for their use

* Industrial Segmentation Demo - Tabletop segmentatoin routine utilizing a kinect-like sensor(modified to be standalone).  The tabletop segmentation routines assume a flat surface is present in the scene.  The algorithms identify the tabletop and then perform cluster analysis on objects immediately above the tabletop.

  In terminal 1, launch the demo:
  ```
  roslaunch industrial_demo_segmentation industrial_segmentation_demo.launch
  ```

  In terminal 2, call the segmentation service from the command line:

  ```
  rosservice call /tabletop_segmentation "table: {}" 
  ```
