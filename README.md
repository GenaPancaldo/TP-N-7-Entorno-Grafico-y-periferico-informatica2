# TP-N-7-Entorno-Grafico-y-periferico-informatica2
* Trabajo realizado por Genaro Pancaldo y Facundo Ponzo
## Descripción del Proyecto
Este proyecto implementa una interfaz gráfica de usuario desarrollada en **Processing** para el monitoreo y control bidireccional de entradas y salidas digitales de una placa **Arduino** a través de comunicación serie (USB).

### Características principales
* **Monitoreo de Entradas (`E1` y `E2`):** Refleja en tiempo real el estado lógico (ALTO/BAJO) de dos pulsadores físicos conectados al Arduino mediante indicadores de color.
* **Control de Salidas desde PC (`L1` y `L2`):** Permite encender o apagar dos LEDs físicos haciendo clic directamente sobre los indicadores gráficos en pantalla con el mouse.
* **Control Local desde Arduino:** Presionar los pulsadores físicos alterna el estado del LED correspondiente y actualiza la interfaz gráfica automáticamente para mantener ambos sistemas sincronizados.

## Conexiones

* | **Pulsador E1** | Pin Digital `2` | Configurado como `INPUT_PULLUP` (conectar el otro terminal a `GND`) |
* | **Pulsador E2** | Pin Digital `3` | Configurado como `INPUT_PULLUP` (conectar el otro terminal a `GND`) |
* | **LED L1** | Pin Digital `8` | En serie con resistencia limitadora de $220\Omega$ hacia `GND` |
* | **LED L2** | Pin Digital `9` | En serie con resistencia limitadora de $220\Omega$ hacia `GND` |


## Instrucciones de Ejecución
1. Armar el circuito según el esquema detallado arriba y conectar el Arduino a la PC por USB.
2. Abrir `arduino_control.ino` en el **IDE de Arduino**, seleccionar la placa y el puerto correspondiente, y subir el código. *(Cerrar el Monitor Serie antes de continuar para no ocupar el puerto)*.
3. Abrir `interfaz_processing.pde` en **Processing** y ejecutar el sketch.

<img width="1086" height="532" alt="image" src="https://github.com/user-attachments/assets/546b6593-5f58-4025-82c0-2484ac9c6dbc" />
