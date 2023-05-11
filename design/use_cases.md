# Casos de usos

Existen dos tipos de usuarios de la aplicación

1. Usuario cliente final: que apartir de ahora será llamado solo __cliente__. Este  cliente hace referencia a los clientes propios de las instituciones que emplean la aplicacion, 

2. Usuario cliente institucional: a partir de ahora sera llamado __usuario__. Hace referencias a los usuarios registrados por la institucion que adquirio la aplicacion __TurNow__, los cuales tienen distintos tipos de acceso y roles dentro de esta.

***
## Cliente => Casos de uso

- El cliente puede solicitar un turno de forma presencial para ser atendido segun su necesidad y acorde a la estructura de turnos establecidas por la institucion.

- El cliente puede visualizar en una pantalla que turnos estan siendo atendidos en el momente y en que modulo se encuentran. En la misma pantalla podra visualizar cuando su turno sea asignado a un modulo.

- El cliente puede solicitar la cancelacion del turno en caso de que no puede esperar la atencion correspondiente


### casos de uso No Soportados

- El cliente no podra solicitar un turno por fuera de las oficinas fisicas ni de forma virtual.

- El cliente no podra solicitar reprogramar su turno en caso de que no se encuentra presente al momento de su asignacion

- El cliente no podra pedir mas de un turno para su atencion.

*** 
## Usuario => Casos de uso
  * Rol gerente:
    - puede ver estadísticas diarias, semanales y/o mensuales de la cantidad de turnos atendidos, categorias de turnos, tiempos de esperas, prioridades de atencion, tiempo de atencion en modulo, entre otros. Las estadisticas no son en tiempo real y se generan diariamente una vez finalizada la jornada laboral.
    
  * Rol administrador:
    - Puede crear categorias para los distintos tipos de servicios prestados y clientes.
    - Puede definir la prioridad de los clientes (tercer edad, discapacidad, etc, clientes registrados o no registrados)
    - Puede configurar los distintos módulos de atención y asignarles las distintas categorias de servicio con sus respectivas prioridades de atencion.
    - Puede configurar los horarios de atención en jornada normal y/o festivos.      
    - Puede agregar nuevos módulos de atención
    - Puede asignar permisos a otros usuarios en función de su rol

  * Rol gestor o facilitador:
    - Puede reiniciar el conteo de turnos si es necesario.
    - Puede eliminar los registros de usuarios si lo requiere.
    - Puede asignar turnos a un cliente
    - Puede reasignar un cliente de modulo en caso de ser necesario.
    - Puede de asignar prioridades a los turnos en tiempo real 
    - Puede ver notificaciones sobre tiempos de espera de clientes cuando esten proximos a ser antendidos.

  * Rol modulo:
    - El usuario módulo puede ver en una pantalla los turnos actuales que se deben atender en ese módulo, y marcarlos como atendidos una vez que hayan sido atendidos.
    - El usuario módulo también puede reasignar un turno a otro módulo si es necesario, por ejemplo, si el servicio que el usuario necesita no se puede proporcionar en ese módulo específico.

  * Rol visual:
    - El usuario solo puede acceder a la pantalla de visualizacion de turnos para proyectarla en un monitor.
