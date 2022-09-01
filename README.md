Hola!
Aca les comparto el nuevo link para importar en Postman: 
https://www.getpostman.com/collections/9bdd35ff02b8d3b9f72c
Tambien subo el nuevo archivo para descargar en el repositorio "templatesnew.jsreport" y actualizo README.md 


# Importar templatesnew.jsreport

- Instala jsreport con configuracion de puerto 5488
- Ejecute JsReport con: jsreport start
- Descargamos el archivo "templatesnew.jsreport" del repositorio https://github.com/KevinArvn/requerimiento_gisworking
- Abrimos en el navegador: (http://localhost:5488/)
- Importamos el archivo "Prueba.jsreport" en JsReport
- Se creara una carpeta llamada "Graficos"
  -- template "graph-pdf" con configuracion para crear un archicvo PDF 
- Siguiendo de esta se creará una carpeta llamada "Peliculas":
  --template "excel-main" con configuración para crear archivos .xlsx
  --template "saldra-main" con configuración para crear archivos PDF
- Tambien otra carperta llamada "Series"
  --template "okeynuevo-xlsx" con configuración para crear archivos .xlsx
  --template "okeynuevo-xlsx" con configuración para crear archivos PDF
-  Tambien otra carpeta llamada "Horarios Report"
  --template "horarios-pdf" con configuración para crear archivos PDF
  --template "horarios-xlsx" con configuración para crear archivos xlsx
-Por ultimo se creara una carpeta llamada "Sueldos"
  --template "sueld-pdf" con configuración para crear archivos PDF
  --template "sueld-xlsx" con configuración para crear archivos xlsx
  
  (Todos con sus respectivos .css)

# Endpoints Postman "Templates"

 # Carpeta "Creación de Templates"

 - POST Crear Template PDF: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templatesnew.jsreport")
 - POST Crear Template Excel: Este Endpoint crea un template con configuración html-to-xlsx (ya está creado si importamos antes "templatesnew.jsreport")
 - POST Creación Template PDF Nuevo: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templatesnew.jsreport")
 - POST Creación Template Excel Nuevo: Este Endpoint crea un template con configuración html-to-xlsx (ya está creado si importamos antes "templatesnew.jsreport")
  - POST Crear Template Horarios-PDF: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templatesnew.jsreport")
  - POST Crear Template Horarios-Excel: Este Endpoint crea un template con configuración html-to-xlsx (ya está creado si importamos antes "templatesnew.jsreport")
  - POST Crear Template Sueldos-Excel: Este Endpoint crea un template con configuración html-to-xlsx (ya está creado si importamos antes "templatesnew.jsreport")
  - POST Crear Template Sueldos-PDF: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templatesnew.jsreport")
 - POST Crear Template Grafico: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templatesnew.jsreport")
 
  
  # Carpeta "Exportación"

POST Exportar Datos Excel: Exporta datos al template "excel-main"
POST Exportar Datos PDF: Exporta datos al template "saldra-main"
POST Exportación de Datos PDF Nuevo: Exporta datos al template "okeynuevo-pdf"
POST Exportación de Datos Excel Nuevo: Exporta datos al template "okeynuevo-xlsx"
POST Exportar Datos Horas PDF: Exporta datos al template "horarios-pdf"
POST Exportar Datos Horas Excel: Exporta datos al template "horarios-xlsx"
POST Exportar Datos Sueldos Excel: Exporta datos al template "sueld-xlsx"
POST Exportar Datos Sueldos PDF: Exporta datos al template "sueld-pdf"


- Carpeta "Muestra de Contenido"

- GET Mostrar contenido de Report-Excel: Muestra el contenido pedido en excel-main con la petición antes hecha 
    - (Si guardamos el archivo en "Save Reponse" con "Save to a file" se crea un archivo response.xlsx con los datos)  
- GET Mostrar contenido de Report-PDF: Muestra el contenido pedido en saldra-main con la peticion antes hecha
    - (Si guardamos el archivo en "Save Reponse" con "Save to a file" se crea un archivo response.pdf con los datos)  
- GET Mostrar todos los Reports: Muestra todos los reportes hechos y guardados en Reports*

- Se podrá acceder a "Reports" en localhost:5488, apretando sobre el botón de herramienta ubicado en la parte superior derecha y accediendo a Reports

Eso es todo.
 
