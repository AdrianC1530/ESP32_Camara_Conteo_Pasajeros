# ESP32-CAM: conteo de pasajeros

Firmware del prototipo de **conteo de pasajeros en tiempo real** desarrollado para la tesis
[TAXIBOCARCHI](https://github.com/AdrianC1530/TAXIBOCARCHI). La placa **ESP32-CAM** captura imágenes
y las envía por WiFi al servidor de detección.

## Evolución

| Carpeta | Qué es |
|---|---|
| `CameraWebServer/` | Primera prueba de la cámara, basada en el ejemplo oficial de Espressif. |
| `esp32_camera/` | Primer firmware propio: captura y envío de imágenes. |
| `esp32_camera_v2/` | Segunda versión del firmware. |
| `prototipo_final/` | Versión final usada en el prototipo de la tesis. |

## Configuración

Antes de cargarlo en la placa, completar en el `.ino`:

```cpp
#define WIFI_SSID "TU_RED_WIFI"
#define WIFI_PASSWORD "TU_CLAVE_WIFI"
#define SERVIDOR_URL "http://IP_DEL_SERVIDOR:PUERTO/deteccion"
```

## Tecnologías

ESP32-CAM (ESP32 Arduino Core 2.0.4), Arduino IDE, C++.
