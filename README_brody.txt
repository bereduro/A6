


          
# Snake Game con Abstract Factory Pattern

## Autor
BRODY DEIBY VELARDE HURTADO

## Descripción
Este proyecto implementa el clásico juego Snake utilizando el patrón de diseño Abstract Factory en Python. El juego presenta una serpiente que puede consumir diferentes tipos de comida, cada una con efectos únicos sobre el juego.

## Características

### Tipos de Comida
- 🟣 **Comida Venenosa**
  - Color: Morado
  - Efecto: Reduce un punto y elimina un segmento de la serpiente

- 🟢 **Comida Fit**
  - Color: Verde
  - Efecto: Añade un punto y un segmento

- 🟡 **Comida Alto en Grasas**
  - Color: Amarillo
  - Efecto: Añade 3 puntos y 3 segmentos
  - Efecto secundario: Ralentiza la serpiente por 5 segundos

- 🟠 **Comida para Reyes**
  - Color: Naranja
  - Efecto: Añade 5 puntos y 5 segmentos
  - Efecto secundario: Aumenta la velocidad

### Controles
- ⬆️ Flecha Arriba: Mover hacia arriba
- ⬇️ Flecha Abajo: Mover hacia abajo
- ⬅️ Flecha Izquierda: Mover hacia la izquierda
- ➡️ Flecha Derecha: Mover hacia la derecha
- 'r': Reiniciar juego (después de perder)
- 'e': Salir del juego

### Características de la Serpiente
- Cabeza cuadrada de color verde brillante
- Cuerpo con segmentos circulares en tonos alternados de verde
- Velocidad adaptativa según el tipo de comida consumida

## Implementación del Patrón Abstract Factory

### Interfaces Abstractas
- `Comida`: Define la interfaz para los diferentes tipos de comida
- `FabricaComida`: Define la interfaz para crear diferentes tipos de comida

### Clases Concretas
- Comidas: `ComidaVenenosa`, `ComidaFit`, `ComidaAltoEnGrasas`, `ComidaParaReyes`
- Fábricas: `FabricaComidaVenenosa`, `FabricaComidaFit`, `FabricaComidaAltoEnGrasas`, `FabricaComidaParaReyes`

## Requisitos
- Python 3.x
- Módulo `turtle` (incluido en la biblioteca estándar de Python)

## Cómo Jugar
1. Ejecuta el script Python
2. Usa las flechas del teclado para dirigir la serpiente
3. Recoge diferentes tipos de comida para crecer y ganar puntos
4. Evita chocar con los bordes y con tu propio cuerpo
5. Cuando pierdas, elige entre reiniciar ('r') o salir ('e')

        