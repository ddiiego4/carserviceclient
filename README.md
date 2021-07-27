NOMBRE DE LA INTEGRACIÓN O DEL API

DUEÑO FUNCIONAL DE LA SOLUCIÓN

Área	Nombre del área dueña de la solución
Contacto	Nombre del responsable por origen
Nombre del responsable por destino

Tabla de contenido
Descripción de la necesidad
Diagrama de la necesidad
Clasificacion de las Interfaces
Atributos de calidad de la solucion
Diagrama de componentes de la Interfaz
Consideraciones
Mapeo de datos
	Mapeo Estructura1
	Mapeo Estructura2
	Mapeo Estructura3	
Características técnicas de la Interfaz
Manejo de Errores
Manejo de reproceso
Manual de despliegue
Inventario de Artefactos
Topologías
Directorios
Operaciones de la Interfaz (Servicio)


Descripción de la necesidad
En esta sección, se debe especificar cual es la necesidad del negocio que se quiere solucionar, para describir la necesidad de acuerdo a los siguientes ítems:

Nombre de la interfaz:	NOMBRE DE LA INTERACIÓN O API
Qué	Especifique la necesidad que se quiere solucionar
Porqué	Especifique el por qué se necesita solucionar la necesidad
Para que	Especique el objetivo que se desea alcanczar con la solución a implementar.
Diagrama de la necesidad
A continuación mostramos algunos ejemplos:

Diagrama

Diagrama

Especifique las notas puntales que sean relevantes para el proceso.
Identifique las integraciones del diagrama de la necesidad y defina cuales están al alcance de este desarrollo.
Una vez identificadas las integraciones dentro del alcance, defina una breve descripción de estas integraciones.
Clasificación de las Interfaces
Atributos de calidad de la solución
Estas preguntas se puedes realizar enfocadas en el proceso de negocio que se está analizando para identificar los atributos de calidad:

¿Con qué frecuencia se generan los mensajes o registros en un día?
¿Qué cantidad de registros o mensajes se generan?
¿Cuál es el crecimiento esperado para la generación de estos registros o mensajes?
¿Cuánto tiempo se necesita para ejecutar el proceso?
¿Cuál es el tiempo en que se espera tener la información?
¿Cómo se comporta la información en un evento especial? En promociones, un día, hora en particular?
En la siguiente tabla se relacionan los atributos de calidad asociados a la solución:

Seguridad		
Característica	Observación	
Identificación y Autenticación		
Autorización		
Confidencialidad		
Integridad		
Auditabilidad		
Desempeño		
Característica	Observación	
Transacciones por Segundo		
Tiempo de Respuesta Máximo en Segundos		
Tiempo de Respuesta Promedio en Segundos		
Frecuencia		
Registros entregados en orden		
Escalamiento		
Característica	Observación	
Cantidad Estimada de Transacciones por Día/Mes/Año		
Porcentaje de Crecimiento Estimado de Transacciones por Día/Mes/Año (%)		
Disponibilidad		
Característica	Observación	
Horario de Disponibilidad de la Solución		
Contingencia		
Manejo de errores		
Característica	Observación	
Trazabilidad		
Endpoint o Partition Key		
Errores		
Alertamiento		
Monitoreo		
Reintentos		


Diagrama de componentes de la Interfaz
En el siguiente diagrama de componentes se muestra el diseño de la integración y la relación con los diferentes componentes: Diagrama ejemplo para ODI:

Diagrama

Diagrama ejemplo para Azure:

Diagrama

Nombre Componente	Descripción del componente	Responsabilidad	Tipo	Herramienta

Consideraciones
​ En esta sección especificar las consideraciones relevantes de la solución a construir.

Este diagrama no es necesario cuando se construye un servicio simple, se crearía el diagrama de secuencia.
Este diagrama debe contemplar el reproceso de la información y el punto desde donde reenviaría la información.
Especificar si es una cola, un servicio que se debe definir.
Mapeo de datos
En las siguientes tablas se relacionan el mapeo de datos entre el mensaje interno capa integración y el mensaje de los proveedores de la Interfaz:

Mapeo de datos				
Nombre del componente: escriba el nombre del componente				
Nombre Del destino: especifique el nombre del componente destino				
Enrutamiento: /				
Campo Destino	Transformación	Origen	Campo Origen	Comentarios
nombre campo destino 1	tipo de transformación	Tipo campo origen 1	Nombre campo origen 1	Especifique algun comentario releventa del campo
Características técnicas de la Interfaz
Las hojas técnicas de infraestructura son relacionadas en la siguiente tabla:

Características Técnicas Desarrollo						

Características Técnicas Calidad						


Esta integración esta orquestada por XXXX:

Parámetros XXXX			
Nombre de la Malla	
Tipo de Ejecución	Secuencial		
Frecuencia	Diario - 8:00 am - 12:00 pm - 5:00 pm		
Escenario	Proyecto	Fuente	Destino

Manejo de Errores
Si/No	Cómo se realiza

Reintentos	Si	Se ejecuta de nuevo el proceso manualmente desde XXXX
Trazabilidad	Si	En la tabla TBL
Contingencia	No	
Manejo de reproceso
Especificar los puntos en que se debe hacer el reproceso y cómo hacerlo.

Punto	Como se reprocesa	Aplicabilidad

Las siguientes operaciones serán ofrecidas por el servicio:

Nombre de la operación
Especificar que realiza la operación.

Mensajes de la Operación	
Descripción del mensaje origen	Descripción del mensaje destino
Especifique el mensaje origen	Especifique el mensaje destino o respuesta
Especifique un ejemplo de como consumir el servicio y cual seria la respuesta

Mensajes de la interfaz
Mensaje en el origen
