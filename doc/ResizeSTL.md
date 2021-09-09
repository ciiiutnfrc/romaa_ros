# Redimensionar archivo de malla en formato STL

Los archivos de malla en formato `stl` que se exportan desde FreeCAD están afectado
por un factor de escala de 1000. Gazebo necesita que la unidad sea el metro y FreeCAD
exporta los archivos en milímetros.
Para redimensionar el archivo `stl` se puede utilizar Blender.

Los pasos a seguir son:
  1. Desde Blender importar el archivo `stl` a redimensionar.
  1. Con el objeto seleccionado buscar en la paleta de la derecha la sección 'Transform'.
  1. Dividir por 1000 la escala en las coordenadas X, Y y Z.
  1. Exportar el archivo en formato `stl`.


Nota:
  * La versión de FreeCAD utilizada para exportar la malla es la 0.18.4
  * La versión de Blender para redimensionar la malla es la 2.82
