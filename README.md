# SGA·CHEM — Plataforma de Gestión de Químicos GHS/SGA

![GHS Colombia](https://img.shields.io/badge/Normativa-Res.%200773%2F2021-orange?style=flat-square)
![GHS](https://img.shields.io/badge/GHS-Rev.%209-red?style=flat-square)
![Colombia](https://img.shields.io/badge/Colombia-Decreto%201496%2F2018-yellow?style=flat-square)
![License](https://img.shields.io/badge/Licencia-MIT-blue?style=flat-square)

Herramienta web para la gestión integral de sustancias químicas peligrosas conforme al Sistema Globalmente Armonizado (SGA/GHS), adaptada al marco normativo colombiano vigente.

## ✨ Funcionalidades

| Módulo | Descripción |
|--------|-------------|
| 📊 **Dashboard** | Panel con indicadores en tiempo real: total sustancias, cobertura FDS, nivel de peligro, incompatibilidades |
| ⚗️ **Inventario** | Registro completo por sustancia: CAS, fórmula, clase GHS, nivel, frases H y P, pictogramas, ubicación, EPP |
| 🔴 **Pictogramas GHS** | Los 9 pictogramas GHS como SVG vectoriales nativos, con preselección automática al elegir la clase |
| 📋 **Matriz de compatibilidad** | Generada automáticamente al registrar sustancias; basada en NFPA 400 e ILO Chemical Safety |
| 📄 **Fichas FDS** | Seguimiento del estado de cada FDS + referencia a las 16 secciones obligatorias del GHS Rev.9 |
| ⚖️ **Normativa** | Marco legal completo: Res. 0773/2021, Decreto 1496/2018, Decreto 1072/2015, Res. 0312/2019 |

## 📐 Marco normativo

- **Resolución 0773 de 2021** — Requisitos FDS en Colombia (GHS Rev.8/9)
- **Decreto 1496 de 2018** — Adopción SGA/GHS en Colombia
- **Decreto 1072 de 2015** — SG-SST: identificación y control de riesgo químico
- **Resolución 0312 de 2019** — Estándares mínimos SG-SST
- **GHS Rev. 9 — ONU** — Estándar internacional de clasificación

## 🚀 Despliegue en GitHub Pages

```bash
# 1. Clonar o crear repositorio
git init
git add index.html README.md
git commit -m "feat: plataforma SGA·CHEM v1.0"

# 2. Subir a GitHub
git remote add origin https://github.com/TU-USUARIO/sga-chem.git
git branch -M main
git push -u origin main
```

**En GitHub → Settings → Pages → Source: `main` / `/ (root)`**

La plataforma quedará disponible en:  
`https://TU-USUARIO.github.io/sga-chem`

## 💾 Almacenamiento

Los datos se guardan en `localStorage` del navegador. Use los botones de **Exportar / Importar** para hacer respaldos en formato JSON o transferir datos entre equipos.

## 🏢 Desarrollado para

Centro de Formación Integral Providencia — Profesional SST  
Palmira, Valle del Cauca, Colombia

---
*Versión 1.0 · 2024*
