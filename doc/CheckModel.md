# Verificación del modelo

Para verificar el modelo `xacro` se pueden utilizar las siguientes herramientas:
  * Obtener el archivo `.urdf` a partir del `.xacro`: `> xacro romaa.xacro > romaa.urdf`
  * Verificar URDF: `> check_urdf <urdf_file>`
  * Visualizar URDF: `> urdf_to_graphiz <urdf_file>`

Otra verificaciones:
  * Imprimir modelo p/Gazebo: `> gz sdf -p romaa.urdf`
  * Verificar modelo p/Gazebo: `> gz sdf -k romaa.urdf`

