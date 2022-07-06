#Instalación

Para instalar el paquete, hay que modificar el archivo `composer.json` de la raíz del proyecto para reemplazar la clase `\PhpOffice\PhpWord\Writer\Word2007\Part\Chart` por la incluida en el paquete:

```json
"autoload": {  
    "exclude-from-classmap": ["vendor/phpoffice/phpword/src/PhpWord/Writer/Word2007/Part/Chart.php"],  
    "classmap": [  
      {"\\PhpOffice\\PhpWord\\Writer\\Word2007\\Part\\Chart":  "PhpWordReports/Chart.php"}  
    ]  
},
``` 
