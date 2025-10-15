# Concepto Básico

Este indicador analiza el volumen de trading para confirmar la fuerza de las tendencias de precio. Combina el OBV (On Balance Volume) con Bandas de Bollinger y una EMA rápida.

## Componentes del Indicador

### 1. OBV (On Balance Volume) - Línea Azul

Es un indicador de volumen acumulativo que mide la presión de compra y venta:

- **Sube:** Cuando el precio cierra más alto que el cierre anterior (volumen de compra)
- **Baja:** Cuando el precio cierra más bajo que el cierre anterior (volumen de venta)

**Concepto clave:** Si el OBV sube mientras el precio sube, confirma que la tendencia alcista es fuerte (hay volumen real detrás del movimiento).

### 2. Bandas de Bollinger aplicadas al OBV

En lugar de aplicarse al precio, estas bandas se aplican al OBV para medir su volatilidad:

- **Banda Media (amarilla punteada):** SMA de 20 períodos del OBV
- **Banda Superior (roja punteada):** Indica alta presión de compra
- **Banda Inferior (verde punteada):** Indica alta presión de venta
- **Relleno verde claro:** Área entre las bandas

### 3. EMA 10 del OBV (línea morada)

Es una media rápida del OBV que detecta cambios de momentum más rápidamente.

### 4. Relleno de Color entre EMA 10 y Banda Media

- **Verde:** EMA 10 por encima de la banda media = momentum alcista en el volumen
- **Rojo:** EMA 10 por debajo de la banda media = momentum bajista en el volumen

## Cómo Interpretarlo

**Divergencias (lo más importante):**
- **Divergencia alcista:** Precio hace mínimos más bajos, pero OBV hace mínimos más altos (posible reversión al alza)
- **Divergencia bajista:** Precio hace máximos más altos, pero OBV hace máximos más bajos (posible reversión a la baja)

**Confirmación de tendencia:**
- Tendencia alcista fuerte: Precio sube Y OBV sube (relleno verde)
- Tendencia bajista fuerte: Precio baja Y OBV baja (relleno rojo)

**Señales de momentum:**
- EMA 10 cruza por encima de la banda media = aumento de presión compradora
- EMA 10 cruza por debajo de la banda media = aumento de presión vendedora