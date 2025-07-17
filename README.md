# Plantilla LaTeX para Informes de Laboratorio – ECIM TEC

Esta plantilla está diseñada para la elaboración de informes de laboratorio en la Escuela de Ciencia e Ingeniería en Materiales del Tecnológico de Costa Rica (ECIM-TEC). Incluye el formato, estructura y estilos sugeridos para reportes académicos, con manejo moderno de bibliografía, tablas, figuras y ecuaciones.

## Características

- Márgenes y tipografía profesional
- Manejo de autores con afiliación institucional
- Numeración automática de ecuaciones por sección
- Inclusión de tablas y figuras con pies personalizados
- Bibliografía automática con citas numeradas (estilo IEEE/numeric)
- Compatibilidad con Overleaf, TeXstudio y otros editores LaTeX

## Archivos incluidos

- `Plantilla_ECIM.tex`: archivo principal del informe
- `references.bib`: archivo de bibliografía de ejemplo
- Carpeta `images/`: para las imágenes de portada y figuras internas

## Estructura sugerida

1. Portada (título, autores, institución)
2. Resumen
3. Introducción
4. Objetivos (general y específicos)
5. Marco Teórico
6. Materiales y Métodos
7. Resultados y Análisis
8. Conclusiones
9. Referencias
10. Anexos

## Cómo compilar

### Opción 1: Overleaf

1. Sube todos los archivos (`Plantilla_ECIM.tex`, `references.bib`, imágenes).
2. Elige como herramienta de bibliografía: **Biber** (no BibTeX).
3. Compila normalmente. Las citas deben aparecer numeradas (`[1]`, `[2]`, etc.).

### Opción 2: TeXstudio / Local

1. Asegúrate de tener instalado **Biber**.
2. Compila con la siguiente secuencia:
    - `pdflatex Plantilla_ECIM.tex`
    - `biber Plantilla_ECIM`
    - `pdflatex Plantilla_ECIM.tex` (dos veces)
3. Si usas TeXstudio:
    - Ve al menú "Herramientas" y ejecuta “Biber” después de la primera compilación.
    - Compila dos veces más con `pdfLaTeX`.

### Nota sobre bibliografía

- La plantilla usa `biblatex` y **Biber** para el manejo moderno de referencias.
- Para agregar una cita, usa `\cite{Clave}` donde “Clave” es el identificador del artículo/libro en `references.bib`.
- En la sección “Referencias” aparecerán automáticamente todas las citas numeradas.

## Ejemplo de cita

En el texto:
```latex
Según diversos autores \cite{Cooper2009,Lozano2010,young:1902}, el análisis...
```
En la bibliografía:
```
[1] Cooper, M. Cooperative Chemistry Lab Manual, Clemson University, 2009.
[2] Lozano Urbina, L.A., et al. Manual de prácticas..., UIS, 2010.
[3] Young, S. Correction of the boiling points..., J. Chem. Soc., 1902.
```

## Requisitos

- Distribución LaTeX actualizada (TeX Live, MiKTeX, MacTeX, etc.)
- Paquete `biblatex` y compilador Biber
- (Opcional) Paquetes adicionales: `tcolorbox`, `siunitx`, `mhchem`, etc.

## Créditos

Plantilla elaborada para ECIM-TEC por **Adrián Quesada Martínez**  
Correo: adquesada@itcr.ac.cr

¿Consultas o sugerencias? ¡No dudes en contactarme!

---
