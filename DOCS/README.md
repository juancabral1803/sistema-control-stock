# Sistema de Control de Stock – Ingeniería del Software

**Docente:** Luis Papazoglu  
**Metodologías:** Scrum + Extreme Programming (XP)

---

##  Descripción general

El **Sistema de Control de Stock** es una aplicación web desarrollada como trabajo integrador para aplicar las metodologías ágiles **Scrum** y **Extreme Programming (XP)** en un contexto real de desarrollo de software.

El sistema permite gestionar de manera eficiente el inventario de una tienda o depósito, registrando productos, controlando movimientos de entrada y salida, mostrando alertas automáticas por bajo stock y generando informes de existencias.

---

##  Objetivo del proyecto

Diseñar, desarrollar y documentar un sistema de software aplicando los principios de las metodologías ágiles.  
Se buscó cumplir con **entregas iterativas e incrementales**, priorizando la **comunicación**, la **calidad del código** y la **satisfacción del cliente**.

---

##  Funcionalidades principales

- **Registro de productos:** permite crear, editar y eliminar artículos.  
- **Control de movimientos:** registra ingresos y salidas de stock.  
- **Alertas automáticas:** notifica productos con stock bajo.  
- **Informes en PDF:** genera reportes generales del inventario.  
- **Gestión de usuarios y roles:** controla accesos y permisos según perfil.  
- **Interfaz web responsiva:** diseño claro, moderno y fácil de usar.

---

##  Tecnologías utilizadas

| Componente              | Tecnología              |
|--------------------------|--------------------------|
| **Lenguaje backend**     | Java                     |
| **Framework**            | Spring Boot              |
| **Motor de plantillas**  | Thymeleaf                |
| **Base de datos**        | MySQL                    |
| **Testing**              | JUnit 5                  |
| **Control de versiones** | Git + GitHub             |
| **Metodologías**         | Scrum + XP               |

---

##  Estructura del repositorio

 sistema-control-stock/
┣  docs/
┃ ┣  iteracion_1/
┃ ┃ ┣  dp.md
┃ ┃ ┗  retrospectiva.md
┃ ┣  iteracion_2/
┃ ┃ ┣  dp.md
┃ ┃ ┗  retrospectiva.md
┃ ┣  iteracion_3/
┃ ┃ ┣  dp.md
┃ ┃ ┗  retrospectiva.md
┃ ┗  erp.md
┣ 📄 README.md

---

##  Ejecución del proyecto

### Requisitos previos

- Java JDK 11 o superior  
- MySQL Server  
- Maven o Gradle  
- Spring Boot 2.7+

---

### Pasos para ejecución local

**1. Clonar el repositorio:**

git clone https://github.com/<usuario>/<repositorio>.git

**2. Crear la base de datos en MySQL:**

CREATE DATABASE control_stock;

**3. Configurar las credenciales en el archivo application.properties:**

spring.datasource.url=jdbc:mysql://localhost:3306/control_stock

spring.datasource.username=tu_usuario

spring.datasource.password=tu_contraseña

**4. Ejecutar la aplicación:**

mvn spring-boot:run

**5. Abrir el navegador y acceder a:**

http://localhost:8080

## Equipo de desarrollo

|Rol	                  |Integrante                             |
|------------------------|--------------------------------------|
|Product Owner	         |Cabral Juan                           |
|Scrum Master	           |Silclir Alejandro                     |
|Equipo de Desarrollo	   |Ruiz Diaz Rocio – Silclir Alejandro   |

## Iteraciones realizadas

|Iteración	   |Objetivo principal	                   |Historias completadas        |
|--------------|---------------------------------------|-----------------------------|
|Iteración 1	 |Registro y salida de productos	       |HU1 – HU2                    |
|Iteración 2	 |Alertas e informes de stock	           |HU3 – HU4                    |
|Iteración 3	 |Optimización, seguridad e interfaz	   |HU5 – HU6 – HU7              |

## Conclusión

El proyecto cumplió con *todos los objetivos establecidos*, logrando un sistema estable, seguro y de fácil mantenimiento.
La aplicación de *Scrum* permitió organizar el trabajo en iteraciones con entregas continuas, mientras que las prácticas de *XP* (pair programming, testing, refactorización) garantizaron calidad y colaboración constante.

El resultado es un sistema funcional y escalable que refleja el valor del enfoque ágil en el desarrollo de software moderno.
