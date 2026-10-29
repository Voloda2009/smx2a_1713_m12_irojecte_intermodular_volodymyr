## 1.Uso de complementos (plugins)
<br>

### Para mayor comodidad y estilo en la presentación de La Taula del Barri, agregué los complementos básicos de MkDocs:
- mkdocs-material (diseño adaptativo y temas).
- mkdocs-material (diseño adaptativo y temas).

## 2.Configuración y despliegue
<br>

### ¿Qué es mkdocs.yml?
#### L'arxiu mkdocs.yml és el fitxer de configuració principal del vostre lloc web estàtic. Hi s'defineix el títol del projecte, el tema visual, l'estructura de la barra de navegació superior i els complements (plugins) actius.
<br>

- Ejemplo de cambio:

```python
site_name: La Taula del Barri
theme:
  name: material
```
<br>

### ¿Qué es deploy.yml?
#### L'arxiu deploy.yml (ubicat generalment a .github/workflows/deploy.yml) forma part de GitHub Actions. La seva funció és automatitzar el procés de construcció (build) i publicació (deploy) de la web cada vegada que es puja (push) un canvi al repositori, pujant el resultat directament a GitHub Pages.
<br>

- Ejemplo de cambio:

```python
name: Deploy MkDocs
on:
  push:
    branches: [ main ]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Install dependencies
        run: pip install mkdocs-material
      - name: Deploy
        run: mkdocs gh-deploy --force
```