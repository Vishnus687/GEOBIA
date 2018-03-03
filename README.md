Introduction
  Object-Based Image Analysis (OBIA) employs two main processes, segmentation and classification. Traditional image segmentation is on a     per-pixel basis. However, OBIA groups pixels into homogeneous objects. These objects can have different shapes and scale. Objects also     have statistics associated with them which can be used to classify objects. Statistics can include geometry, context and texture of       image objects.When applied to earth images, OBIA is known as Geographic Object-Based Image Analysis (GEOBIA).

Objective
  Finding area using Object Based Image Analysis(OBIA)

Resources:-Sample Data:-Landsat-8 imagery(GeoTiff) and Shapefiles for training
Source:-Planet Labs(Planet.com),Earth Explorer
  ->Resolution:-30m
  ->Shape files for training which can be created using QGIS tool.
   

Description(Steps)
1.Step1-Classification
Classifying into 2 classes Green fields and Freshly ploughed fields (mostly brown) using OBIA(Classification)
2.Step2-Segmentation
3.Step3-Training
 ->Training using shapefiles
 ->No of  shape files created for training:-2
 ->No of classes :-2(Green and Brown)
4.Step4-Finding Area
 ->Calculated total number of pixels for each class.
 ->Since it is a 30m resolution image area per pixel is calculated by (pixel value*30*30)
 ->Calculated area for each class using (pixel value*30*30)/1000 KM.
 
 
 
