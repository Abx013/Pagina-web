# Baymax · Panel de exposición

Panel web para el proyecto escolar Baymax. Está pensado para funcionar desde **celular o laptop** durante la exposición.

## Dos formas de usarlo

### 1) Modo demostración / respaldo
Abre la página publicada con GitHub Pages. Permite:
- ver temperatura, peso, altura, IMC y distancia simulados;
- controlar el movimiento en modo demostración;
- probar la secuencia completa de evaluación;
- simular voz, buzzer y estado del robot;
- registrar manualmente presión arterial y glucosa.

Este modo sirve aunque el robot todavía no tenga todos los sensores conectados.

### 2) Modo real con ESP32
Para la exposición, el ESP32 debe crear su propia red Wi‑Fi:

- Red: **Baymax-Expo**
- Contraseña: **BaymaxExpo2026**
- Dirección habitual: **http://192.168.4.1**

Conecta el celular o laptop a esa red y abre la dirección anterior. Así no dependes del Wi‑Fi de la escuela.

El modo real está preparado para:
- MLX90614: temperatura;
- HX711 + 4 celdas: peso;
- VL53L1X: altura;
- cálculo automático del IMC;
- HC-SR04: distancia/obstáculos;
- TB6612FNG + 2 motores: movimiento;
- DFPlayer Mini: frases de voz;
- buzzer: avisos;
- presión y glucosa: registro manual con equipos externos.

## Recomendación para el día de la exposición

1. Llevar el panel de GitHub Pages abierto como respaldo.
2. Encender Baymax.
3. Conectarse a **Baymax-Expo**.
4. Abrir **http://192.168.4.1**.
5. Usar **Evaluación automática** para mostrar el flujo completo.
6. Si un sensor falla, cambiar a demostración y continuar la exposición sin detenerse.

> Prototipo educativo. Las mediciones no sustituyen dispositivos médicos certificados ni valoración profesional.
