# Paquetes de ROS para el robot RoMAA

> :memo: El repositorio `romaa_ros` con el driver del robot RoMAA fue renombrado a `romaa_driver` ([link](https://github.com/ciiiutnfrc/romaa_driver))


## Visualización del modelo URDF en RViz

Para visualizar el model URDF del robot ejecutar:
```
roslaunch romaa_description romaa_rviz.launch
```

## Simulación en Gazebo

Para cargar el modelo del robot en el simulador Gazebo hay que ejecutar:
```
roslaunch gazebo_ros empty_world.launch
roslaunch romaa_gazebo spawn_xacro.launch
```

## Verificación del modelo

  * Obtener el archivo `.urdf` a partir del `.xacro`: `> xacro romaa.xacro > romaa.urdf`
  * Verificar URDF: `> check_urdf <urdf_file>`
  * Visualizar URDF: `> urdf_to_graphiz <urdf_file>`

Otra verificaciones:
  * Imprimir modelo p/Gazebo: `> gz sdf -p romaa.urdf`
  * Verificar modelo p/Gazebo: `> gz sdf -k romaa.urdf`


## Documentación

  * [Redimensionar archivo de malla en formato STL](doc/ResizeSTL.md)
  * [Cálculo de parámetros dinámicos con FreeCAD](doc/FreeCADFCInfo.md)
  * [Modelo de simulación en Gazebo](doc/GazeboModel.md)

