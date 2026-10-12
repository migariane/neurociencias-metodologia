# Neurociencias: Introducción a la Metodología Científica

Material docente del Máster Universitario en Neurociencias Básicas, Aplicadas y Dolor (Universidad de Granada). Dos temas que cubren el ciclo completo de la investigación sanitaria: cómo se diseña y se lee un estudio cualitativo, y cómo se mide, se estima y se contrasta en un estudio cuantitativo.

Cada tema está disponible de dos formas: una presentación web navegable (Quarto RevealJS) y un PDF listo para imprimir o proyectar (Beamer).

Miguel Angel Luque-Fernández, Departamento de Estadística e Investigación Operativa, Universidad de Granada

---

## Temas

### T01. Investigación Cualitativa

Fundamentos de la metodología cualitativa, validez diagnóstica (sensibilidad, especificidad, valores predictivos, curvas ROC), práctica basada en la evidencia, bases de datos bibliográficas y estrategias de revisión.

- [Ver en el navegador](https://migariane.github.io/neurociencias-metodologia/T01_Investigacion_Cualitativa.html)
- [Descargar PDF](pdf/T01_Investigacion_Cualitativa.pdf), 39 diapositivas

### T02. Investigación Cuantitativa

Demografía sanitaria y medidas de frecuencia, fundamentos cuantitativos (tipos de variables, medidas de posición y dispersión), epidemiología (riesgo, odds ratio, tasas) y un supuesto práctico resuelto paso a paso.

- [Ver en el navegador](https://migariane.github.io/neurociencias-metodologia/T02_Investigacion_Cuantitativa.html)
- [Descargar PDF](pdf/T02_Investigacion_Cuantitativa.pdf), 38 diapositivas

---

## Contenido del repositorio

```
.
├── index.html                        # Portada del sitio
├── T01_Investigacion_Cualitativa.html
├── T02_Investigacion_Cuantitativa.html
├── pdf/                              # Versiones Beamer para imprimir
│   ├── T01_Investigacion_Cualitativa.pdf
│   └── T02_Investigacion_Cuantitativa.pdf
├── assets/                           # Figuras e imágenes
├── sources/                          # Código fuente (Quarto + LaTeX)
│   ├── *.qmd, _quarto.yml            # Fuentes Quarto
│   ├── ugr-scientific-theme.scss     # Tema UGR Scientific (vigente)
│   ├── madrid-theme.scss             # Tema anterior (referencia)
│   ├── references.bib                # Bibliografía
│   └── beamer/*.tex                  # Fuentes Beamer
├── LICENSE
└── NOTICE
```

El sitio está publicado con GitHub Pages a partir de la raíz del repositorio.

---

## Reproducir la compilación

Necesitas [Quarto](https://quarto.org) (probado con 1.9.x) y, para los PDF, una distribución de LaTeX con `xelatex`.

```bash
# Sitio web (genera _site/)
cd sources
quarto render

# PDF Beamer
cd beamer
TEXINPUTS=../../../Preambles:$TEXINPUTS xelatex T01_Investigacion_Cualitativa.tex
TEXINPUTS=../../../Preambles:$TEXINPUTS xelatex T02_Investigacion_Cuantitativa.tex
```

---

## Licencia

MIT. Consulta [LICENSE](LICENSE). El alcance exacto (y qué no cubre) está detallado en [NOTICE](NOTICE).

---

## Autor

Miguel Angel Luque-Fernández
Departamento de Estadística e Investigación Operativa, Universidad de Granada

- Correo: [mluquefe@ugr.es](mailto:mluquefe@ugr.es)
- Web: [migariane.github.io](https://migariane.github.io)
- Publicaciones: [maluque.netlify.app](https://maluque.netlify.app)
- Google Scholar: [scholar.google.es/citations?user=lA11XToAAAAJ](https://scholar.google.es/citations?hl=es&user=lA11XToAAAAJ)
- GitHub: [github.com/migariane](https://github.com/migariane)
- Universidad de Granada: [www.ugr.es](https://www.ugr.es)
- Departamento de Estadística e I.O.: [estadistica.ugr.es](https://www.ugr.es/~estadis/)

---

## Palabras clave

metodología científica, bioestadística, investigación cualitativa, investigación cuantitativa, epidemiología, demografía sanitaria, validez diagnóstica, sensibilidad, especificidad, curvas ROC, práctica basada en la evidencia, revisiones sistemáticas, estadística médica, neurociencias, docencia universitaria, Quarto, RevealJS, Beamer, LaTeX, educación abierta
