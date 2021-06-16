Object detection using YOLOv4 :
-------------------------------
 in this project we tried with 6 classe acctualy you can do whatever you want darknet is open source and performant, in this case we have 6  classes {masque, mal_mis, velo, trottinette , pas_de_masque)

2_Create_labels(1)
------------------
  1) the first step is getting data
  2) make some anotation on it identify the nember of classes you can use VGG anotator for that
  3) and the we do some data cleaning using panda
  4) and than we split the data in 2 part 0.75 for train and 0.25 for test or validation 

yolov4_myProject_(2)
--------------------

  1) make sure that you have GPU, openCV and darknet 
  2) and after that you can start training the model 
  3) get predections and save it in csv files .csv in please remember that you can do anything in our case we did 3 types of submissions the first one  (pieton,masque,mal_mis) second one (trottinette,velo) le trosieme (pieton,velo)
  
test with images 
-----------------

![143923142_423536878890375_1162483937575691006_n](https://user-images.githubusercontent.com/74276606/106903837-ccdfac80-66fa-11eb-834e-c5df5b95be52.gif)
#
## test with videos
!./darknet detector demo /content/drive/MyDrive/YOLOV4-multi-data/data_names/project.data /content/drive/MyDrive/YOLOV4-multi-data/cfg/yolov4.cfg /content/drive/MyDrive/YOLOV4-multi-data/weights/yolov4_last.weights -dont_show /content/drive/MyDrive/YOLOV4-multi-data/my_test_video/5_clip.mp4 -i 0 -out_filename /content/drive/MyDrive/YOLOV4-multi-data/my_test_video/results.avi
