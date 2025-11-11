🗓️ Información general

Proyecto: Sistema de Control de Stock
Iteración: 1
Duración estimada: 3 semanas
Objetivo principal: Implementar las funcionalidades básicas del sistema: registro de productos nuevos y registro de salidas de stock.

🎯 Historias de usuario seleccionadas
HU1 – Registrar producto nuevo

Historia de usuario:

Como encargado quiero registrar nuevos productos con su código, nombre, precio y stock inicial para mantener actualizada la base de datos.

Criterios de aceptación:

Todos los campos (código, nombre, precio, stock inicial) son obligatorios.

Si el producto ya existe (mismo código), se muestra un mensaje de error.

Si se guarda correctamente, aparece mensaje de confirmación.

El producto queda visible en el listado general.

Tareas técnicas:

Diseñar formulario “Nuevo Producto”.

Validar campos requeridos en el frontend.

Crear método insertarProducto() en el backend.

Probar inserción en la base de datos MySQL.

Testear interfaz con datos válidos e inválidos.

Pareja XP asignada:

Pareja A: Juan y María

Roles rotativos: Juan (driver), María (navigator), alternan cada media jornada.

Tiempo estimado: 7 días.

Observaciones:
Se prioriza la funcionalidad de alta de productos, ya que es base para las demás operaciones del sistema.

HU2 – Registrar salida de producto

Historia de usuario:

Como encargado quiero registrar las salidas de productos para llevar un control actualizado de ventas y existencias.

Criterios de aceptación:

Solo se pueden registrar salidas si hay stock disponible.

Si la cantidad a restar supera el stock actual, se muestra mensaje de error.

La operación actualiza el stock en tiempo real.

Se genera un registro histórico del movimiento.

Tareas técnicas:

Crear formulario “Salida de Producto”.

Implementar método registrarSalida() en backend.

Actualizar campo de stock en base de datos.

Generar tabla “movimientos” para auditoría.

Test unitarios con JUnit sobre operaciones de salida.

Pareja XP asignada:

Pareja B: Carlos y Ana

Roles rotativos: Carlos (driver, backend), Ana (navigator, testing), alternan por día.

Tiempo estimado: 5 días.

Observaciones:
Se busca validar la correcta actualización del stock y evitar inconsistencias en base de datos.

⚙️ Tareas generales de la iteración

Crear estructura de paquetes del proyecto (modelo, repositorio, servicio, controlador).

Configurar conexión a base de datos MySQL y probar acceso.

Implementar interfaz inicial con Thymeleaf.

Configurar control de versiones en GitHub.

Documentar avance y pruebas en retrospectiva.md.

🧾 Definición de “Hecho” (Definition of Done)

Las funcionalidades HU1 y HU2 están desarrolladas, probadas y validadas por el equipo.

La base de datos contiene los registros de productos y movimientos.

Se genera documentación técnica y capturas del funcionamiento.

Los commits están correctamente subidos al repositorio.

🚀 Resultado esperado

Un sistema funcional que permita registrar productos nuevos y actualizar el stock con cada salida, dejando la base para las próximas iteraciones (alertas e informes).