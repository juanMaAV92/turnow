# Turnow

* __Resumen__

...

* __Objetivo__

Diseñar una aplicación de gestión de turnos genérica para facilitar y optimizar la atención y/o prestacion de servicios en distintos tipos de organizaciones o empresas, permitiendo una mejor organización, control y atención a los usuarios o clientes.

* __Espectativas__

Permitir un mayor control: La aplicación proporcionará una mejor visibilidad y control de la programación de turnos, lo que puede ayudar a las organizaciones a planificar mejor sus recursos y optimizar la atención.

Mejorar la eficiencia en la atención: La aplicación puede permitir una mejor gestión de los turnos y citas, lo que ayuda a las organizaciones a prestar servicios de manera más eficiente.

Ofrecer una experiencia de usuario mejorada: Una aplicación bien diseñada puede proporcionar una experiencia de usuario atractiva y fácil de usar, lo que puede aumentar la adopción y el uso de la aplicación

Incrementar la satisfacción de los usuarios: Al mejorar la eficiencia en la atención y que los turnos se asignen de una manera más fácil y rápida, puede aumentar la satisfacción de los usuarios finales.

* __Alcance__

La aplicación permitirá la asignación de turnos en forma presencial en establecimientos de atención al usuario:  como Bancos, centros de salud, laboratorios clinicos, etc.

Se podrá configurar y asignar distintas categorias de turnos dependiendo del tipo de servicio a solicitar o de la prioridad (dada por la organización).

La aplicación debe contar con una pantalla para la solicitud del turno por parte del usuario final; una pantalla para visualizar el turno actual y el modulo de atencíon a donde se debe dirigir el usuario; una pantalla para la administración de turnos; una pantalla para atender un turno en un modulo especifico. 


* __Solución propuesta y alternativa__


* __Casos de uso a soportar__

  * Usuario final:
      - El usuario solicita un turno para ser atendido segun la clasificación de tipo de usuario.
      - El usuario visualiza su nombre en la pantalla de espera para saber el momento en que podrá pasar a ser atendido.
      - El usuario obtiene un mensaje de error en caso de que su registro no se haya realizado con exito y podrá intentarlo nuevamente.
      - El usuario obtiene un mensaje de advertencia cuando ya se haya llegado al límite de turnos en el día.
  
  * Usuario modulo:
  
  * Usuario Administrador:
      - El administrador crea categorias para los tipos de usuario segun su modelo de atención.
      - El administrador limita el numero de turnos a otorgar.
      - El administrador reinicia el conteo de turnos si es necesario.
      - El administrador elimina los registros de usuarios si lo requiere.
  
  * Usuario Organización:
  
* __Out of Scope (casos de uso No Soportados)__
  - Como usuario me gustaría tomar un turno estando fuera del establecimiento fisico

* __Arquitectura__

  * SO: Linux o Windows
  * Tipo de aplicación: WEB
    * Backend: Python (DJango)
    * Frontend: HTML + JavaScript + CSS; servidos por DJango como estaticos
  * Base de datos: PostgreSQL, ORM: SQLAlchemist
  * Modelo de datos:
  	- Diseño de entidades:
  		

  	


* __Limites__
	- La base de datos guardará un numero limitado de registros en el tiempo.
	- Solo podrá registrarse un usuario a la vez

