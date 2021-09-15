# Cálculo de parámetros dinámicos con FreeCAD

Para determinar los parámetros de la dinámica (masa y momento de inercia) de las diferentes partes del robot se utiliza el complemento [FCInfo](https://wiki.freecadweb.org/Macro_FCInfo) de FreeCAD.

## Instalación

  1. Abrir el administrador de complementos: _"Tool --> Addon manager"_.
  1. En la pestaña _"Macros"_ buscar _"FCInfo"_ e instalar el complemento.


Nota:
En la versión 0.18.4 de FreeCAD el administrador de complementos se bloquea y no muestra el listado de macros a instalar. Una forma de corregir este error se muestra en [Addons wizard stuck retrieving info from wiki](https://www.reddit.com/r/FreeCAD/comments/ijgo2q/addons_wizard_stuck_retrieving_info_from_wiki/?utm_name=Bing).

## Uso de la macro `FCInfo`

Para determinar los parámetros de la dinámica de una pieza se deben aplicar los siguientes pasos:

  1. Abrir el archivo del diseño de la pieza.
  1. Del menú _"Macro"_ elegir la opción _"Macros..."_.
  1. Ejecutar la macro _"FCInfo.FCMacro"_.
  1. Seleccionar la pieza a la cual se le quieren calcular los parámetros.
  1. En la sección _"Surface and Volume"_ cargar la densidad del material (2.7 Kg/dm3 para el aluminio y 7.5 Kg/dm3 para el hierro).

