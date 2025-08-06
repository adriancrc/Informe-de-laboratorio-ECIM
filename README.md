# 📄 Plantilla LaTeX para Informes de Laboratorio – ECIM TEC

[![Made with LaTeX](https://img.shields.io/badge/Made%20with-LaTeX-blue)](https://www.latex-project.org/)
![License](https://img.shields.io/github/license/adriancrc/Plantilla-Informes-Latex-ECIM)
![Platform](https://img.shields.io/badge/Platform-Overleaf%20%7C%20TeXstudio-lightgrey)
![Educational Use](https://img.shields.io/badge/Use-Educational-important)
![Author](https://img.shields.io/badge/Author-Adrián%20Quesada%20Martínez-blueviolet)
![Developed at ITCR](https://img.shields.io/badge/Developed%20at-ITCR-blue)

Plantilla diseñada para la elaboración de informes de laboratorio en la **Escuela de Ciencia e Ingeniería en Materiales del Tecnológico de Costa Rica (ECIM-TEC)**. Ofrece un formato profesional y moderno, compatible con **Overleaf**, **TeXstudio** y otros editores LaTeX, integrando buenas prácticas para redacción académica y científica.

---

## ✨ Características principales

- Márgenes y tipografía profesional adaptados al estilo institucional
- Manejo de múltiples autores con afiliación académica
- Numeración automática de ecuaciones por sección
- Inserción de tablas y figuras con pies personalizables
- Citado automático mediante `biblatex` (estilo IEEE/numeric)
- Compatible con **Biber** para bibliografía moderna
- Totalmente funcional en Overleaf, TeXstudio y entornos locales

---

## 📁 Archivos incluidos

- `Plantilla_ECIM.tex` – Archivo principal del informe
- `references.bib` – Archivo de bibliografía de ejemplo
- `images/` – Carpeta para portada y figuras internas

---

## 🧱 Estructura sugerida del informe

1. Portada (título, autores, institución)
2. Resumen
3. Introducción
4. Objetivos (general y específicos)
5. Marco teórico
6. Materiales y métodos
7. Resultados y análisis
8. Conclusiones
9. Referencias
10. Anexos

---

## ⚙️ Instrucciones para compilar

### 🔹 Opción 1: Overleaf

1. Sube todos los archivos: `Plantilla_ECIM.tex`, `references.bib`, e imágenes.
2. En “Settings”, elige **Biber** como herramienta de bibliografía.
3. Compila normalmente. Las citas aparecerán como `[1]`, `[2]`, etc.

### 🔹 Opción 2: Compilación local (TeXstudio, etc.)

1. Asegúrate de tener **Biber** instalado.
2. Ejecuta en este orden:

```bash
pdflatex Plantilla_ECIM.tex
biber Plantilla_ECIM
pdflatex Plantilla_ECIM.tex
pdflatex Plantilla_ECIM.tex
```

> 💡 En **TeXstudio**, podés ir al menú `Herramientas > Biber`, y luego compilar dos veces más con `pdfLaTeX`.

---

## 📚 Notas sobre bibliografía

- El archivo `references.bib` utiliza el formato BibTeX estándar.
- La plantilla usa `biblatex` con estilo **numeric** (similar a IEEE).
- Para citar: `\cite{Clave}` (donde `Clave` es el identificador en el archivo `.bib`).
- Las referencias se insertan automáticamente al compilar con Biber.

---

## 📝 Ejemplo de cita

En el código fuente:

```latex
Según diversos autores \cite{Cooper2009,Lozano2010,young:1902}, el análisis...
```

Se verá en el PDF así:

```
[1] Cooper, M. Cooperative Chemistry Lab Manual, Clemson University, 2009.
[2] Lozano Urbina, L.A., et al. Manual de prácticas..., UIS, 2010.
[3] Young, S. Correction of the boiling points..., J. Chem. Soc., 1902.
```

---

## 🧰 Requisitos del sistema

- Distribución LaTeX actualizada (TeX Live, MiKTeX, MacTeX, etc.)
- Paquetes requeridos:
  - `biblatex`
  - `biber`
  - (Opcional) `tcolorbox`, `siunitx`, `mhchem`, entre otros

---

## 👨‍🏫 Créditos

Plantilla desarrollada para ECIM-TEC por:  
**Adrián Quesada Martínez**  
📧 [adquesada@itcr.ac.cr](mailto:adquesada@itcr.ac.cr)

¿Consultas, sugerencias o mejoras? ¡No dudes en escribirme!
