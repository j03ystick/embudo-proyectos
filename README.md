# Embudo de Proyectos

Página web que muestra el estatus de los proyectos de la compañía en forma de embudo.

- `proyectos.xlsx`: **los proyectos** (pestaña Proyectos: Proyecto, Etapa, Coordinador, Área).
- `parametros.json`: etapas (en orden) y coordinadores. Se edita desde la página con el botón ⚙ Parámetros.
- `index.html`, `styles.css`: la página y su diseño.
- `lib/xlsx.full.min.js`: librería (SheetJS) para leer archivos de Excel.

## Zoom por fase
Al hacer clic en una fase del embudo se muestra solo ese anillo, en grande y arriba al centro, con la cantidad de proyectos de esa etapa y su % del total. Debajo quedan solo sus proyectos. Clic en el anillo, en **← Ver embudo completo** o la tecla Esc para regresar.

## Enlace con el dashboard
La página lee los proyectos del [dashboard de seguimiento](https://github.com/j03ystick/dashboard-proyectos) (`../Dashboard-proyectos/` en el mismo sitio de GitHub Pages). Si un proyecto del Excel tiene detalle allá, en la lista aparece como enlace **Ver detalle →**.
- Se enlaza por nombre (igual al del dashboard, sin importar mayúsculas ni acentos).
- Opcional: agrega una columna **ID** al Excel con el ID del dashboard (por ejemplo `PRY-2026-001`) para enlazarlo aunque el nombre sea distinto.

## Actualizar proyectos
1. Abre `proyectos.xlsx` en Excel y haz tus cambios. Guarda.
2. En GitHub: **Add file → Upload files**, arrastra el Excel (con el mismo nombre) y haz clic en **Commit changes**.
3. En 1 o 2 minutos la página muestra los datos nuevos.

## Pendiente
Conectar el Excel con Google Sheets o SharePoint para que se actualice solo (por decidir).
La versión con SharePoint + Power Automate quedó en el historial (commit be6ad74).
