# Guia testing - GLA 2023

## Temario:

## 1. Conceptos basicos.


> 1. __Calidad__:
el grado de un sistema o proceso que satisface los requerimientos especificos y las expectativas o necesidades del cliente.

Tambien se lo puede denominar como:
- __Eficiencia__.
- __Flexibilidad__.
- __Confiabilidad__.
- __Mantenibilidad__.
- __Portabilidad__.
- __Usabilidad__.
- __Seguridad__.
- __Integridad__.
---
> 2. __Testing__: Proceso utilizado para verificar _la correccion_, _la integridad y calidad_ del software desarrollado (Funcionales y tecnicos).

- Esto implica poner a prueba la aplicacion bajo condiciones controladas (normales y anormales) segun los __casos de prueba__ predefinidos y evaluar los resultados.
Las pruebas buscan que algo en el software "salga mal" para determinar si algo sucede cuando no deberia.
---
> 3. __Asegurar la Calidad__: ¿Como asegurarla? a traves de
- Estrategias de pruebas.
- Tipos de prueba.
- Tecnicas de pruebas.
- Herramientas.
- Procesos y actividades relacionadas a la planificacion.
- Artefactos. documentaciones e informes.

> __Beneficios__: ¿Que beneficios nos proporciona el testing?
- Comprobar si los resultados son consistentes con el requerimiento.
- Reducir la mayor cantidad de defectos productivos.
- Anticipar riesgos o desvios.

---

## 2. Roles - Responsabilidades y actividades.

> __Equipo de calidad de GLA__.
- QA Analyst: Primera linea QA. Pruebas __MANUALES__.
Seguimiento de ejecuciones de "Casos automatizados".

- QA Enginner: Pruebas __MIXTO__.
Analisis de factibilidad de automatizacion (Que vale la pena automatizar), diseño, desarrollo, despliegue y mantenimiento de pruebas automatizadas (_simples_).

- QA Automation: Pruebas __AUTOMATIZADAS__.
Diseño, desarrollo, despliegue y mantenimiento de pruebas
automatizadas (_complejas_), y mantenimiento de las
herramientas de automatizacion.

- QA Lead: Es el __responsable__ de un equipo QA.
Gestiona al equipo y planifica su trabajo, ademas
puede participar en las tareas de testing.

> __Seniorities__.
- Trainee / Pasante.
- Junior.
- Semi Senior.
- Senior.
- Lead.

> __Estructura de la organizacion__.

![image](https://user-images.githubusercontent.com/120741890/214307917-995394b7-50eb-40a7-b04a-d7b624c67a1d.png)

_Focos_:
- QA Manual: Negocio, especialistas por verticales.
- QA Mixto: Negocio y aspectos tecnicos, especialistas por verticales.
- QA Automation: Tecnico - Cross negocio.

> __Responsabilidades__.

1. __Compromiso__:
Es la capacidad de actuar como el dueño del negocio, lo que conlleva instrumentar decisiones para lograr objetivos comunes potenciando el trabajo en equipo.
Evaluar acciones y resultados de forma critica e intencion de mejora y controlar la puesta en marcha de las acciones comprometidas.

__Caracteristicas__:
- Iniciativa y moviliza los recursos para agregar valor.
- Asume responsabilidad con actitud protagonista.
- Se anticipa a potenciales problemas, los detecta y actua en consecuencia.
- Se esfuerza al maximo para alcanzar los objetivos. Es exigente con los estandares y siempre busca mejorar.

2. __Orientacion a la calidad__:
Capacidad para lograr resultados de excelencia, teniendo en cuenta las expectativas y necesidades del cliente.
Tener una vision proyectada en la mejora continua de procesos que optimicen las soluciones y servicios, y es la capacidad de establecer estandares altos de cumplimiento optimizando los recursos disponibles.

__Caracteristicas__:
- Analiza exhaustivamente las causas de los problemas, sin quedarse en lo evidente.
- Explora alternativas, buscando mejoras en los procesos.
- Considera todos los datos y escenarios antes de tomar una decision.

3. __Trabajo en equipo__.
Se relaciona con el grupo de pertenencia (relaciones intragrupales) y tambien con miembros de otros grupos (intergrupales), mostrando confianza y respeto, comunicacion efectiva, integracion de objetivos y valores personales con los del grupo y de la organizacion.
Dispuesto a colaborar con los demas y contribucion plena a las tareas y resultados pertinentes.

__Caracteristicas__:
- Se involucra con los objetivos del equipo y los hace propios.
- Contribuye a generar y a mantener el buen clima de trabajo.
- Construye vinculos de confianza y promueve el respeto.
- Se muestra predispuesto a apoyar y ayudar a los compañeros.

---

## 3. Entregables de calidad.

> ¿_Que es un entregable de calidad_?
- Documentacion generada por el area de calidad,
tambien llamados __artefactos__.
- Es un conjunto de documentos que obtiene el __tester__.

> __Clasificacion de un entregable de calidad__.
- Checklist de Proyecto.
- Plan de pruebas (Estrategia de pruebas).
- Escenarios de prueba.
- Casos de prueba.
- Matriz de trazabilidad.
- Reportes de prueba:
    - Informe de avances diario.
    - Informe al final de Sprint.
    - Informe evolutivo de Sprint.

> ¿_En que momento se utilizan_?
- Checklist: Antes, durante y despues de cada iteracion.
- Plan de pruebas y estrategias de prueba: Al inicio del proyecto.
- Escenarios de prueba y casos de prueba: Durante el Sprint.
- Matriz de trazabilidad: Durante el Sprint.
- Reportes: Durante o al final de la ejecucion.
- Manual del usuario: Al final del Sprint


> ¿_Con quien se comparten los artefactos_?

Se comparten con el cliente, con el equipo de prueba, con los lideres de equipo y los sponsor (partes interasadas del proyecto) y tambien con miembros de otros equipos.

---

## 4. Tipos de test

### 4.1 - __Pruebas funcionales__.
> Estas pruebas __verifican__ que el producto cumple con lo especificado en los requerimientos, US o CU.

<br>

> __Tipos de pruebas__.

- __Pruebas unitarias__.
Prueban una unidad o fragmento de codigo mas pequeño
que se puede aislar logicamente en un sistema.
Es responsabilidad del __desarrollador__, que se realiza
al terminar el codigo a testear en un ambiente de desarrollo.

- __Pruebas de sistema funcional / integracion__.
Aseguran que el sistema satisface las funcionalidades
previamente diseñadas. Se evalua como los
diferentes componentes de una aplicacion interactuan
juntos en el sistema o aplicacion completa e integra.
Se realizan mediante el diseño de casos de prueba
que buscan evaluar cada una de las posibilidades para
verificar si se cumplen los requerimientos.
Son responsabilidad del __Calidad__ y se realizan una
vez finalizadas las pruebas unitarias en un ambiente
de prueba / test.

    - __Look and feel__: Validar la apariencia de la aplicacion.
        - Responsive: Verifica si se adaptan a las diferentes pantallas.
        - __Brownsers__: Valida la compatibilidad con los diferentes 
        navegadores, versiones y modo.
        - __Platforms__: Verifica la aplicacion en diferentes
        plataformas web o mobile (Android, IOS).
    - __Enlaces__: Validar los links y redireccionamientos.
    - __Integracion__: Los modulos se combinan y se testea
    como un grupo integro y las interacciones con
    las diferentes partes del sistema como BE, BD, Servicios
    u APIS.
    - __Accesibilidad__: Garantizan que todas las personas,
    incluso las que poseen incovenientes puedan usar la aplicacion.
- __Pruebas exploratorias__.
Se utilizan en el momento que una persona necesita aprender 
o conocer rapidamente el producto, proveer feedback.
Se espera obtener el punto de vista del lado del usuario.
Es responsabilidad de __Calidad__ y se realiza on demand, 
en un ambiente Test / UAT (User Acceptance Testing).

- __Pruebas de sanidad__.
Prueban cambiamos menores, sin mucha profundidad 
o para verificar si los defectos fueron arreglados.
Es responsabilidad de __Calidad__ y se realizan 
cuando se solicite y puede ser al inicio del Sprint en un ambiente de Test.

- __Pruebas de humo__ (smook).
Aseguran que las funcionalidades criticas estan funcionando correctamente. 
Orientado a la estabilidad del sistema.
Es responsabilidad de __Calidad__, y se realizan segun
planificacion, cuando se dispone de poco tiempo, y suelen
ser al inicio del Sprint en un entorno de Test.

- __Pruebas de regresion__.
Suite de pruebas de todas las funcionalidades del software
que aseguran que en las nuevas versiones no se introduzcan
nuevos incidentes.
Es responsabilidad de __Calidad__ se realizan segun
la planificacion y pueden ser al inicio del Sprint, en un
entorno de Test.

- __Pruebas de aceptacion__. (UAT)
Son pruebas realizadas por el cliente/negocio en un 
periodo de tiempo para corroborar que el sistema
cumple con lo solicitado.
Son responsabilidad del __cliente/usuario final__, 
se realizan al finalizar el Sprint para recibir 
feedback de la aplicacion en un ambiente UAT.

---
### 4.2 - __Pruebas NO funcionales__.
> Se enfocan en aspectos importantes pero
no estan relacionados con las funciones que realiza
el sistema.

<br>

> __Tipos de pruebas__.

- __Pruebas de stress__.
Intentan romper el sistema bajo condiciones de carga
extremadamente pesadas.
El proposito principal detras de esto es asegurar
que el sistema falle y se recupere correctamente
bajo situaciones crtiicas.
Es responsabilidad de __Calidad__ y se realizan
Antes / Durante o despues de un Sprint en un ambiente
de Test / UAT.

- __Pruebas de Performance__.
Intenta determinar el rendimiento de un sistema
para medir, validar o verificar los atributos
de calidad del sistema, como la capacidad de respuesta,
velocidad, escalabilidad y estabilidad en una variedad
de carga.
Es responsabilidad de __Calidad__ y se realizan
Antes / Durante o despues de un Sprint en un ambiente
de Test / UAT.

- __Pruebas de seguridad__.
Se buscan encontrar vulnerabilidades de seguridad.
Es responsabilidad de __Calidad__ y se realizan
Antes / Durante o despues de un Sprint en un ambiente
de Test / UAT.

- __Pruebas de instalacion__.
Verifican todo lo relacionado con el despliegue
del producto: documentacion, instalacion, configuracion
post-instalacion, etc.
Es responsabilidad de __Calidad__ y se realizan
al finalizar el despliegue en un ambiente
de Test / UAT.

- __Pruebas de usabilidad__.
Estan enfocadas en el usuario final y ayudan a crear
una mejor experiencia tambien conocido como UX.
Testean la facilidad de uso del usuario en terminos de
operacion, aprendizaje y preparacion de entradas y salidas,
Es responsabilidad de __Calidad__ y se realizan
durante el Sprint en un ambiente
de Test / UAT.

- __Pruebas de Accesibilidad__.
Tambien llamadas de "__Compliance__" (cumplimiento).
Se realizan para verificar si se siguen o no los
estandares definidos. Se realizan auditorias para verificar
el cumplimiento de la norma.
Es responsabilidad de __Calidad__ y se realizan
durante el Sprint en un ambiente
de Test / UAT.

---

### 4.3 - __Tipos de test - Manual y Automatizado__.

- __Pruebas Manuales__:
> Es un tipo de prueba de software donde los __testers__
ejecutan manualmente los casos de prueba sin usar ninguna
herramienta de automatizacion, utlizando diferentes
tecnicas y metodos para validar los requisitos.
Cualquier aplicacion nueva debe probarse manualmente antes
de que esta pueda automatizarse.
Requiere de mayor esfuerzo pero es necesaria para
verificar la viabilidad de la automatizacion.

- __Pruebas Automatizadas__:
> Es una tecnica de testing automatico realizada por
una herramienta. Se suele utilizar en conjunto de
sistemas de repote automatico para proveer un testeo
y reporte automatico sin tener que utilizar horas de un QA manual.
Las principales ventajas del testeo automatico es su velocidad, no consume el tiempo de los QA manual, aumenta la cobertura de testing e incrementa la ejecucion de los test.
Este tipo de test se suele utilizar cuando los tests son repetitivos, el proyecto se hace extenso lo que conlleva
que probar todo manualmente se perderia mucho tiempo.

---

## 5. Casos de prueba.
> Es un _conjunto_ de __condiciones__ o variables
bajo las cuales se _determinara_ si el __comportamiento__
de una aplicacion o un sistema __resulta__ o no _aceptable_.

> ¿_Que es un caso de prueba_?

Responde a la pregunta: ¿_Que voy a probar_?

Se desarrollan para __definir__ las acciones que son
necesarias validar a fin de __asegurar__ que el sistema funcione
correctamente y este construido con un alto nivel de calidad.

> ¿_Como conseguirlo_?

Estructurando como vamos a realizar las pruebas
cubriendo la mayor cantidad de escenarios.

> Identificando los escenarios de prueba.

El objetivo de plantear escenarios de prueba es
__obtener__ una _aproximacion_ para luego diseñar los casos
de prueba correspondientes.

- __Caja negra__: verifica las condiciones de la
entrada __sin__ importar como esta codificado.
- __Caja blanca__: verificacion del codigo.
- __Caja gris__: Es una combinacion de ambas.

![image](https://user-images.githubusercontent.com/120741890/214345508-24d72124-d1a6-4e63-8751-5b2012a9822d.png)

Tenemos que tener en cuenta que los valores de entrada
tambien denominados __inputs__ que son aquellos que nosotros ingresamos manualmente, se dividen en __dos__ tipos:
- __validos__: Los que se espera que reciba.
- __invalidos__ Los que no se espera que reciba.
Y los valores de salida tambien llamados __outputs__
que son los resultados que nosotros esperamos.

> Diseñando los casos de prueba.

Plantear los casos en base a los escenarios. <br>
Luego de analizar las US, podemos dividir los casos en:

![image](https://user-images.githubusercontent.com/120741890/214347670-c93ea35c-b091-4f6c-b2b5-aadd55fb037d.png)

1. __Flujo positivo__: Cuando se cumple la situacion ideal
de la historia __End2End__ que por lo general suele ser
la mas importante y el __core__ de la funcionalidad.
Pueden haber mas de uno.

2. __Flujo Alternativo__: Se despreden del principal cuyas
variantes representan una alternativa para validar.

3. __Flujo negativo__: Son aquellos flujos que forzamos
para que nos informen que no se cumple con lo 
necesario para avanzar, puede ser el faltante de un dato,
no respeta el formato, etc.

> Proceso de una ejecucion

![image](https://user-images.githubusercontent.com/120741890/214349875-572ef8f0-9364-4ca8-9037-e4511ae67493.png)

> Estados de un caso de prueba.
- __Failed__ (Fallo).
El caso de prueba fallo en una o mas validaciones.
En dicho caso se debe reportar un bug y clasificarlo
segun la criticidad del mismo.
- __Passed__ (Paso).
El caso de prueba se ejecuto correctamente.
En donde el resultado es el mismo al resultado __esperado__.
- __Blocked__ (Bloqueada).
El caso de prueba esta bloqueado por otro caso o
paso antecesor.
Se lo define cuando un caso anterior ha fallado y es
precondicion para su ejecucion.
Por lo tanto no se considera fallido porque
no se ha realizado la validacion.

> __Buenas practicas__ para escribir los casos de prueba.
- Resumen / Titulo descriptivo del caso.
En donde se detalla la finalidad que persigue el testing.
Que vamos a probar, como lo vamos a probar, datos que necesitemos, etc.
- Precondiciones.
Requisitos necesarios previos para que este CP pueda
pasar o aprobarse.
Acceso a una BD, credenciales, un dato especifico, etc.
- Pasos / Steps + Datos de prueba.
El paso a seguir para replicar dicha prueba y ademas
se recomienda agregar los datasets para saber
si la prueba fallo por el uso de algun dato en particular.
- Resultados esperados.
Se detallara los resultados esperados de la validacion
realizada en el paso.
- Keywords.
Se define el tipo de prueba que se va a realizar,
es decir, si es funcional, no funcional, de tipo regresion, integracion, etc.
- Requisitos.
Es donde vamos a relacionar el CP con la US que vamos
a estar testeando.
- Tipo de ejecucion.
Indicara si las pruebas seran de tipo manual o automatizadas.
- Version.
La version del caso, dado que cada caso puede mantener 
su resultado final esperado o cambiar sus pasos
y dichos resultados esperados de cada uno.
Por lo que puede que un caso deba de modificar y ser
una version 2, 3, etc.

> ¿Splintear? (__Dividir__ las pruebas)
- Ventaja: Tenemos bien identificados los casos que fallan.
- Desventaja: Se necesita mas tiempo de escritura y 
actualizacion de estados.

Luego se debera decidir si se reporta un bug por caso
fallido o se incluye todo en un mismo defecto.

> Requisitos para ejecutar los CP

- Diseño de escenarios de cobertura validos por el equipo.
- Casos de prueba finalizados.
- Data set generado. (Datos que se utilizaron par hacer las pruebas)
- Contar con las configuraciones, accesos y usuarios
necesarios para la utilizacion de la herramienta.
- Historia en Jira con sub-tareas de desarrollo finalizadas,
incluidas las pruebas unitarias.
- Codigo deployado en el ambiente exclusivo de calidad, es decir en el ambiente de QA.
- Ambientes disponibles, para evitar re-hacer las pruebas
o que otro tambien las este haciendo al mismo tiempo.

> Tareas de cierre de la ejecucion.
- Recolectar evidencia.
Pueden ser capturar, grabar la pantalla de ser necesario
para mostrar la evidencia del resultado esperado que se cumpla.
- Actualizar herramienta con estado final de la ejecucion.
- Enviar reporte de ejecucion + defectos.

---