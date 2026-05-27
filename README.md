# 📊 Análisis de Vibración por Frecuencia - Motor Eléctrico con Cargas

## 🎯 Objetivo del Análisis

Caracterizar el comportamiento vibratorio de un motor eléctrico en **tres condiciones operativas** mediante el análisis en el dominio de la frecuencia (FFT), para identificar patrones espectrales que permitan predecir fallos o sobrecargas.

---

## 📁 Datasets Recolectados

Se recolectaron **3 datasets** de aceleración (ejes X, Y, Z) bajo diferentes condiciones de carga:

| Dataset       | Condición                                 | Duración | Muestras | Archivo                  |
|---------------|-------------------------------------------|----------|----------|--------------------------|
| **Dataset 1** | 🟢 **Funcionamiento normal - Sin carga** | 60 seg   | ~100     | `datos-s.csv`       |
| **Dataset 2** | 🟡 **Carga media** (30% de capacidad)    | 60 seg   | ~100     | `datos-m.csv`  |
| **Dataset 3** | 🔴 **Carga pesada** (80% de capacidad)   | 60 seg   | ~100     | `datos-g.csv` |

### 📈 Configuración de Muestreo

- **Frecuencia de muestreo:** 100 Hz (100 muestras/segundo)
- **Ejes:** X, Y, Z (aceleración en m/s²)
- **Sensor:** Acelerómetro 
- **Condiciones ambientales:** Temperatura constante, motor fijo a bancada

---

## 🔬 Procesamiento de Datos

### 1. Limpieza y Filtrado

```python
# Filtro pasa-altas (eliminar componente de gravedad)
Fc = 0.5  # Frecuencia de corte
Fs = 100  # Frecuencia de muestreo

### 2. Graficas

<img width="839" height="456" alt="WhatsApp Image 2026-05-25 at 7 54 51 PM (2)" src="https://github.com/user-attachments/assets/0ff39f46-c9a3-4e5c-a451-913885466323" />

<img width="836" height="456" alt="WhatsApp Image 2026-05-25 at 7 54 51 PM (1)" src="https://github.com/user-attachments/assets/3a23e408-7c22-4028-9bc0-7b6e9d043d2b" />

<img width="835" height="456" alt="WhatsApp Image 2026-05-25 at 7 54 51 PM" src="https://github.com/user-attachments/assets/48cec9c9-9b21-4f38-a055-73ac3bb51c2e" />

