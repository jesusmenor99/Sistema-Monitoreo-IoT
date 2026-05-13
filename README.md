# Sistema-Monitoreo-IoT
Artículo IEEE sobre el proyecto de un Sistema de Monitoreo Ambiental IoT (ESP32 &amp; Cloud)
# Sistema de Monitoreo Ambiental IoT de Bajo Costo | ESP32 + Blynk


> Artículo IEEE presentado como parte del trabajo en la carrera de Implementación de Sistemas Electrónicos Industriales.  
> **Unidades Tecnológicas de Santander (UTS) - 2025**

---

## 📌 Descripción General

Este proyecto implementa una **estación de monitoreo ambiental de bajo costo (≈25 USD)** basada en IoT, capaz de medir y visualizar:

- 🌡️ **Temperatura** (precisión ±0.6°C)
- 💧 **Humedad relativa** (precisión ±4%)
- 📊 **Presión barométrica local** (precisión ±0.4 hPa)
- 🏔️ **Presión corregida a nivel del mar** (precisión ±0.7 hPa)

Los datos se muestran **localmente** en una pantalla LCD con navegación por pulsador, y **remotamente** en un dashboard de Blynk accesible desde cualquier smartphone o navegador. Una funcionalidad innovadora permite **activar/desactivar el envío a la nube** mediante un botón virtual, optimizando el uso del plan gratuito de Blynk.

---

## 🎯 Objetivo del Proyecto

Diseñar, implementar y validar un sistema de monitoreo ambiental IoT de bajo costo, fácilmente replicable para fines educativos, que combine visualización local y remota, con precisión adecuada para aplicaciones de enseñanza y prototipado rápido.

---

## ⚙️ Tecnologías y Componentes

| Categoría           | Componente / Tecnología |
|---------------------|--------------------------|
| **Microcontrolador** | ESP32-WROOM-32 (WiFi + Bluetooth integrado) |
| **Sensor temp/humedad** | DHT11 (1-wire, GPIO15) |
| **Sensor presión**  | BMP280 (I2C, dirección 0x76) |
| **Pantalla**        | LCD 1602A + módulo I2C (dirección 0x27) |
| **Entrada usuario** | Pulsador HW-483 (GPIO13, pull-up interno) |
| **Plataforma IoT**  | Blynk (pines virtuales V0–V5) |
| **Entorno desarrollo** | Arduino IDE |
| **Librerías**       | Blynk, DHT, Adafruit_BMP280, LiquidCrystal_I2C |

---

