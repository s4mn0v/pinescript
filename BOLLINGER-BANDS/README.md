# Concepto Básico

Este indicador combina dos herramientas de análisis técnico: EMAs para identificar tendencias y Bandas de Bollinger para medir volatilidad y niveles de sobrecompra/sobreventa.

## Componentes del Indicador

### 1. Bandas de Bollinger

Son tres líneas que forman un canal alrededor del precio:

- **Banda Superior (roja):** Indica posible zona de sobrecompra
- **Banda Media (azul punteada):** Es el promedio móvil de 20 períodos, muestra el precio medio
- **Banda Inferior (verde):** Indica posible zona de sobreventa
- **Relleno morado:** El área entre las bandas superior e inferior muestra la volatilidad del mercado

**Configuración:** 
- Usa SMA de 20 períodos por defecto
- Desviación estándar de 2.0
- Puedes cambiar el tipo de media móvil (SMA, EMA, WMA, etc.)

### 2. EMAs (Medias Móviles Exponenciales)

- **EMA 9 (línea roja):** Media rápida que sigue de cerca el precio actual
- **EMA 21 (línea verde):** Media más lenta que indica la tendencia de mediano plazo

### 3. Relleno de Color entre EMA 9 y Banda Media

- **Verde:** Cuando EMA 9 está por encima de la banda media (tendencia alcista)
- **Rojo:** Cuando EMA 9 está por debajo de la banda media (tendencia bajista)

## Cómo Interpretarlo

**Señales Alcistas:**
- Precio por encima de la banda media
- EMA 9 por encima de la banda media (relleno verde)
- EMA 9 por encima de EMA 21

**Señales Bajistas:**
- Precio por debajo de la banda media
- EMA 9 por debajo de la banda media (relleno rojo)
- EMA 9 por debajo de EMA 21

**Volatilidad:**
- Bandas anchas = alta volatilidad
- Bandas estrechas = baja volatilidad (posible ruptura próxima)
