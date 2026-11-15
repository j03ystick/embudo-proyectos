# Embudo de Proyectos

Página web que muestra el estatus de los proyectos de la compañía en forma de embudo.

- `proyectos.xlsx`: **los proyectos** (pestaña Proyectos: Proyecto, Etapa, Coordinador, Área).
- `parametros.json`: la lista de etapas (en orden) y de coordinadores. **Se edita desde la página**, con el botón ⚙ Parámetros.
- `index.html`: la página; lee el Excel y los parámetros, y dibuja el embudo.
- `styles.css`: colores, tamaños y forma del embudo.
- `lib/xlsx.full.min.js`: librería (SheetJS) que permite a la página leer archivos de Excel.

## Actualizar proyectos
1. Abre `proyectos.xlsx` en Excel y haz tus cambios. Guarda.
2. En GitHub: **Add file → Upload files**, arrastra el Excel (con el mismo nombre) y haz clic en **Commit changes**.
3. En 1 o 2 minutos la página muestra los datos nuevos.

## Cambiar etapas o coordinadores
En la página, botón **⚙ Parámetros** → agrega, quita u ordena → **Guardar para todos**.
Para guardar se necesita una clave de GitHub (fine-grained token) con permiso *Contents: Read and write* solo sobre este repositorio.
Los colores se asignan solos según el lugar en la lista.
