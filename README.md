Hola BUENAS!
Aca les comparto el nuevo link para importar en Postman: 
https://www.getpostman.com/collections/0a5b265b5e47d58dd1be
Tambien subo el nuevo archivo para descargar en el repositorio "templates.jsreport" y actualizo README.md 


# Importar Prueba.Jsreport

- Instala jsreport con configuracion de puerto 5488
- Ejecute JsReport con: jsreport start
- Descargamos el archivo "Prueba.jsreport" del repositorio https://github.com/KevinArvn/requerimiento_gisworking
- Abrimos en el navegador: (http://localhost:5488/)
- Importamos el archivo "Prueba.jsreport" en JsReport
- Se creará una carpeta llamada "Peliculas":
  --template "excel-main" con configuración para crear archivos .xlsx
  --template "saldra-main" con configuración para crear archivos PDF
- Tambien otra carperta llamada "Series"
  --template "okeynuevo-xlsx" con configuración para crear archivos .xlsx
  --template "okeynuevo-xlsx" con configuración para crear archivos PDF
- Y por ultimo otra carpeta llamada "Horarios Report"
  --template "horarios-pdf" con configuración para crear archivos PDF
  
  (Todos con sus respectivos .css)

# Endpoints Postman "Templates"

 # Carpeta "Creación de Templates"

 - POST Crear Template PDF: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templates.jsreport")
 - POST Crear Template Excel: Este Endpoint crea un template con configuración html-to-xlsx (ya está creado si importamos antes "templates.jsreport")
 - POST Creación Template PDF Nuevo: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templates.jsreport")
 - POST Creación Template Excel Nuevo: Este Endpoint crea un template con configuración html-to-xlsx (ya está creado si importamos antes "templates.jsreport")
  - POST Crear Template Horarios-PDF: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "templates.jsreport")
  
  # Carpeta "Exportación"

POST Exportar Datos Excel: Exporta datos al template "excel-main"
POST Exportar Datos PDF: Exporta datos al template "saldra-main"
POST Exportación de Datos Excel Nuevo: Exporta datos al template "okeynuevo-xlsx"
POST Exportación de Datos PDF Nuevo: Exporta datos al template "okeynuevo-pdf"
POST Exportar Datos Excel: Exporta datos al template "horarios-pdf"

- Carpeta "Muestra de Contenido"

- GET Mostrar contenido de Report-Excel: Muestra el contenido pedido en excel-main con la petición antes hecha 
    - (Si guardamos el archivo en "Save Reponse" con "Save to a file" se crea un archivo response.xlsx con los datos)  
- GET Mostrar contenido de Report-PDF: Muestra el contenido pedido en saldra-main con la peticion antes hecha
    - (Si guardamos el archivo en "Save Reponse" con "Save to a file" se crea un archivo response.pdf con los datos)  
- GET Mostrar todos los Reports: Muestra todos los reportes hechos y guardados en Reports*

- Se podrá acceder a "Reports" en localhost:5488, apretando sobre el botón de herramienta ubicado en la parte superior derecha y accediendo a Reports
