## 1.Uso de complementos (plugins)
<br>

### Para mayor comodidad y estilo en la presentación de La Taula del Barri, agregué los complementos básicos de MkDocs:
- mkdocs-material (diseño adaptativo y temas).
- mkdocs-material (diseño adaptativo y temas).

## 2.Configuración y despliegue
<br>

### ¿Qué es mkdocs.yml?
#### Es el archivo principal de configuración del sitio web (nombre, tema, navegación).
<br>

- Ejemplo de cambio:

```python
site_name: La Taula del Barri
theme:
  name: material
```
<br>

### ¿Qué es deploy.yml?
#### Es el archivo de GitHub Actions para la compilación y publicación automática del sitio en GitHub Pages tras cada commit.
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