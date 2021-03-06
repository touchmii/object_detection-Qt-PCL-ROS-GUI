# Software guide

### wangzi

1. **cpp class**
(diff cpp files)

* Qtdisplay class
  Param     class
* PCL       class
* pcl_io    class
* ROS       class
* Recog     class
* Socket  class

2. **Dialog**
* point cloud display window 	  <left up big>
* detailed display window 	  <left down small>
* param window 			  <right up rect>
* information text display window <right down long>

3. **Timeline**
* setup ros_qt basic env  		<done>
* basic implement of PCL and RealSense	<done>
* Vision of point cloud			<done> 

```
  -- remain : 
  QVTKwidget(PLC_qt_visualizer_tutorial)  librviz(testRVIZ)  //openGL
  thing about it, is it have to use ROS, also the rviz topic manage.
  what's the step of QVTKwidget. this should be more convenient.
  -- seems :
  there is a simple way to use vtkQwidget if you have install VTK5.x
  just need to include the related headfile and Qwidget inhert QVTKWidget
  detach it to a layout then you can make it.
```

* Class setup of pointcloud class       <done>
* Param class				<done>
* GUI Interface setup			<done>
* Makeup 				<done>

4. **Feature**
* class orientation	<done>
* scalable<optional>  	<done>
* Exception handling	<doing>

5. **cpp discription**
* gui<done>
   ├─ pointcloud vtkwidget
   ├─ infoprint widget
   ├─ param widget(multipage)
   ├─ subview widget
* qrealsense<done>
   ├─ rs receive/config
   ├─ return frame
   ├─ pcd file read/store
* basic<done>
   ├─ publish final info in qt
   ├─ receive and printout in receive node
* qvtk<done>
   ├─ update pointcloud display
   ├─ add pointcloud display
   ├─ display config - colour visable size
* qpcl<done>
   ├─ pointcloud preprocess<done>
   ├─ keypoint extract<done>
   ├─ segmentation<done>
   ├─ normal estimation<done>
   ├─ feature compute<done>
   ├─ surface reconstruct<done> -- *MLS
   ├─ alignment<done> -- *RANSAC *SACIA
   ├─ registration<done> -- *NDT *ICP
   ├─ diff feature same reco<doing> -- *shot352 *fpfh
* socket<done>
   ├─ image transform between python and C++
* system<taking>
   ├─ pointcloud interface<done>
   ├─ poincloud realsense<done> -- *continuning_play *multi_processing 
   ├─ param editting<done>
   ├─ Pointcloud mask<done>
   ├─ error catching 
   ├─ documental work<done>
* gezabo<taking>
   ├─ UR5 physical implement
   ├─ UR5 control API
   ├─ kinetic sensor implement
   ├─ environment&object body setup






