# Concepto Básico

Esta estrategia compra y vende automáticamente basándose en el cruce de dos líneas: una EMA rápida (9 períodos) y una EMA lenta (21 períodos).

## ¿Qué es una EMA?

EMA = Media Móvil Exponencial. Es una línea que suaviza el precio y muestra la tendencia promedio. La EMA rápida (9) reacciona más rápido a los cambios de precio que la EMA lenta (21).

## Señales de Compra y Venta

**COMPRA:** Cuando la EMA de 9 cruza por encima de la EMA de 21
- Significa que el precio está subiendo con fuerza
- La estrategia entra en posición larga (compra)

**VENTA:** Cuando la EMA de 9 cruza por debajo de la EMA de 21
- Significa que el precio está bajando o perdiendo fuerza
- La estrategia cierra la posición (vende)

## Parámetros de la Estrategia

- Capital inicial: 1000 USDT
- Usa el 100% del capital en cada operación
- Solo permite 1 operación abierta a la vez (pyramiding = 1)
- Puedes definir las fechas de inicio y fin para el backtest
- Opción de colorear el fondo: verde cuando EMA 9 > EMA 21, rojo cuando EMA 9 < EMA 21

## Visualización

- Etiqueta verde "Buy" aparece debajo de la vela cuando hay señal de compra
- Etiqueta roja "Sell" aparece encima de la vela cuando hay señal de venta