# Platzi - Curso Profesional de JavaScript
  
## Proyecto a desarrollar:  
Vamos a desarrollar un media player.  
Para encontrar documentación acerca de las funcionalidades que se le pueden dar a un media player, buscar **mdn htmlmediaelement**.  
  
------  
  
> Cómo llega un script al navegador?  
> El DOM es una representación de un documento HTML.  
> Cuando el navegador recibe la petición de un *index.html*, procesa todas las etiquetas y su contenido. Una vez cargado todo el documento HTML, se obtiene el evento **DOMContentLoaded**.  
  
------  
  
### Formas de cargar un script
Hay diferentes formas de cargar un script.  
Cuando se está cargando la página y el DOM encuentra una etiqueta script, se limita a cargar sólo el contenido de esa etiqueta dejando de cargar HTML en ese momento. Por eso es más que recomendable dejar las etiquetas script al final del documento, ya que si tenemos un querySelector de algo que aún no ha cargado, nos va a dar un error.  
  
### Carga asíncrona
Se puede cargar un script de forma asíncrona utiliando la palabra **async**.  
```
<head>
    <script async src="...></script>
</head>
```
Si tengo dos scripts asíncronos (uno grande y otro chico), se cargará primero el script más pequeño.  
  
### Cargar script al final
Utilizando la palabra **defer**, le decimos al DOM que cargue el script luego de cargar todo el HTML:  
```
<script defer src="..."></script>
```

