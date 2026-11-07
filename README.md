# FORM-FB-01 — Fichas bibliográficas: fundamentos de sistemas distribuidos y arquitecturas distribuidas

Repositorio del grupo para la actividad **FORM-FB-01** (Semana 2), asignatura Sistemas Distribuidos, Universidad Técnica Estatal de Quevedo (UTEQ).
Cada integrante entrega sus propias cinco fichas bibliográficas, con su declaración de uso de inteligencia artificial, dentro de su carpeta.

## Integrantes y carpetas

| Integrante | Carpeta |
|---|---|
| Silva Triviño John Jairo | [`silva-trivino-john-jairo/`](silva-trivino-john-jairo/) |
| Emanuel Pino Juliana Romina | [`emanuel-pino-juliana-romina/`](emanuel-pino-juliana-romina/) |
| Lombeida Escaleras Bryan Humberto | [`lombeida-escaleras-bryan-humberto/`](lombeida-escaleras-bryan-humberto/) |
| Mera Jumbo Allison Michelle | [`mera-jumbo-allison-michelle/`](mera-jumbo-allison-michelle/) |

Cada carpeta es autosuficiente: no depende de archivos de otras carpetas ni de la raíz del repositorio.

## Instrucciones de compilación (comunes a todas las carpetas)

- **Compilador:** `pdflatex`, con `biber` como motor de bibliografía (`biblatex`, estilo IEEE).
- **Archivo principal:** `main.tex`, dentro de la carpeta de cada integrante.

**Orden de comandos** (desde dentro de la carpeta):

```
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

Este proceso genera `main.pdf`. Los PDF incluidos en las carpetas pueden tener otro nombre porque se descargaron desde Overleaf, pero corresponden al mismo documento.

Alternativa en un solo comando: `latexmk -pdf main.tex`.

**Compilación en Overleaf**

1. Subir los archivos de la carpeta (`main.tex`, `referencias.bib` y, si existe, `ieee-config.sty`) a un proyecto nuevo.
2. Seleccionar el compilador `pdfLaTeX` y `main.tex` como documento principal.
3. Compilar. Si la bibliografía aparece vacía o con `?`, usar *Recompile from scratch*.

**Dependencias generales:** una distribución de LaTeX reciente (TeX Live o MiKTeX) con el programa `biber` y los paquetes `biblatex`, `babel` (español), `csquotes`, `hyperref`, `geometry`, `inputenc` y `fontenc`. Los paquetes adicionales de cada carpeta se indican abajo.

---

### silva-trivino-john-jairo

**Autor:** Silva Triviño John Jairo, Universidad Técnica Estatal de Quevedo.
**Contenido:** cinco fichas bibliográficas sobre sistemas distribuidos y arquitecturas de microservicios, con la declaración de uso de inteligencia artificial.

| Archivo | Descripción |
|---|---|
| `main.tex` | Archivo principal del documento LaTeX. |
| `referencias.bib` | Base de datos bibliográfica con las cinco fuentes. |
| `fichas_silva_trivino.pdf` | PDF compilado. |

**Dependencias adicionales:** las generales, más `enumitem` y `xcolor` si el documento los usa.

---

### emanuel-pino-juliana-romina

**Autora:** Emanuel Pino Juliana Romina, Universidad Técnica Estatal de Quevedo.
**Contenido:** cinco fichas bibliográficas sobre arquitecturas de microservicios, con la declaración de uso de inteligencia artificial.

| Archivo | Descripción |
|---|---|
| `main.tex` | Archivo principal del documento LaTeX. |
| `referencias.bib` | Base de datos bibliográfica con las cinco fuentes. |
| `fichas_bibliograficas.pdf` | PDF compilado. |

**Dependencias adicionales:** `lmodern`, `xcolor` y `enumitem`. La bibliografía usa `sorting=none`, de modo que las referencias salen en el orden en que se citan.

---

### lombeida-escaleras-bryan-humberto

**Autor:** Lombeida Escaleras Bryan Humberto, Universidad Técnica Estatal de Quevedo.
**Contenido:** cinco fichas bibliográficas sobre microservicios (rendimiento, reutilización, observabilidad y diagnóstico de fallos), con la declaración de uso de inteligencia artificial.

| Archivo | Descripción |
|---|---|
| `main.tex` | Archivo principal del documento LaTeX. |
| `ieee-config.sty` | Configuración de paquetes y de `biblatex` (estilo IEEE) que `main.tex` carga con `\usepackage{ieee-config}`. |
| `referencias.bib` | Base de datos bibliográfica con las cinco fuentes. |
| `fichas_lombeida.pdf` | PDF compilado. |

**Importante:** `ieee-config.sty` debe estar en la misma carpeta que `main.tex`; sin él, el documento no compila.

**Dependencias adicionales:** `graphicx` y `booktabs` (cargados desde `ieee-config.sty`), y `babel` con los idiomas español e inglés.

---

### mera-jumbo-allison-michelle

**Autora:** Mera Jumbo Allison Michelle, Universidad Técnica Estatal de Quevedo.
**Contenido:** cinco fichas bibliográficas sobre sistemas distribuidos y arquitecturas de microservicios, con la declaración de uso de inteligencia artificial.

| Archivo | Descripción |
|---|---|
| `main.tex` | Archivo principal del documento LaTeX. |
| `referencias.bib` | Base de datos bibliográfica con las cinco fuentes (`fuente1` a `fuente5`). |
| `ta_ind_01_fichas_AllisonMera.pdf` | PDF compilado. |

**Dependencias adicionales:** `tcolorbox` (con la biblioteca `breakable`), `enumitem` y `xcolor`.

---

## Notas

- Las referencias se verificaron abriendo su DOI o ISBN.
- Cada documento incluye la declaración de uso de inteligencia artificial de su autor.
- Los archivos auxiliares de LaTeX (`.aux`, `.bbl`, `.bcf`, `.blg`, `.run.xml`, etc.) no se suben al repositorio.
