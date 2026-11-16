# Embudo de Proyectos

Página web que muestra el estatus de los proyectos de la compañía en forma de embudo.

- **Excel en SharePoint** (fuera de este repositorio): la lista de proyectos. Cuando cambia, Power Automate manda los datos aquí.
- `proyectos.json`: copia de los proyectos que llega sola desde SharePoint. **No editar a mano.**
- `.github/workflows/actualizar-proyectos.yml`: proceso que recibe los datos de Power Automate y actualiza `proyectos.json`.
- `parametros.json`: etapas (en orden) y coordinadores. Se edita desde la página con el botón ⚙ Parámetros.
- `proyectos.xlsx`: plantilla del Excel (con la tabla `TablaProyectos`). Se usa como respaldo si aún no existe `proyectos.json`.
- `index.html`, `styles.css`: la página y su diseño.
- `lib/xlsx.full.min.js`: librería (SheetJS) para leer archivos de Excel.

## Flujo de Power Automate
1. Disparador: SharePoint, *When a file is created or modified (properties only)* en la biblioteca del Excel.
2. Excel Online (Business), *List rows present in a table*: tabla `TablaProyectos`.
3. GitHub, *Create a repository dispatch event*: owner `j03ystick`, repo `embudo-proyectos`, event `actualizar-proyectos`, payload `{"filas": <value de List rows>}`.
