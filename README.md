# Project-Yolo_objec_dect_video
ELEC-4555-Computer-Vision-Project

Objective:
The objective of this project is to be able to detect users utilizing desks and tables in public spaces. Due to COVID it is ever more important to keep desks clean and this system would be able to recognize if a table has been used. Examples of its use include in classroom areas, common areas, labs, and auditoriums. The program should be able to detect and track users and recognize if they are using a desk. Users of public spaces will be able to know when a table is clean and ready to use and cleaning staff will be able to clean more efficiently. This will be impactful to the current COVID situation by improving awareness and cleaning process and efficiency.
What to investigate

Detection method:
YOLO Object detection with OpenCV
Yolo is a one stage detector with real time tracking, which allow us to track object with 45 fps in a video. We choose YOLO instead of RCNN because YOLO is substantially faster and allow us to track people interacting with table in real time. Thus, we can see if a table has been used and whether it's in need of cleaning/sanitizing.

Tracking method:
1. Determine the object type, what type of object is it? (person, car, cat, table etc...), for the same type of object (Ex: multiple people or desk). We will assign each of them with induvial ID for better tracking.
2. Pick out two of the specific objects we want to track, in this case person and table.
3. Set a distance parameter for safe and not safe. Example, if a person approaches a table within certain distance, we could determine that the table has been used and it's in needs of cleaning. Vice versa, if the person is out of the “non safe zone” the table is not used and therefore no need to be clean.

References:
https://www.pyimagesearch.com/2018/11/12/yolo-object-detection-with-opencv/
https://stackoverflow.com/questions/44674517/yolo-darknet-detecting-only-specific-class-like-person-cat-dog-etc
https://pysource.com/2019/06/27/yolo-object-detection-using-opencv-with-python/
https://www.youtube.com/watch?list=PLrrmP4uhN47Y-hWs7DVfCmLwUACRigYyT&v=NM6lrxy0bxs

Dataset:
https://cocodataset.org/
PIROPO Database-Room B(with people leave the table and approaching table)
Lab_Database- Lab room setting(With student entering their desk and leaving the room)
Visor Data set- Videos of people sitting on a chair
HMDB-Human motion Data set
HOLLYWOOD2-Human Actions and Scenes Dataset
