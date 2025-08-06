
# 📦 Sistema de Facturación - REST API

Este proyecto es una aplicación RESTful construida con **Spring Boot** para gestionar un sistema de facturación. Incluye gestión de clientes, productos, facturas, proveedores y más.

---

## 🏗️ Estructura del Proyecto

```
InvocingSystem_RestAPI-EstebanNUEVA/
├── src/
│   ├── main/
│   │   ├── java/com/example/proyecto_2_progra_4/
│   │   │   ├── data/                  # Repositorios JPA
│   │   │   ├── logic/DTOEntities/     # Objetos DTO
│   │   │   ├── logic/Entities/        # Entidades del modelo
│   │   │   ├── presentation/Controllers/  # Controladores REST
│   │   │   ├── Proyecto2Progra4Application.java  # Clase principal
│   │   │   ├── WebConfig.java         # Configuración web
├── pom.xml                            # Configuración Maven
```

---

## 🧠 Capas del Proyecto

### 📁 `Entities`
Contiene las clases JPA que representan las tablas en la base de datos:
- `Clientes.java`
- `Facturas.java`
- `Productos.java`
- `Proveedores.java`
- `Detalle_Factura.java`

### 📁 `DTOEntities`
DTOs utilizados para transportar datos desde/hacia los controladores:
- `ClientesDTO`
- `FacturasDTO`
- `ProductosDTO`
- `ProveedoresDTO`
- `Detalle_FacturaDTO`

### 📁 `data`
Interfaces de repositorio que extienden `JpaRepository`:
- `ClienteRepository`
- `FacturaRepository`
- `ProductoRepository`
- `ProveedorRepository`
- `DetalleFacturaRepository`

### 📁 `Controllers`
Controladores REST:
- `AdminController`
- `ClienteController`
- `FacturaController`
- `MainController`
- `ProductoController`
- `ProveedorController`

---

## 🌐 Endpoints REST Principales

> ⚠️ Los endpoints exactos pueden variar según las anotaciones. Revisa los archivos en `presentation/Controllers/` para obtener más detalles.

Ejemplos típicos que podrías encontrar:

### ClienteController
- `GET /api/clientes` – Obtener todos los clientes
- `GET /api/clientes/{id}` – Obtener cliente por ID
- `POST /api/clientes` – Crear nuevo cliente
- `PUT /api/clientes/{id}` – Actualizar cliente
- `DELETE /api/clientes/{id}` – Eliminar cliente

### ProductoController
- `GET /api/productos`
- `POST /api/productos`
- ...

### FacturaController
- `GET /api/facturas`
- `POST /api/facturas`
- `GET /api/facturas/{id}`

---

## ▶️ Ejecución del Proyecto

### 🛠️ Requisitos
- Java 17+
- Maven 3.6+
