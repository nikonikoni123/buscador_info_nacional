# buscador_info_nacional
Proyecto Nikou: Mi Asistente Digital para Conectar al Ciudadano y el Estado en Colombia...
Toda la documentación y funcionamiento se encuentran anexados dentro de Buscador_info_nacional.ipynb

## Introducción
Desde que empecé a interesarme por la transformación digital, he notado lo difícil que resulta encontrar información en los distintos portales .gov.co. a menudo, la navegación se vuelve confusa y frustrante. Por eso, decidí crear Nikou, un chatbot que pueda acompañarte tanto en WhatsApp como directamente en las páginas .gov.co, para facilitar el acceso a la información pública de manera rápida y sencilla. Lastimosamente esta primera versión no puede ser desplegada en WhatsApp por falta de recursos económicos, siendo esta primera versión un prototipo técnico que sueño con verlo implementado en la realidad.

## Objetivos
Bajo la premisa de una búsqueda Eficiente de Información: En esta primera etapa, Nikou actúa como un buscador inteligente, redirigiéndote al sitio o documento (PDF) correcto según tu consulta, ahorrando tiempo y complicaciones.
Simplificación de la Experiencia Digital: Transforma la forma en que interactuar con la información, evitando textos largos y técnicos, ofreciendo una respuesta clara, fácil de entender.
Fundamento para el Futuro: Este proyecto es solo el comienzo; la visión es que Nikou evolucione y se integre a todas las tecnologías nacionales creadas hasta convertirse en una Inteligencia Artificial General (AGI) pública no dependiente de servicios terceros para una protección de datos eficiente, capaz de gestionar tareas complejas y adaptarse a las necesidades de cada ciudadano.
Descripción de la Herramienta
Nikou es una propuesta integradora que busca simplificar la vida digital, facilitando el acceso a información. La idea es que funcione como tu asistente personal, en diversas plataformas de acceso limitado para acompañar a los usuarios en cada paso desde las regiones:

Redirección Inteligente: Cuando cuentas lo que necesitas, Nikou actúa de inmediato para identificar y dirigirte a la página o documento oficial correcto, evitando que tengas que buscar manualmente.

Accesibilidad Universal: Con su presencia en WhatsApp, cualquier persona, sin importar su nivel de familiaridad con la tecnología, puede obtener la información estatal de forma rápida y eficiente.

Visión a Futuro: Evolución hacia una AGI Pública:

La meta es transformar y actualizar la gestión pública, convirtiendo a Nikou en un entorno de Inteligencia Artificial General (AGI) que gestione múltiples procesos estatales de forma autónoma y eficiente, adaptando a las necesidades del ciudadano y funcionarios especializados.

## Conclusión
El proyecto Nikou nace de mi convicción de que el acceso a la información correcta no tiene por qué ser complicada. Con este asistente digital, quiero acercar a la ciudadanía y las diferentes herramientas tecnológicas públicas de manera directa y sencilla, ya sea a través de WhatsApp o en las páginas .gov.co. Hoy, Nikou es tu buscador inteligente, pero mi visión es que se convierta en un compañero digital completo, transformando la experiencia de interacción. Estoy convencido de que, con este proyecto, la función pública se volverá más cercana, eficiente e inclusiva para todos.

## NOTAS ADICIONALES DE AUTOR:
esta es una versión beta realizada en mi tiempo libre desde la clínica de la sabana, continuando su desarrollo apasionadamente desde casa, logrando implementar servicios de r1 7B de manera local e independiente, generando un control privado de información.

En un inicio fue planeado como complemento a un modelo bert que he ido realizando por más de 2 años que busca optimizar la búsqueda de procesos judiciales. El modelo bert busca entender la normativa aplicable en cada consulta para tener una comprensión legal que pueda facilitar el acceso a la documentación (este modelo se encuentra en entrenamiento) sin embargo el proyecto fue creciendo hasta obtener vida propia, siendo una alternativa amigable y necesaria.

## Como funciona:
es un sistema simple, por medio de search realiza una búsqueda inicial limitando a solo páginas de dominio.gov.co.
Extrae la información por medio de scraping plano, elimina las etiquetas html encontradas.
Cita el link de la página web.
Resume y comprime la información para ser más accesible al usuario.
Si la información no es encontrada, verifica documentos pdf de dominio .gov.co extrae la información y verifica si el documento tiene similitud con la consulta.
