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

- Pruebas de regresion.
Suite de pruebas de todas las funcionalidades del software
que aseguran que en las nuevas versiones no se introduzcan
nuevos incidentes.
Es responsabilidad de __Calidad__ se realizan segun
la planificacion y pueden ser al inicio del Sprint, en un
entorno de Test.

- Pruebas de aceptacion. (UAT)
Son pruebas realizadas por el cliente/negocio en un 
periodo de tiempo para corroborar que el sistema
cumple con lo solicitado.
Son responsabilidad del __cliente/usuario final__, 
se realizan al finalizar el Sprint para recibir 
feedback de la aplicacion en un ambiente UAT.
