
# Sorteo de Amigos

Este proyecto es una aplicación simple que permite a los usuarios agregar nombres de amigos a una lista y luego realizar un sorteo para seleccionar un amigo al azar. El objetivo principal de este desafío es fortalecer las habilidades en lógica de programación y manipulación del DOM utilizando JavaScript.

## Características

- **Agregar Amigos**: Los usuarios pueden ingresar nombres de amigos en un campo de texto y agregarlos a una lista.
- **Renderizar Lista**: La lista de amigos se actualiza automáticamente cada vez que se agrega un nuevo amigo.
- **Sortear Amigo**: Se puede realizar un sorteo para seleccionar un amigo al azar de la lista.
- **Validación de Entrada**: Se valida que el campo de texto no esté vacío antes de agregar un amigo.

## Cómo Usar

1. **Agregar Amigos**:
   - Ingresa el nombre de un amigo en el campo de texto.
   - Haz clic en el botón "Agregar" para agregar el nombre a la lista.

2. **Sortear Amigo**:
   - Una vez que hayas agregado varios amigos a la lista, haz clic en el botón "Sortear" para seleccionar un amigo al azar.
   - El nombre del amigo sorteado se mostrará en la pantalla.

3. **Reiniciar**:
   - Después de realizar un sorteo, la lista de amigos se limpiará automáticamente, permitiéndote comenzar de nuevo.

## Estructura del Código

- **`agregarAmigo()`**: Esta función toma el valor del campo de texto, valida que no esté vacío y luego agrega el nombre a la lista de amigos. Finalmente, limpia el campo de texto y vuelve a renderizar la lista.
  
- **`renderizarAmigos()`**: Esta función se encarga de mostrar la lista de amigos en el DOM. Recorre la lista de amigos y crea un elemento `<li>` para cada uno, agregándolo a la lista en el HTML.

- **`sortearAmigo()`**: Esta función selecciona un amigo al azar de la lista y muestra el resultado en el DOM. Luego, limpia la lista de amigos para permitir un nuevo sorteo.

# Contacto
Si tienes alguna pregunta o sugerencia, no dudes en contactarme a través de mi correo electrónico.

## Ejemplo de Uso

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sorteo de Amigos</title>
</head>
<body>
    <h1>Sorteo de Amigos</h1>
    <input type="text" id="amigo" placeholder="Ingresa el nombre de un amigo">
    <button onclick="agregarAmigo()">Agregar</button>
    <button onclick="sortearAmigo()">Sortear</button>
    <ul id="listaAmigos"></ul>
    <p id="resultado"></p>

    <script>
        // Código JavaScript aquí
    </script>
</body>
</html>
