# Concepto Básico

Este indicador mide la fuerza del impulso del precio (momentum) de una manera más suave y menos ruidosa que el MACD tradicional. Usa medias móviles especiales para filtrar el ruido del mercado.

## Componentes del Indicador

### 1. Línea Verde (ImpulseMACD) - md

Es la línea principal que mide el impulso:

- **Cómo funciona:** Calcula la distancia entre el precio promedio y sus bandas superiores/inferiores
- **Encima de cero:** Impulso alcista (el precio está por encima de su rango normal)
- **Debajo de cero:** Impulso bajista (el precio está por debajo de su rango normal)
- **En cero:** Sin impulso definido (el precio está en su rango normal)

### 2. Línea Roja (Línea de Señal) - sb

Es una media móvil suavizada de la línea verde (9 períodos):

- Funciona como un filtro para confirmar cambios de tendencia
- Se mueve más lento que la línea verde

### 3. Histograma Rojo (ImpulseHisto) - sh

Son las barras verticales que muestran la diferencia entre la línea verde y la línea roja:

- **Barras grandes:** Gran diferencia entre impulso actual y su promedio (momentum fuerte)
- **Barras pequeñas:** Poca diferencia (momentum débil o cambiando)
- **Histograma creciendo:** El impulso se está fortaleciendo
- **Histograma decreciendo:** El impulso se está debilitando

### 4. Línea Gris en Cero

Es simplemente una referencia visual del nivel cero.

## Señales de Trading

**Señal Alcista:**
- Línea verde cruza por encima de línea roja
- Histograma pasa de negativo a positivo

**Señal Bajista:**
- Línea verde cruza por debajo de línea roja
- Histograma pasa de positivo a negativo

**Divergencias (importante):**
- Precio hace máximos más altos, pero indicador hace máximos más bajos = posible reversión bajista
- Precio hace mínimos más bajos, pero indicador hace mínimos más altos = posible reversión alcista

## Parámetros

- **lengthMA (34):** Período principal para calcular las bandas de impulso
- **lengthSignal (9):** Período para suavizar la señal