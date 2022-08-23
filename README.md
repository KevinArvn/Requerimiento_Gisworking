# Importar Prueba.Jsreport

- Instala jsreport con configuracion de puerto 5488
- Ejecute JsReport con: jsreport start
- Descargamos el archivo "Prueba.jsreport" del repositorio https://github.com/KevinArvn/requerimiento_gisworking
- Abrimos en el navegador: (http://localhost:5488/)
- Importamos el archivo "Prueba.jsreport" en JsReport
- Se creará un archivo llamado "Prueba":
  template "excel-main" con configuración para crear archivos .xlsx
  template "saldra-main" con configuración para crear archivos PDF

# Endpoints Postman "Prueba"

1. POST Crear Template PDF: Este Endpoint crea un template con configuración chrome-pdf (ya está creado si importamos antes "Prueba.jsreport")
2. POST Crear Template Excel: Este Endpoint crea un template con configuración html-to-xlsx (ya está creado si importamos antes "Prueba.jsreport")
3. POST Exportar Datos Excel: Exporta datos al template "excel-main"
4. POST Exportar Datos PDF: Exporta datos al template "saldra-main"
5. GET Mostrar contenido de Report-Excel: Muestra el contenido pedido en excel-main con la petición antes hecha 
    - (Si guardamos el archivo en "Save Reponse" con "Save to a file" se crea un archivo response.xlsx con los datos)  
6. GET Mostrar contenido de Report-PDF: Muestra el contenido pedido en saldra-main con la peticion antes hecha
    - (Si guardamos el archivo en "Save Reponse" con "Save to a file" se crea un archivo response.pdf con los datos)  
7. GET Mostrar todos los Reports: Muestra todos los reportes hechos y guardados en Reports*

- Se podrá acceder a "Reports" en localhost:5488, apretando sobre el botón de herramienta ubicado en la parte superior derecha y accediendo a Reports
