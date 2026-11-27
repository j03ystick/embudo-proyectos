# Embudo de Proyectos

Página web que muestra el estatus de los proyectos de la compañía en forma de embudo.

- `proyectos.xlsx`: **los proyectos** (pestaña Proyectos: id, Folio, Nombre de Proyecto, Cliente, Estatus, Responsable, Notas/Comentarios, Fecha de Inicio, Fecha de Fin, Semaforo). "Estatus" se usa como la etapa del embudo y "Responsable" como el coordinador. El archivo del repositorio trae datos de ejemplo. Las columnas Estatus y Responsable tienen listas desplegables (pestaña "Listas").
- Estatus válidos: No Iniciado, Iniciado, Por Confirmar, Concluido, Cerrado. Responsables: Angeles Sanchez, Fernanda Hernandez, Gabriela Cabezas, Joseph Huesca, POR ASIGNAR (un proyecto sin responsable cuenta como POR ASIGNAR). No importan mayúsculas ni acentos.
- `parametros.json`: etapas (en orden) y coordinadores. Se edita desde la página con el botón ⚙ Parámetros.
- `index.html`, `styles.css`: la página y su diseño.
- `lib/xlsx.full.min.js`: librería (SheetJS) para leer archivos de Excel.

## Actualizar proyectos (desde la página)
1. Abre la página y haz clic en **⚙ Parámetros**.
2. **⬇ Exportar Excel** descarga los proyectos actuales. Ábrelo en Excel, haz tus cambios y guarda.
3. **⬆ Importar Excel**, elige tu archivo: el embudo se actualiza solo en tu pantalla.
4. Presiona **Guardar para todos** (pide la clave de GitHub). En 1 o 2 minutos todos ven los datos nuevos.

También se puede subir `proyectos.xlsx` a mano en GitHub (**Add file → Upload files**, con el mismo nombre).

## Pendiente
Conectar el Excel con Google Sheets o SharePoint para que se actualice solo (por decidir).
La versión con SharePoint + Power Automate quedó en el historial (commit be6ad74).
