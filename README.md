# SGA·CHEM — Plataforma de Gestión de Químicos GHS/SGA

![GHS Colombia](https://img.shields.io/badge/Normativa-Res.%200773%2F2021-orange?style=flat-square)
![GHS](https://img.shields.io/badge/GHS-Rev.%209-red?style=flat-square)
![Colombia](https://img.shields.io/badge/Colombia-Decreto%201496%2F2018-yellow?style=flat-square)
![License](https://img.shields.io/badge/Licencia-MIT-blue?style=flat-square)
![Version](https://img.shields.io/badge/Versión-2.0-green?style=flat-square)

Herramienta web para la gestión integral de sustancias químicas peligrosas conforme al Sistema Globalmente Armonizado (SGA/GHS), adaptada al marco normativo colombiano vigente. Funciona como archivo único `index.html` — sin instalación, sin servidor, desplegable en GitHub Pages.

---

## ✨ Funcionalidades

| Módulo | Descripción |
|--------|-------------|
| 📊 **Dashboard** | Panel con indicadores en tiempo real: total sustancias, cobertura FDS, peligro alto, incompatibilidades detectadas y barra de cumplimiento FDS |
| ⚗️ **Inventario** | Registro completo por sustancia: CAS, fórmula, sinónimo, clase GHS, nivel, frases H y P, pictogramas, ubicación, EPP, proveedor, estado FDS |
| 🔺 **Pictogramas GHS** | Los 9 pictogramas oficiales (Res. 0773/2021 / Decreto 1496/2018) redibujados en SVG vectorial: rombo rojo, figura negra, fondo blanco. Con código GHS, nombre oficial y descripción técnica |
| 🗂️ **Matriz de compatibilidad** | Generada automáticamente al registrar sustancias; basada en NFPA 400 e ILO Chemical Safety. Tres estados: Compatible / Precaución / Incompatible |
| 📄 **Fichas FDS** | Carga directa del PDF de la FDS por sustancia, almacenado en el sistema. Visualización en línea. Tabla de seguimiento de estado por sustancia + 16 secciones obligatorias GHS Rev.9 |
| ⚖️ **Normativa** | Marco legal completo: Res. 0773/2021, Decreto 1496/2018, Decreto 1072/2015, Res. 0312/2019, Res. 2400/1979, GHS Rev.9, NFPA 400, Ley 1252/2008 |

---

## 🔺 Pictogramas GHS incluidos

Los 9 pictogramas oficiales adoptados por Colombia, fieles a la imagen de referencia normativa:

| Código | Nombre oficial |
|--------|---------------|
| GHS01 | Peligro de Explosivos |
| GHS02 | Inflamable |
| GHS03 | Carburante / Oxidante |
| GHS04 | Gases bajo presión |
| GHS05 | Corrosión |
| GHS06 | Toxicidad (calavera y tibias) |
| GHS07 | Químico Nocivo (exclamación) |
| GHS08 | Daño al Medio Ambiente |
| GHS09 | Peligro para la Salud |

---

## 📋 Campos de registro por sustancia

- **Identificación:** nombre, CAS, fórmula química, sinónimo/nombre comercial, área/proceso, proveedor
- **Clasificación GHS:** clase de peligro, categoría, frases H (peligro), frases P (prudencia)
- **Pictogramas:** selección múltiple con preselección automática según clase de peligro
- **Almacenamiento:** cantidad, estado físico, tipo de recipiente, ubicación
- **FDS:** estado (disponible / pendiente / no disponible), nombre de archivo, versión, idioma, **carga directa del PDF** (máx. 15 MB), visualización en línea

---

## 📐 Marco normativo

| Norma | Alcance |
|-------|---------|
| **Resolución 0773 de 2021** | Requisitos FDS en Colombia — GHS Rev.8/9 |
| **Decreto 1496 de 2018** | Adopción SGA/GHS en Colombia |
| **Decreto 1072 de 2015** | SG-SST: identificación y control del riesgo químico |
| **Resolución 0312 de 2019** | Estándares mínimos SG-SST |
| **Resolución 2400 de 1979** | Almacenamiento y manipulación de sustancias peligrosas |
| **GHS Rev. 9 — ONU** | Estándar internacional de clasificación y etiquetado |
| **NFPA 400** | Código de materiales peligrosos — base matriz de compatibilidad |
| **Ley 1252 de 2008** | Residuos peligrosos (RESPEL) |

---

## 🚀 Despliegue en GitHub Pages

```bash
# 1. Inicializar repositorio local
git init
git add index.html README.md
git commit -m "feat: plataforma SGA·CHEM v2.0"

# 2. Subir a GitHub
git remote add origin https://github.com/TU-USUARIO/sga-chem.git
git branch -M main
git push -u origin main
```

**En GitHub → Settings → Pages → Source: `main` / `/ (root)`**

La plataforma quedará publicada en:
```
https://TU-USUARIO.github.io/sga-chem
```

> Solo se necesitan **dos archivos**: `index.html` y `README.md`. No requiere dependencias, build tools ni servidor.

---

## 💾 Gestión de datos

| Función | Descripción |
|---------|-------------|
| **localStorage** | Los datos persisten en el navegador automáticamente |
| **Exportar JSON** | Descarga un backup completo del inventario (incluye PDFs en base64) |
| **Importar JSON** | Restaura o fusiona un backup previo |
| **PDF FDS** | Almacenado en base64 dentro del registro de cada sustancia |

> ⚠️ Los datos de localStorage son locales al navegador y equipo. Use **Exportar** regularmente para respaldar su inventario.

---

## 🏢 Desarrollado para

Centro de Formación Integral Providencia  
Profesional SST — Palmira, Valle del Cauca, Colombia

---

*Versión 2.0 · 2024 — Pictogramas GHS oficiales + Carga PDF FDS*
