# Embudo de Proyectos

Página web que muestra el estatus de los proyectos de la compañía en forma de embudo.

- `proyectos.xlsx`: **los proyectos** (pestaña Proyectos: Proyecto, Etapa, Coordinador, Área).
- `parametros.json`: etapas (en orden) y coordinadores. Se edita desde la página con el botón ⚙ Parámetros.
- `index.html`, `styles.css`: la página y su diseño.
- `lib/xlsx.full.min.js`: librería (SheetJS) para leer archivos de Excel.

## Actualizar proyectos
1. Abre `proyectos.xlsx` en Excel y haz tus cambios. Guarda.
2. En GitHub: **Add file → Upload files**, arrastra el Excel (con el mismo nombre) y haz clic en **Commit changes**.
3. En 1 o 2 minutos la página muestra los datos nuevos.

## Pendiente
Conectar el Excel con Google Sheets o SharePoint para que se actualice solo (por decidir).
La versión con SharePoint + Power Automate quedó en el historial (commit be6ad74).
