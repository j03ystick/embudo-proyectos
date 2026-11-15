# Embudo de Proyectos

Página web que muestra el estatus de los proyectos de la compañía en forma de embudo.

- `proyectos.xlsx`: **los datos**. Es el único archivo que hay que cambiar para actualizar la información.
  - Pestaña **Proyectos**: un renglón por proyecto (Proyecto, Etapa, Coordinador, Área).
  - Pestaña **PARAMETROS**: la lista de etapas (en orden, con color opcional) y la lista de coordinadores.
- `index.html`: la página; lee el Excel y dibuja el embudo.
- `styles.css`: colores, tamaños y forma del embudo.
- `lib/xlsx.full.min.js`: librería (SheetJS) que permite a la página leer archivos de Excel.

## Cómo actualizar los datos
1. Abre `proyectos.xlsx` en Excel y haz tus cambios. Guarda.
2. En GitHub: **Add file → Upload files**, arrastra el Excel (con el mismo nombre) y haz clic en **Commit changes**.
3. En 1 o 2 minutos la página muestra los datos nuevos.
