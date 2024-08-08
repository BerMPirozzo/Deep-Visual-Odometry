# Deep-Visual-Odometry

Para poder utilizar este modelo de CNN lo que se necesita es:

1) Descargar el entorno de https://github.com/Gastd/p3at_tutorial.

2) Agregar la cámara monocular a este modelo.

3) Ejecutar en terminales diferentes:

   a) Nodo maestro.
   
   b) entorno pioneer3at.gazebo.launch.
   
   c) move_base_mapless_demo.launch.

   d) Ejecutar gmapping.

   e) Abrir el modelo de la CNN y darle como entrada la imagen monocular color de la cámara publicada en el tópico /pioneer3at/camera/image_raw.

   f) Publicar el archivo poses.csv en el tópico /waypoint_markers.
