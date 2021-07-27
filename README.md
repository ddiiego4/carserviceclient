NOMBRE DE LA INTEGRACION O DEL API

DUENO FUNCIONAL DE LA SOLUCION

area	Nombre del area duena de la solucion
Contacto	Nombre del responsable por origen
Nombre del responsable por destino

Tabla de contenido
Descripcion de la necesidad
Diagrama de la necesidad
Clasificacion de las Interfaces
Atributos de calidad de la solucion
Diagrama de componentes de la Interfaz
Consideraciones
Mapeo de datos
	Mapeo Estructura1
	Mapeo Estructura2
	Mapeo Estructura3	
Caracteristicas tecnicas de la Interfaz
Manejo de Errores
Manejo de reproceso
Manual de despliegue
Inventario de Artefactos
Topologias
Directorios
Operaciones de la Interfaz (Servicio)


Descripcion de la necesidad
En esta seccion, se debe especificar cual es la necesidad del negocio que se quiere solucionar, para describir la necesidad de acuerdo a los siguientes items:

Nombre de la interfaz:	NOMBRE DE LA INTERACION O API
Que	Especifique la necesidad que se quiere solucionar
Porque	Especifique el por que se necesita solucionar la necesidad
Para que	Especique el objetivo que se desea alcanczar con la solucion a implementar.
Diagrama de la necesidad
A continuacion mostramos algunos ejemplos:

Diagrama

Diagrama

Especifique las notas puntales que sean relevantes para el proceso.
Identifique las integraciones del diagrama de la necesidad y defina cuales estan al alcance de este desarrollo.
Una vez identificadas las integraciones dentro del alcance, defina una breve descripcion de estas integraciones.
Clasificacion de las Interfaces
Atributos de calidad de la solucion
Estas preguntas se puedes realizar enfocadas en el proceso de negocio que se esta analizando para identificar los atributos de calidad:

Con que frecuencia se generan los mensajes o registros en un dia
Que cantidad de registros o mensajes se generan
Cual es el crecimiento esperado para la generacion de estos registros o mensajes
Cuanto tiempo se necesita para ejecutar el proceso
Cual es el tiempo en que se espera tener la informacion
Como se comporta la informacion en un evento especial En promociones, un dia, hora en particular
En la siguiente tabla se relacionan los atributos de calidad asociados a la solucion:

Seguridad		
Caracteristica	Observacion	
Identificacion y Autenticacion		
Autorizacion		
Confidencialidad		
Integridad		
Auditabilidad		
Desempeno		
Caracteristica	Observacion	
Transacciones por Segundo		
Tiempo de Respuesta Maximo en Segundos		
Tiempo de Respuesta Promedio en Segundos		
Frecuencia		
Registros entregados en orden		
Escalamiento		
Caracteristica	Observacion	
Cantidad Estimada de Transacciones por Dia/Mes/Ano		
Porcentaje de Crecimiento Estimado de Transacciones por Dia/Mes/Ano (%)		
Disponibilidad		
Caracteristica	Observacion	
Horario de Disponibilidad de la Solucion		
Contingencia		
Manejo de errores		
Caracteristica	Observacion	
Trazabilidad		
Endpoint o Partition Key		
Errores		
Alertamiento		
Monitoreo		
Reintentos		


Diagrama de componentes de la Interfaz
En el siguiente diagrama de componentes se muestra el diseno de la integracion y la relacion con los diferentes componentes: Diagrama ejemplo para ODI:

Diagrama

Diagrama ejemplo para Azure:

Diagrama

Nombre Componente	Descripcion del componente	Responsabilidad	Tipo	Herramienta

Consideraciones
​ En esta seccion especificar las consideraciones relevantes de la solucion a construir.

Este diagrama no es necesario cuando se construye un servicio simple, se crearia el diagrama de secuencia.
Este diagrama debe contemplar el reproceso de la informacion y el punto desde donde reenviaria la informacion.
Especificar si es una cola, un servicio que se debe definir.
Mapeo de datos
En las siguientes tablas se relacionan el mapeo de datos entre el mensaje interno capa integracion y el mensaje de los proveedores de la Interfaz:

Mapeo de datos				
Nombre del componente: escriba el nombre del componente				
Nombre Del destino: especifique el nombre del componente destino				
Enrutamiento: /				
Campo Destino	Transformacion	Origen	Campo Origen	Comentarios
nombre campo destino 1	tipo de transformacion	Tipo campo origen 1	Nombre campo origen 1	Especifique algun comentario releventa del campo
Caracteristicas tecnicas de la Interfaz
Las hojas tecnicas de infraestructura son relacionadas en la siguiente tabla:

Caracteristicas Tecnicas Desarrollo						

Caracteristicas Tecnicas Calidad						


Esta integracion esta orquestada por XXXX:

Parametros XXXX			
Nombre de la Malla	
Tipo de Ejecucion	Secuencial		
Frecuencia	Diario - 8:00 am - 12:00 pm - 5:00 pm		
Escenario	Proyecto	Fuente	Destino

Manejo de Errores
Si/No	Como se realiza

Reintentos	Si	Se ejecuta de nuevo el proceso manualmente desde XXXX
Trazabilidad	Si	En la tabla TBL
Contingencia	No	
Manejo de reproceso
Especificar los puntos en que se debe hacer el reproceso y como hacerlo.

Punto	Como se reprocesa	Aplicabilidad

Las siguientes operaciones seran ofrecidas por el servicio:

Nombre de la operacion
Especificar que realiza la operacion.

Mensajes de la Operacion	
Descripcion del mensaje origen	Descripcion del mensaje destino
Especifique el mensaje origen	Especifique el mensaje destino o respuesta
Especifique un ejemplo de como consumir el servicio y cual seria la respuesta

Mensajes de la interfaz
Mensaje en el origen
