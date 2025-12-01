# el_renacimiento
Trabajo del curso de actividades culturales en la carrera de ingeniería de sistemas.

## Cómo compilar la monografía

La carpeta `Monografia` contiene el proyecto LaTeX. Para que las referencias se resuelvan (y no aparezcan signos de interrogación en las citas), es necesario ejecutar la etapa bibliográfica con `bibtex` o `latexmk`.

### Opción rápida con `latexmk`

```bash
cd Monografia
latexmk -pdf main.tex
```

### Secuencia manual

Si no tienes `latexmk`, compila en este orden:

```bash
cd Monografia
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Las figuras se numeran automáticamente, por lo que las leyendas no deben incluir el texto "Figura XX:"; el número se añadirá al inicio de la leyenda durante la compilación.
