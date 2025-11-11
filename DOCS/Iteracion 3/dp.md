## Iteración 3 – Información general

**Proyecto:** Sistema de Control de Stock  
**Iteración:** 3  
**Duración estimada:** 2 a 3 semanas  
**Objetivo principal:** Mejorar la calidad general del sistema mediante optimizaciones de rendimiento, refactorización del código, mejoras de seguridad y ajustes en la interfaz de usuario.

---

### Historias de usuario seleccionadas

#### HU5 – Optimizar rendimiento de consultas

**Historia de usuario:**  
Como encargado quiero que las búsquedas y listados se carguen más rápido para mejorar la eficiencia en la gestión del stock.

**Criterios de aceptación:**

- El tiempo de carga del listado general no debe superar los 2 segundos.  
- Las consultas a la base de datos deben estar optimizadas con índices.  
- Los informes deben poder generarse sin bloqueos, incluso con más de 1000 registros.  
- Las pruebas de carga deben mostrar una mejora respecto a la iteración anterior.

**Tareas técnicas:**

- Revisar y optimizar consultas SQL.  
- Implementar paginación en el listado de productos.  
- Agregar índices a campos clave (código, nombre, stock).  
- Ejecutar pruebas de rendimiento con datos simulados.  
- Documentar resultados y métricas.

**Pareja XP asignada:**  
Pareja A: Juan y María  
Roles rotativos cada dos días (Juan driver / María navigator).  
**Tiempo estimado:** 5 días

---

#### HU6 – Implementar control de acceso y seguridad

**Historia de usuario:**  
Como administrador quiero que solo usuarios autorizados puedan acceder a las funciones del sistema, garantizando la seguridad de la información.

**Criterios de aceptación:**

- El sistema debe tener un inicio de sesión con usuario y contraseña.  
- Cada rol (Administrador / Encargado) debe tener permisos específicos.  
- Los intentos fallidos deben registrar logs de seguridad.  
- Los datos sensibles deben almacenarse de forma encriptada.

**Tareas técnicas:**

- Agregar módulo de autenticación con **Spring Security**.  
- Configurar roles y permisos en controladores.  
- Crear tabla usuarios con contraseñas cifradas.  
- Implementar logs de acceso y errores.  
- Pruebas de seguridad básicas (sesiones, roles, SQL Injection).

**Pareja XP asignada:**  
Pareja B: Carlos y Ana  
Roles rotativos: Carlos (driver), Ana (navigator).  
**Tiempo estimado:** 6 días

---

#### HU7 – Mejorar la interfaz de usuario

**Historia de usuario:**  
Como usuario quiero una interfaz más clara y agradable para poder gestionar el stock de forma simple y rápida.

**Criterios de aceptación:**

- La interfaz debe mantener coherencia visual (colores, tipografía, botones).  
- Los formularios deben ser responsivos.  
- Debe haber mensajes claros ante errores o confirmaciones.  
- El menú principal debe incluir accesos rápidos a las funciones más usadas.

**Tareas técnicas:**

- Aplicar diseño unificado (plantilla base con CSS/Bootstrap).  
- Mejorar feedback visual en formularios y botones.  
- Incorporar alertas modales (confirmación, error, éxito).  
- Validar adaptabilidad a dispositivos móviles.

**Pareja XP asignada:**  
Pareja mixta (Juan y Ana) para fomentar colaboración cruzada  
Roles rotativos por jornada  
**Tiempo estimado:** 4 días

---

### Tareas generales de la iteración

- Refactorizar código duplicado en servicios y controladores.  
- Actualizar documentación técnica del sistema.  
- Realizar backup de la base de datos antes del despliegue.  
- Probar integración completa de módulos.  
- Preparar presentación final del proyecto.

---

### Definition of Done (DoD)

- Las optimizaciones de rendimiento verificadas con métricas.  
- Control de acceso totalmente funcional.  
- Interfaz final integrada y coherente.  
- Pruebas de integración superadas sin errores críticos.  
- Proyecto documentado y listo para entrega.

---

### Resultado esperado

Al finalizar esta iteración, el sistema será estable, seguro y visualmente mejorado, con un desempeño optimizado.  
El equipo completará la **entrega final del proyecto** con un producto funcional, bien documentado y alineado con los principios de **Scrum y XP**.
