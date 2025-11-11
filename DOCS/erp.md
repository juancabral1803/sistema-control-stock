Especificación de Requisitos del Proyecto
📌 1. Información general

Proyecto: Sistema de Control de Stock
Materia: Ingeniería del Software
Metodología: Scrum + XP
Equipo:

Juan Pérez (Scrum Master)

María López (Product Owner)

Carlos Gómez y Ana Díaz (Equipo de desarrollo)
Repositorio GitHub: [a completar con el enlace del grupo]

🎯 2. Descripción general del sistema

El sistema de control de stock permitirá a una tienda o depósito gestionar de forma digital el ingreso, salida y control de productos.
El objetivo principal es mantener actualizada la información del inventario, evitando pérdidas o desabastecimientos.

Los usuarios podrán registrar productos nuevos, actualizar cantidades, consultar listados y generar alertas automáticas cuando un artículo esté por debajo del stock mínimo.

👥 3. Actores del sistema
Actor	Descripción	Funciones principales
Encargado	Usuario que gestiona el stock y realiza operaciones diarias.	Registrar ingresos/salidas, consultar productos, ver alertas.
Administrador	Usuario con permisos avanzados.	Configurar stock mínimo, agregar usuarios, generar reportes.
🧱 4. Requisitos funcionales
ID	Requisito	Descripción
RF1	Registrar producto nuevo	Permitir crear un nuevo producto con código, nombre, precio y stock inicial.
RF2	Registrar ingreso de stock	Registrar el aumento de unidades de un producto existente.
RF3	Registrar salida de stock	Registrar las ventas o egresos de productos.
RF4	Consultar productos	Mostrar listado de productos con sus datos y estado actual.
RF5	Generar alerta de bajo stock	Enviar notificación visual o sonora cuando un producto esté en o por debajo del stock mínimo.
RF6	Generar informe de stock	Mostrar resumen general de existencias, productos en falta y movimientos recientes.
🚫 5. Requisitos no funcionales
ID	Requisito	Descripción
RNF1	Usabilidad	Interfaz simple e intuitiva.
RNF2	Rendimiento	Responder a consultas en menos de 3 segundos.
RNF3	Seguridad	Autenticación de usuarios con roles.
RNF4	Portabilidad	Accesible desde navegador web.
RNF5	Mantenibilidad	Código estructurado en capas (MVC).
⚙️ 6. Tecnologías y entorno
Componente	Tecnología seleccionada
Lenguaje backend	Java
Framework	Spring Boot
Base de datos	MySQL
Motor de plantillas	Thymeleaf
Testing	JUnit 5
Control de versiones	Git / GitHub
Metodología	Scrum + XP
📅 7. Planificación ágil

El desarrollo se realizará en 3 iteraciones (sprints) de aproximadamente 3 semanas cada una.

Iteración	Objetivo principal	Entregables
Iteración 0	Preparación del entorno y configuración inicial.	Proyecto base, BD, repositorios, modelos.
Iteración 1	Funcionalidades de registro y listado.	HU1 y HU2 completadas.
Iteración 2	Alertas e informes.	HU3 y HU4 completadas.
💡 8. Historias de usuario (resumen)
ID	Historia de usuario	Prioridad	Tiempo estimado
HU1	Como encargado quiero registrar nuevos productos con su código, nombre, precio y stock inicial para mantener actualizada la base de datos.	Alta	7 días
HU2	Como encargado quiero registrar las salidas de productos para llevar un control actualizado de ventas.	Alta	5 días
HU3	Como encargado quiero ver una alerta cuando un producto tenga stock igual o menor al mínimo para reponerlo.	Media	4 días
HU4	Como administrador quiero generar un informe de stock para conocer la situación general del inventario.	Media	6 días
🔄 9. Criterios de aceptación generales

Todos los campos obligatorios deben validarse antes de guardar.

Las operaciones deben registrarse en la base de datos.

Los mensajes de error o confirmación deben ser claros.

Las alertas deben actualizarse automáticamente al modificar stock.

📦 10. Riesgos y consideraciones

Posible falta de disponibilidad del servidor o conexión a la base de datos.

Cambios en requerimientos del cliente durante el desarrollo.

Necesidad de capacitación para el uso del sistema.