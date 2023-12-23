# Examenes

## Teoria
8/12, felicidades, eres el unico que acertó la pregunta de que tipos de datos primitivos existen! Los fallos han sido en detalles muy concretos donde casi todos habeis caido, muy bien en general.

## Práctica
7/10, está muy bien! Usar un framework es definitivamente una buena opción para estilizar rápido, pero te has olvidado un poco de la usabilidad de la página. Al añadir participantes, la interfaz va desplazandose hacia abajo, por lo que el usuario tendrá que hacer scroll conforme añada mas y mas personas a la lista, creo que intentaste arreglarlo sobreescribiendo encima de picocss, en este caso es fácil, solo debes añadir este estilo:

```css
.left{
    position: absolute;
    top: 2em;
    left: 2em;
    }
body{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    }
```

Para que esto además funcione, debemos cerrar bien esta estructura:

```html
  <div class ="left">
    <h1>Participantes</h1> 
  <div class="ganador"></div>
</div> <!-- el contenedor left estaba cerrado al final del body, encerrando tanto la lista de participantes como la de la interfaz de los inputs --> 

```
![Correccion](fix0.png)

Échale un ojo a tu código y lo entenderás, si tienes dudas este jueves te lo aclaro sin problema.

## Documentación

Falta la documentación entera. Además tampoco editaste bien el archivo README.md con tus datos, debes tener cuidado con estos detalles antes de enviar.

Nota: 7