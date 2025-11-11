🗓️ Información general

Proyecto: Sistema de Control de Stock
Iteración: 2
Duración: 3 semanas
Objetivo: Incorporar las funcionalidades de alerta de bajo stock (HU3) y generación de informe de stock (HU4).

✅ Aspectos positivos

Se completaron todas las historias de usuario planificadas (HU3 y HU4) en los tiempos estimados.

Las alertas de stock bajo funcionan correctamente y se actualizan en tiempo real.

El informe de stock puede generarse y exportarse en formato PDF, cumpliendo los criterios de aceptación.

Hubo una excelente coordinación entre las parejas XP, que permitió dividir tareas de frontend, backend y pruebas de manera equilibrada.

Se mejoró la organización del repositorio GitHub, aplicando la convención de commits y ramas definida al cierre de la Iteración 1.

Las reuniones diarias (Daily Scrum) se mantuvieron breves y efectivas, lo que ayudó a anticipar bloqueos.

⚠️ Aspectos a mejorar

Persistieron pequeñas diferencias de diseño visual entre componentes desarrollados por distintas parejas.

La exportación a PDF tuvo problemas iniciales por incompatibilidades con la librería iText.

Algunos test unitarios necesitaron ajustes por errores en las rutas de la base de datos de prueba.

Se detectó que la carga inicial de productos en la base de datos podía ralentizar la generación del informe con grandes volúmenes de datos.

💡 Acciones de mejora

Crear una guía de estilos visuales para mantener coherencia entre componentes de la interfaz.

Documentar claramente la configuración del entorno de pruebas (paths, versiones, dependencias).

Evaluar optimización de consultas SQL para informes (uso de índices y paginación).

Implementar una función de “previsualización” antes de exportar a PDF.

Realizar pruebas de carga con datos simulados para medir rendimiento.

🤝 Lecciones aprendidas

La importancia de probar con datos reales y volúmenes variados antes de entregar la funcionalidad.

El valor de tener un repositorio bien estructurado y documentado para facilitar la colaboración.

La utilidad de la revisión cruzada de código (code review) entre parejas XP para mejorar la calidad final.

Que las herramientas de automatización (scripts de pruebas, logs, build) ahorran tiempo en iteraciones posteriores.

🧭 Conclusión

La Iteración 2 consolidó las funciones principales del sistema y mejoró el trabajo en equipo.
El producto ahora cuenta con un módulo completo de gestión de stock, alertas inteligentes y reportes automáticos, cumpliendo los objetivos de las primeras dos entregas.
El grupo adquirió mayor madurez en el uso de Scrum y XP, y se encuentra preparado para planificar una posible Iteración 3 orientada a optimización, seguridad o diseño visual.