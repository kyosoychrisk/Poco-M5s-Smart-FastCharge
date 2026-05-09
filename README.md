# ⚡ Poco M5s Smart FastCharge (Rosemary)
Módulo para APatch/Magisk diseñado para desbloquear y gestionar inteligentemente la carga rápida en el **Poco M5s** (rosemary). Especialmente útil para ROMs AOSP como Evolution X, donde la velocidad de carga por defecto suele estar muy limitada o ser inestable.
## 🧠 Lógica de Control Térmico Inteligente
A diferencia de otros módulos que fuerzan la carga al máximo constantemente (arriesgando la vida útil de la batería), este script implementa **escalones térmicos** similares a los del kernel stock de Xiaomi. El módulo ajusta el amperaje en tiempo real según la temperatura actual del dispositivo:

| Temperatura | Modo de Carga | Amperaje Máximo |
| :--- | :--- | :--- |
| **Menos de 39°C** | 🟢 Ultra Rápido | ~4500 mA (Aprovechando los 33W) |
| **De 39°C a 43°C** | 🟡 Balanceado | ~2800 mA |
| **De 43°C a 45°C** | 🟠 Enfriamiento | ~1500 mA |
| **Más de 45°C** | 🔴 Protección | ~500 mA (Previene sobrecalentamiento) |

## 📱 Requisitos
- **Dispositivo:** Poco M5s (rosemary) con MediaTek Helio G95.
- **Root:** APatch (Recomendado) o Magisk.
- **Sistema:** Probado en ROMs AOSP (Android 14, 15 y Android 16 Baklava).
## 🛠️ Instalación
1. Ve a la sección de [Releases](../../releases) a la derecha de esta página y descarga el archivo `FastCharge_Smart.zip` más reciente.
2. Abre tu gestor de root (APatch o Magisk).
3. Ve a la pestaña de Módulos, selecciona instalar desde el almacenamiento y elige el archivo `.zip`.
4. **Reinicia el dispositivo.**
5. *Nota técnica:* El script tiene un retraso programado (`sleep 40`) para evitar conflictos durante el arranque del sistema. Espera aproximadamente un minuto tras encender el equipo para conectar el cargador y ver los resultados en Ampere.
## ⚠️ Disclaimer
> Tu garantía ya está anulada. Modificar los perfiles de carga siempre conlleva un riesgo. No me hago responsable por dispositivos dañados o baterías degradadas. Monitorea la temperatura de tu equipo durante los primeros ciclos de uso para asegurar que el control térmico actúa correctamente.