# Autoventas Duarte | Plataforma Automotriz de Alta Gama & Centro de Control

> **Ubicación Oficial**: Calzada Roosevelt 7-24 Zona 2, Mixco, Guatemala  
> **PBX / WhatsApp**: +502 5717-5666 (`wa.me/50257175666`)  
> **Línea Gráfica**: Rojo Duarte Deportivo (`#DC2626`), Carbono Obsidiana (`#050608`), Acentos Líquidos Trans translúcidos y Tipografía *Plus Jakarta Sans*.  
> **Regla de Oro**: CERO EMOJIS (100% iconografía vectorial SVG limpia).

---

## Enlaces Principales del Proyecto

- **Showroom Público (Landing Page + Catálogo)**: [index.html](file:///c:/Users/josej/OneDrive/Desktop/carros%201/index.html)
- **Centro de Control Administrativo (Gestión de Stock & Leads)**: [admin.html](file:///c:/Users/josej/OneDrive/Desktop/carros%201/admin.html)

---

## Módulos y Arquitectura Técnica

### 1. Showroom y Experiencia Pública (`index.html`)
- **Animación Cinemática al Abrir**: Velo preloader con monograma cromado y revelado escalonado sin saltos de interfaz.
- **Hero Section Editorial**: Titular de alta gama con micro-etiqueta de sala, botones en píldora, métricas de confianza y escaparate focal con conmutador dinámico de vehículos.
- **4 Tarjetas Cuadradas de Garantías (`[ 01 ]` al `[ 04 ]`)**:
  - `[ 01 ]` Importación Directa & Carfax Oficial
  - `[ 02 ]` Visacuotas & Financiamiento Bancario
  - `[ 03 ]` Garantía Mecánica Multipunto (120 puntos)
  - `[ 04 ]` Traspaso Inmediato & Póliza SAT
- **Motor de Búsqueda y Filtros Avanzados (2x4)**: Filtrado reactivo en JavaScript por marca, tipo, año, transmisión, tracción, presupuesto, estado y método de pago.
- **Catálogo Interactivo con Modal Multi-Foto**: Cada auto importado cuenta con 5 fotografías reales de inspección (frontal, lateral, habitáculo, motor y certificación Carfax).
- **Calculadora de Visacuotas & Agendamiento**:
  - Cálculo instantáneo de cuotas mensuales a 12, 24, 36 y 48 meses con slider de enganche (15% a 60%).
  - Selector de fechas interactivas para los próximos 14 días.
  - Generación automática de mensaje pre-llenado hacia WhatsApp y sincronización instantánea con el centro de control.
- **Preguntas Frecuentes (*Liquid Glass*)**: Acordeón con estética de cristal líquido translúcido y animación fluida mediante CSS Grid (`grid-rows-[0fr]` a `grid-rows-[1fr]`).
- **Sede Roosevelt: Visor Circular de Google Maps**: Integración del mapa oficial de Google Maps en un bisel circular de precisión con conmutador entre *Modo Noche Lujo* y *Modo Satélite/Estándar*, además de estimaciones de tiempo de llegada en vivo.

---

### 2. Centro de Control Administrativo (`admin.html`)
- **Métricas y KPIs en Tiempo Real**: Total de vehículos en inventario, unidades disponibles, autos vendidos y valor acumulado en Quetzales.
- **Gestión de Stock de Vehículos**:
  - Botón de acción rápida para conmutar un vehículo entre **Disponible** y **Vendido** (actualiza el catálogo público en vivo con etiqueta sobreimpresa).
  - Eliminación y filtrado por estado.
- **Publicador de Nuevos Autos**: Formulario con carga de datos técnicos (marca, modelo, año, tracción, transmisión, precio, cuota y fotografías).
- **Bandeja de Mensajes y Citas Recibidas (Leads)**:
  - Registro cronológico de solicitudes generadas desde la calculadora pública.
  - Detalle del vehículo de interés, enganche, cuota calculada, fecha y hora de la visita solicitada.
  - Botón de un clic para contactar directamente al cliente vía WhatsApp.
- **Sincronización Bidireccional (`localStorage`)**: Las acciones efectuadas en el panel administrativo impactan de inmediato el catálogo público sin requerir recargar base de datos externa.

---

## Instrucciones para Despliegue en GitHub

Para subir este proyecto a tu cuenta de GitHub, ejecuta los siguientes comandos en tu terminal de Git / PowerShell:

```bash
# 1. Crear el repositorio en github.com (ej. "autoventas-duarte")

# 2. Conectar el repositorio remoto (reemplaza con tu usuario y repo):
git remote add origin https://github.com/TU-USUARIO/autoventas-duarte.git

# 3. Asignar rama principal y subir el proyecto:
git branch -M main
git push -u origin main
```
