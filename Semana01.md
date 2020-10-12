Ejercicio 1
Buscar una aplicación de ejemplo, preferiblemente propia, y deducir qué patrón es el que usa. ¿Qué habría que hacer para evolucionar a un patrón tipo microservicios?

La aplicación que elegí fue una desarrollado que realicemos (dos personas) para la empresa a la cual trabajo el aplicativo conlleva en migrar las afiliaciones de cliente naturales (persona individual) y clientes jurídicos(empresas).

El aplicativo usa una arquitectura basada en eventos, los eventos de plataforma permiten el flujo de mensajes de eventos en Salesforce o hacia y desde aplicaciones externas. Las aplicaciones de la plataforma de Salesforce usan un método Ápex para publicar eventos y un desencadenador de Ápex o el componente Lightning empApi para consumir eventos. Como alternativa al código, puede publicar eventos con herramientas declarativas, como Process Builder y Flow Builder. Las aplicaciones externas publican eventos utilizando la API de sObject y consumen eventos empleando CometD. Como puede ver, el grado de flexibilidad es considerable a la hora de elegir cómo usar los eventos de plataforma.

Lo que tendríamos que hacer es migrar a una arquitectura de microservicios es utilizar Heroku es un excelente lugar para ejecutar aplicaciones y microservicios que puede utilizar con Salesforce a través de varios métodos de integración.

Ejercicio 2
En la aplicación que se ha usado como ejemplo en el ejercicio anterior, ¿podría usar diferentes lenguajes? ¿Qué almacenes de datos serían los más convenientes?

Si podríamos usar diferentes lenguaje utilizando Heroku el cual permite desarrollar en varios lenguajes tales como: Java , Node.js , Scala , Clojure , Python , PHP y Go. El aplicativo usa almacenes de datos SOQL (Salesforce Object Query Language) el cual puede usar para leer los registros guardados. SOQL es similar al lenguaje SQL estándar, pero se ha personalizado para la Plataforma Lightning, se puede usar base de datos no relacionadas como como mongo, cassandra. 

