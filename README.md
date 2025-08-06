# Billing System - REST API

This project is a RESTful application built with **Spring Boot** to manage a billing system. It includes client, product, invoice, supplier management, and more.

# Skills
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![SQL](https://img.shields.io/badge/Language-SQL-4479A1?style=for-the-badge&logo=sqlite&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Hibernate](https://img.shields.io/badge/ORM-Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)
![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)




## Project Structure

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


## Project Layers

### 📁 `Entities`
Contains JPA classes representing database tables:
- `Clientes.java` (Clients)
- `Facturas.java` (Invoices)
- `Productos.java` (Products)
- `Proveedores.java` (Suppliers)
- `Detalle_Factura.java` (Invoice Details)

### `DTOEntities`
DTOs used to transport data to/from controllers:
- `ClientesDTO`
- `FacturasDTO`
- `ProductosDTO`
- `ProveedoresDTO`
- `Detalle_FacturaDTO`

### `data`
Repository interfaces extending `JpaRepository`:
- `ClienteRepository`
- `FacturaRepository`
- `ProductoRepository`
- `ProveedorRepository`
- `DetalleFacturaRepository`

### `Controllers`
REST Controllers:
- `AdminController`
- `ClienteController` (Client)
- `FacturaController` (Invoice)
- `MainController`
- `ProductoController` (Product)
- `ProveedorController` (Supplier)

---

## Main REST Endpoints

> Exact endpoints may vary based on annotations. Check files in `presentation/Controllers/` for details.

Typical examples you might find:

### ClienteController (Client)
- `GET /api/clientes` – Get all clients
- `GET /api/clientes/{id}` – Get client by ID
- `POST /api/clientes` – Create new client
- `PUT /api/clientes/{id}` – Update client
- `DELETE /api/clientes/{id}` – Delete client

### ProductoController (Product)
- `GET /api/productos`
- `POST /api/productos`
- ...

### FacturaController (Invoice)
- `GET /api/facturas`
- `POST /api/facturas`
- `GET /api/facturas/{id}`

---

## ▶️ Running the Project

### 🛠️ Requirements
- Java 17+
- Maven 3.6+
