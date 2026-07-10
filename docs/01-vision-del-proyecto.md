# 🌸 Flor Studio

## Visión del proyecto

Flor Studio será una Aplicación Web Progresiva (PWA) diseñada para administrar un taller de flores artesanales hechas con limpiapipas.

El objetivo es crear un sistema completo de gestión que permita controlar inventario, materiales, compras, producción, costos, clientes, pedidos y ventas desde una sola plataforma.

---

# Objetivo principal

Crear una herramienta que permita conocer:

- Cuánto cuesta fabricar cada producto.
- Cuánto material se necesita.
- Cuánto tiempo requiere la producción.
- Cuál es la ganancia real.
- Cuándo comprar materiales.
- Cómo organizar la producción.

---

# Usuarios iniciales

## Cuchurrumi

Administrador.

Permisos:
- Gestión completa del sistema.
- Inventario.
- Compras.
- Producción.
- Ventas.
- Reportes.

## Araguatita

Administradora.

Permisos:
- Gestión completa del sistema.

---

# Módulos principales

## Dashboard

Panel principal con:

- Ventas del día.
- Ventas del mes.
- Ganancias.
- Pedidos pendientes.
- Alertas de inventario.
- Productos más vendidos.

---

## Inventario

Control de materiales:

- Limpiapipas.
- Silicón.
- Papel coreano.
- Floral tape.
- Pistillos.
- Cajas.
- Decoraciones.

Cada material tendrá:

- Nombre.
- Categoría.
- Color.
- Proveedor.
- Costo.
- Cantidad disponible.
- Stock mínimo.

---

## Productos

Gestión de productos:

- Flores.
- Ramos.
- Cuadros.
- Lámparas.
- Personalizados.

---

## Recetas

Cada producto tendrá una receta de fabricación.

Ejemplo:

Rosa roja:

- 6 limpiapipas.
- 2 pistillos.
- 1 uso de floral tape.
- 0.5 usos de silicón.

La aplicación calculará automáticamente el costo.

---

## Costos

Cálculo:

Materiales
+
Mano de obra
+
Gastos indirectos

=

Costo real

Luego calculará precio recomendado de venta.

---

# Tecnología

Frontend:
- Next.js
- TypeScript
- Tailwind CSS

Backend:
- Supabase

Base de datos:
- PostgreSQL

Autenticación:
- Supabase Auth

---

# Roadmap

## Fase 1

- Usuarios.
- Inventario.
- Productos.
- Recetas.
- Cálculo de costos.

## Fase 2

- Compras.
- Proveedores.
- Clientes.
- Pedidos.
- Producción.

## Fase 3

- Reportes avanzados.
- Catálogo público.
- Integración WhatsApp.
- Asistente Flora.
