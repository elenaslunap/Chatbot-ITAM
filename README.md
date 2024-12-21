# Chatbot-ITAM
Diseño de un chatbot creado con Landbot que ayude a un alumno que acaba de entrar al ITAM.

## Metodología
La metodología utilizada en el proyecto es Agile, un enfoque que permite desarrollar el chatbot de forma iterativa y adaptable. Esta metodología es especialmente adecuada debido a la naturaleza dinámica del proyecto, que requiere pruebas constantes y ajustes en función del feedback recibido. Agile facilita dividir el desarrollo en etapas cortas y manejables, conocidas como sprints, en las que se trabaja en funcionalidades específicas, asegurando avances constantes hacia el objetivo final.

A lo largo del desarrollo, Agile fomenta la colaboración continua entre los miembros del equipo y los interesados en el proyecto. Esto garantiza que las decisiones tomadas reflejen las necesidades reales de los usuarios, permitiendo priorizar las tareas más relevantes y ajustar el plan a medida que surgen nuevos requisitos o cambios en las prioridades.

Además, esta metodología asegura la entrega frecuente de incrementos funcionales del sistema, lo que permite identificar problemas o mejoras desde las primeras etapas del proyecto. Esta capacidad de adaptación y respuesta rápida a los cambios contribuye a crear un producto final de mayor calidad, alineado con los objetivos planteados y con las expectativas de los usuarios.

En resumen, Agile no solo proporciona una estructura flexible y eficiente para la gestión del proyecto, sino que también garantiza un desarrollo centrado en el usuario y en la mejora continua, factores clave para el éxito del chatbot.

La planeación del desarrollo del chatbot está dividida en cuatro sprints, organizados de manera que cada etapa construya una parte fundamental del proyecto de forma progresiva y funcional. Además, cada sprint incluye la recopilación de retroalimentación del trabajo previamente realizado, permitiendo realizar mejoras y ajustes continuos para optimizar la experiencia del usuario.

En el Sprint 1, se establece la base del chatbot. Durante esta etapa, el chatbot debe saludar al usuario de forma amigable y mostrarle las seis categorías principales: campus y mapas, horarios generales, actividades extracurriculares, cafetería, servicios escolares y biblioteca. Aunque no se desarrollan los detalles de cada categoría, el enfoque está en garantizar una navegación clara y funcional por las opciones iniciales.

El Sprint 2 se dedica a desarrollar el contenido específico de cada una de las categorías presentadas en el sprint anterior. Aquí, el chatbot proporcionará detalles importantes como la ubicación y horarios del campus, las actividades disponibles, los servicios escolares y de la cafetería, así como los horarios y servicios de la biblioteca. A partir de la retroalimentación obtenida del primer sprint, se mejorará la claridad de las opciones iniciales y la lógica de navegación del chatbot.

En el Sprint 3, se amplían las funcionalidades relacionadas con las actividades extracurriculares. El chatbot permitirá al usuario enviar correos personalizados o predeterminados para solicitar información sobre clubes o eventos. Además, se añadirá una función que pregunte al usuario si necesita más ayuda tras cada consulta o si desea terminar la conversación. En esta etapa, se incorporarán los comentarios y ajustes identificados en los sprints anteriores, asegurando que el chatbot sea más intuitivo y eficiente.

Finalmente, en el Sprint 4, se integrará un mapa que ofrezca una vista general de la distribución del campus, junto con guías detalladas para áreas clave como la cafetería, la biblioteca y los departamentos de las carreras. Este sprint no solo completa las funcionalidades principales del chatbot, sino que también se beneficia de la retroalimentación acumulada a lo largo del desarrollo para perfeccionar las secciones previas y cerrar el proyecto con un sistema completamente funcional y optimizado.

## Propuesta económica
Se hicieron los siguientes cálculos para una versión avanzada del proyecto, considerando a un senior y junior software developer, product manager, database manager, DevOps junior y diseñador UX/UI.

Los resultados que se obtuvieron fueron: 
- Total de días programados: 33
- Total de días reales: 47.85
- Total sueldos: $53604
- Precio operativo: $53,831
- Precio total: $107,435
- IVA: $17,190

Total con IVA: $124,625

Link para consultar los cálculos: https://docs.google.com/spreadsheets/d/1q1lEzyGmpEZIBDwYOzISUC78EbtqOmf4wvWlQMpoBkQ/edit?usp=sharing 

## Documentación para replicar
A continuación, se muestran los comentarios de cada sección del chatbot. 
En general, su funcionamiento consiste en 
1) Preguntar al alumno sobre qué tema tiene dudas
2) Dar información general del tema
3) Preguntar si tiene dudas en específico, y de ser el caso, proporcionar los medios (ya sean imágenes, videos, vínculos o envío de correos) para resolverla.

Finalmente, se pregunta si se tienen más dudas, si es así, el ciclo regresa al paso 1, sino, manda un mensaje de adiós y queda listo para que se vuelva a iniciar la conversación. El chatbot está diseñado para resolver preguntas de lo más generales a lo más específicas, proporcionando así el apoyo necesario para un alumno de nuevo ingreso sobre los temas más importantes en sus primeros días de clases en el ITAM. Las fases comentadas en la documentación pueden ser replicadas y mejoradas en un proyecto futuro.

![Screen Shot 2024-12-20 at 11 32 34 PM](https://github.com/user-attachments/assets/28ead25f-43a7-4f50-b609-67dcd6ef3610)

![Screen Shot 2024-12-20 at 11 33 12 PM](https://github.com/user-attachments/assets/05b2c34b-b1ef-4aeb-acdb-0579f5dbd95e)

![Screen Shot 2024-12-20 at 11 34 01 PM](https://github.com/user-attachments/assets/02a35537-11da-492b-84d9-974a9e856593)

![Screen Shot 2024-12-20 at 11 36 27 PM](https://github.com/user-attachments/assets/0751a8bd-21c0-4a5c-9300-3485a6baae28)

## ARQUITECTURA

 La arquitectura del proyecto está basada en eventos, un enfoque ideal para sistemas interactivos que requieren adaptarse dinámicamente a las acciones de los usuarios. En este caso, cada interacción genera un evento que desencadena una respuesta específica, permitiendo que el sistema sea reactivo y responda en tiempo real a las necesidades del usuario. Esto garantiza una experiencia fluida y eficiente durante el uso del sistema.

El diseño basado en eventos es adecuado porque facilita la gestión simultánea de múltiples interacciones, lo cual resulta fundamental para entornos donde varios usuarios pueden estar activos de manera concurrente. Además, la estructura modular de esta arquitectura permite que los distintos componentes del sistema operen de manera independiente, simplificando tanto el mantenimiento como la incorporación de nuevas funcionalidades sin afectar el resto del sistema.

Por último, esta arquitectura optimiza el rendimiento del proyecto al ejecutar procesos únicamente cuando ocurren eventos específicos, asegurando un uso eficiente de los recursos. Estas características hacen que la arquitectura basada en eventos sea la más apropiada para alcanzar los objetivos planteados.

<img width="561" alt="Screen Shot 2024-12-21 at 0 08 04" src="https://github.com/user-attachments/assets/70e8392d-8fbe-493b-b27a-692f39910e70" />



Plan de calidad 
El plan de calidad en el diseño de un proyecto sirve como una guía para asegurarse de que todo lo que se haga cumpla con los estándares necesarios y que el resultado final sea lo que se espera. Básicamente, ayuda a organizar los pasos, definir cómo se medirá el éxito y garantizar que las cosas funcionen bien, sean fáciles de mantener y seguras. Es como un mapa que asegura que todos en el equipo trabajen en la misma dirección y que el proyecto entregue algo útil y confiable.

Garantía de la Funcionalidad
Para garantizar la funcionalidad del chatbot de ayuda para alumnos de nuevo ingreso, se definirá un conjunto claro de requisitos funcionales, que incluyen dar al estudiante la información que necesita en cuanto a campus y mapas, horarios, actividades extracurriculares, cafetería, servicios escolares y biblioteca. Se implementarán pruebas automatizadas y manuales para validar que el chatbot proporcione respuestas correctas, oportunas y relevantes para un estudiante. Estas pruebas cubrirán casos de uso comunes y variaciones en el lenguaje normal. Adicionalmente, un modelo futuro del sistema se entrenará con conjuntos de datos reales basados en preguntas frecuentes, y se empleará aprendizaje automático para mejorar continuamente la precisión y pertinencia de las respuestas.
