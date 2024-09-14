Este script tiene como objeto analizar y resumir un texto que se le pase como entrada
El script hace el siguiente trabajo:
- Toma el texto de entrada
- Analiza el texto según el patrón (pattern) que se le haya  indicado
- Devuelve el Análisis realizado
----------------------------
Archivos necesarios:
- todos los del repo https://github.com/danielmiessler/fabric
----------------------------
Requerimientos:
- Interprete de lenguaje Go
- Opcional:
--+ Application Yt
    para descargar transcripcion del texto de un video de Youtube
    go install github.com/danielmiessler/yt@latest
--+ Libreria Trans
    para la traducción a otro idioma de un texto de entrada
----------------------------
Ejemplos de ejecución:
- Desde línea de comandos:
--+ yt --transcript {{url}} | fabric --stream --pattern extract_wisdom | trans -b :es

---------------------------