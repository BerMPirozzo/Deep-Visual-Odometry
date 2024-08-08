# Deep-Visual-Odometry

Para poder utilizar este modelo de CNN lo que se necesita es:

1) Descargar el entorno de https://github.com/Gastd/p3at_tutorial.

2) Agregar la cámara monocular a este modelo.

3) Ejecutar:
   
   a) entorno pioneer3at.gazebo.launch
   
   b) move_base_mapless_demo.launch

   c) Ejecutar gmapping

   d) Abrir el modelo de la CNN y darle como entrada la imagen monocular color de la cámara publicada en el tópico /pioneer3at/camera/image_raw

   e) Publicar el archivo poses.csv en el tópico /waypoint_markers 
