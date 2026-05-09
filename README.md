# Poco-M5s-Smart-FastCharge

[![Android](https://img.shields.io/badge/Android-16+-2196F3?style=flat-square&logo=android)](https://www.android.com/)
[![License](https://img.shields.io/badge/License-GPL%203.0-green?style=flat-square)](LICENSE)
[![Release](https://img.shields.io/badge/Release-v4.0-blue?style=flat-square)](https://github.com/kyosoychrisk/Poco-M5s-Smart-FastCharge/releases)

## 📱 Descripción

Módulo Magisk para carga rápida inteligente en Poco M5s. Optimiza el control térmico y la velocidad de carga mediante un sistema avanzado de gestión de batería y temperatura.

## ✨ Características

- ⚡ Carga rápida optimizada
- 🌡️ Control inteligente de temperatura
- 🔋 Gestión avanzada de batería
- 📊 Monitoreo en tiempo real
- 🎯 Compatible con Android 16+

## 🌡️ Niveles Térmicos

| Nivel | Temperatura | Estado | Acción |
|-------|------------|--------|---------|
| **Frío** | < 30°C | Normal | Carga máxima |
| **Óptimo** | 30-40°C | Ideal | Carga rápida |
| **Moderado** | 40-45°C | Alerta | Carga estándar |
| **Caliente** | 45-50°C | Advertencia | Carga reducida |
| **Crítico** | > 50°C | Peligro | Pausa de carga |

## 🚀 Instalación

1. Descarga `FastCharge_Smart.zip` desde [Releases](https://github.com/kyosoychrisk/Poco-M5s-Smart-FastCharge/releases)
2. Abre Magisk Manager
3. Ve a "Módulos" → "Instalar desde almacenamiento"
4. Selecciona el archivo ZIP descargado
5. Reinicia tu dispositivo

## 📋 Requisitos

- ✅ Magisk 25.0+
- ✅ Android 11+
- ✅ Dispositivo rooteado (Poco M5s)

## 🛠️ Configuración

El módulo se configura automáticamente. Para ajustes avanzados, edita:
```bash
/data/adb/modules/FastCharge_Smart/service.sh
```

## 📝 Cambios en v4.0

- Soporte para Android 16
- Mejora en algoritmo de control térmico
- Optimización de consumo de batería
- Interfaz mejorada

## 🤝 Contribuir

Las contribuciones son bienvenidas. Para cambios mayores:
1. Fork el repositorio
2. Crea una rama (`git checkout -b feature/mejora`)
3. Commit tus cambios (`git commit -am 'Agrega mejora'`)
4. Push a la rama (`git push origin feature/mejora`)
5. Abre un Pull Request

## ⚖️ Licencia

Este proyecto está bajo la licencia [GPL-3.0](LICENSE). Ver el archivo LICENSE para más detalles.

## 📞 Soporte

Para reportar problemas o sugerencias, abre un [Issue](https://github.com/kyosoychrisk/Poco-M5s-Smart-FastCharge/issues).

## 👤 Autor

**kyosoychrisk**

---

⭐ Si te fue útil, no olvides darle una estrella al repositorio
