## Iteración 2 – Información general

**Proyecto:** Sistema de Control de Stock  
**Iteración:** 2  
**Duración estimada:** 3 semanas  
**Objetivo principal:** Implementar las **alertas automáticas por bajo stock** y el **módulo de informes generales del inventario**.

---

### Historias de usuario seleccionadas

#### HU3 – Mostrar alerta de bajo stock

**Historia de usuario:**  
Como encargado quiero recibir una alerta cuando un producto tenga stock igual o menor al mínimo, para poder reponerlo a tiempo.

**Criterios de aceptación:**

- Si `stock_actual ≤ stock_mínimo`, se muestra una alerta visual en el sistema.  
- Solo usuarios con rol “Encargado” o superior pueden verla.  
- Si no hay productos con bajo stock, se muestra el mensaje “Sin alertas”.  
- La alerta se actualiza automáticamente al modificar el stock.

**Tareas técnicas:**

- Crear consulta SQL que detecte productos con stock bajo.  
- Diseñar componente visual (alerta o ícono con color de advertencia).  
- Implementar actualización automática del estado de stock.  
- Validar permisos de usuario según rol.  
- Probar alertas con distintos valores de stock y usuarios.

**Pareja XP asignada:**  
Pareja B: Carlos y Ana  
Roles rotativos: Carlos (driver – backend), Ana (navigator – testing/UI).

**Tiempo estimado:** 4 días  
**Observaciones:** Se prioriza la respuesta visual inmediata y la automatización de la actualización para mejorar la toma de decisiones del encargado.

---

#### HU4 – Generar informe de stock

**Historia de usuario:**  
Como administrador quiero generar un informe general del stock para conocer la situación actual del inventario y detectar faltantes.

**Criterios de aceptación:**

- El informe debe mostrar todos los productos con sus cantidades y estado (normal o bajo stock).  
- Debe poder exportarse en formato PDF o visualizarse en pantalla.  
- Debe incluir la fecha y hora de generación.  
- Solo accesible para usuarios con rol “Administrador”.

**Tareas técnicas:**

- Diseñar plantilla de informe con **Thymeleaf**.  
- Implementar método `generarInforme()` en el backend.  
- Integrar librería para exportación a PDF (por ejemplo, **iText**).  
- Probar informe con distintos volúmenes de datos.  
- Agregar filtros por categoría o rango de fechas (opcional).

**Pareja XP asignada:**  
Pareja A: Juan y María  
Roles rotativos: María (driver – frontend/reportes), Juan (navigator – backend), alternan semanalmente.

**Tiempo estimado:** 6 días  
**Observaciones:** El módulo debe ser claro, rápido y fácilmente entendible por el administrador. Se busca entregar una herramienta útil para auditorías internas.

---

### Tareas generales de la iteración

- Actualizar la base de datos: agregar campo `stock_minimo` a la tabla de productos.  
- Integrar un sistema de notificaciones visuales en la interfaz.  
- Implementar funcionalidad de exportación a PDF.  
- Realizar pruebas de rendimiento y validación de permisos.  
- Actualizar documentación del repositorio (`README.md` y `changelog`).

---

### Definition of Done (DoD)

- HU3 y HU4 desarrolladas, probadas y funcionales.  
- Alertas de stock bajo se muestran correctamente y se actualizan en tiempo real.  
- Informes de stock exportables a PDF.  
- Revisión de código completada por ambas parejas XP.  
- Actualización de documentación y commits verificados.

---

### Resultado esperado

Al finalizar esta iteración, el sistema podrá alertar al encargado sobre productos con **bajo stock** y generar **informes completos de inventario**, consolidando las funciones principales del control de stock y preparando el terreno para una posible **tercera iteración** (optimización o mejoras visuales).
