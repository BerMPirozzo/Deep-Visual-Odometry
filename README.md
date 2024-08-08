# Deep-Visual-Odometry

Para poder utilizar este modelo de CNN lo que se necesita es:

1) Descargar el entorno de https://github.com/Gastd/p3at_tutorial.

2) Agregar la cámara monocular a este modelo siguiendo los pasos indicados para agregar sensores en la página oficial de ROS. Además colocar al robot en las siguientes coordenadas, con la siguiente orientación:
   x =-9,y=-9, Yaw= 0.0.

4) Ejecutar en terminales diferentes:

   a) Nodo maestro.
   
   b) Entorno: pioneer3at.gazebo.launch.
   
   c) Move Base: move_base_mapless_demo.launch.

   d) Ejecutar el nodo gmapping.

   e) Abrir el modelo de la CNN y darle como entrada la imagen monocular color de la cámara publicada en el tópico /pioneer3at/camera/image_raw.

   f) Publicar el archivo poses.csv en el tópico /waypoint_markers e iniciar el server de move_base para que elija la opción a seguir tal que el robot se desplace.
