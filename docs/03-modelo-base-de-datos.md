# 🌸 Flor Studio - Modelo de Base de Datos

## Introducción

Este documento define la estructura inicial de la base de datos de Flor Studio.

La base estará construida utilizando PostgreSQL mediante Supabase.

---

# Tabla: usuarios

Almacena los usuarios del sistema.

Campos:

- id
- nombre
- email
- contraseña
- rol
- fecha_creacion

---

# Tabla: materiales

Almacena todos los materiales utilizados.

Campos:

- id
- nombre
- categoria
- color
- imagen
- unidad_medida
- stock_actual
- stock_minimo
- costo_unitario
- proveedor_id
- fecha_creacion

Ejemplo:

Limpiapipas rosa

Unidad:
Paquete

Stock:
20 paquetes

---

# Tabla: movimientos_inventario

Registra todas las entradas y salidas de materiales.

Campos:

- id
- material_id
- tipo_movimiento

Tipos:

- COMPRA
- CONSUMO
- AJUSTE

Campos adicionales:

- cantidad
- fecha
- usuario_id
- observacion

---

# Tabla: proveedores

Información de proveedores.

Campos:

- id
- nombre
- telefono
- whatsapp
- direccion
- observaciones

---

# Tabla: productos

Productos fabricados por Flor Studio.

Campos:

- id
- nombre
- categoria
- imagen
- precio_venta
- tiempo_fabricacion
- descripcion

Ejemplo:

Rosa roja

Categoría:
Flores

Tiempo:
20 minutos

---

# Tabla: recetas

Relaciona productos con materiales.

Campos:

- id
- producto_id
- material_id
- cantidad
- unidad

Ejemplo:

Rosa roja:

6 limpiapipas

2 pistillos

1 uso floral tape

---

# Tabla: clientes

Información de clientes.

Campos:

- id
- nombre
- telefono
- whatsapp
- direccion
- cumpleaños
- fecha_registro

---

# Tabla: pedidos

Pedidos realizados.

Campos:

- id
- cliente_id
- fecha_pedido
- fecha_entrega
- estado
- costo_total
- precio_total
- ganancia

Estados:

- Pendiente
- Producción
- Terminado
- Entregado

---

# Tabla: detalle_pedido

Productos dentro de cada pedido.

Campos:

- id
- pedido_id
- producto_id
- cantidad
- precio

---

# Tabla: ventas

Registro de ventas completadas.

Campos:

- id
- pedido_id
- fecha
- metodo_pago
- total
- ganancia

---

# Relaciones principales

Usuario
|
|---- Movimientos inventario


Proveedor
|
|---- Materiales


Producto
|
|---- Recetas
        |
        |---- Materiales


Cliente
|
|---- Pedidos
        |
        |---- Detalle pedido
                    |
                    |---- Productos


---

# Consideraciones futuras

La base de datos podrá ampliarse para:

- Catálogo público.
- Código QR.
- Reportes avanzados.
- Notificaciones.
- Integración con WhatsApp.
