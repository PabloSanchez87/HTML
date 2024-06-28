# FORMULARIOS
## ¿Qué es un formulario?
- Bloque con un conjunto de elementos de entrada de información.
- Es de las únicas formas en las que podemos enviar datos a un servidor.
- Se conoce como **formulario** a los mecanismos para enviar información por parte del usuario, a tracés de unos campos visuales de forma sencialla e intuitiva, que determinan la naturaleza del tipo de información que se va a enviar u como hacerla llegar a otro enxtremo donde se procesará esa información

### ¿Formulario más sencillo que se te pueda ocurrir?
<br>
<div style="text-align: center;">
  <img src="formulario.png"/>
</div>


## Objetivos
- Hacer lo más sencillo posible el proceso de inserción de datos por parte del usuario.
- Intentar que la experiencia de usuario sea lo más agradable y cómoda posible.
- Intetar que los datos introducidos estén en un formato predecible y esperado.
- Reducir los errores al introducir datos en la medida de lo posible
- Comunicar de forma clara y rápidamente si ocurren errores al introducir datos.

### Etiqueta `<form>`
- Etiqueta de bloque con atributos propios.
- Englobará todo el contenido del formulario.
- Pueden coexistir carios formularios en la misma página.

- Atributos propios:
<br>
<div style="text-align: center;">
  <img src="atributos_propios.png"/>
</div>
<br>

- Información que puedes enviar en un formulario:
    - Texto
    - Email
    - Cantidades
    - Numéricos
    - Fechas
    - etc...
<br>
<div style="text-align: center;">
  <img src="informacion.png"/>
</div>
<br>

- Sintaxis de un formulario.
```html
<form action="/ruta-del-servidor" method="post">
    <!-- Campo de texto -->
    <label for="nombre">Nombre:</label><br>
    <input type="text" id="nombre" name="nombre"><br><br>

    <!-- Campo de correo electrónico -->
    <label for="email">Correo Electrónico:</label><br>
    <input type="email" id="email" name="email"><br><br>

    <!-- Campo de contraseña -->
    <label for="password">Contraseña:</label><br>
    <input type="password" id="password" name="password"><br><br>

    <!-- Campo de fecha -->
    <label for="fecha">Fecha de Nacimiento:</label><br>
    <input type="date" id="fecha" name="fecha"><br><br>

    <!-- Campo de selección -->
    <label for="genero">Género:</label><br>
    <select id="genero" name="genero">
        <option value="masculino">Masculino</option>
        <option value="femenino">Femenino</option>
        <option value="otro">Otro</option>
    </select><br><br>

    <!-- Casillas de verificación -->
    <label>Intereses:</label><br>
    <input type="checkbox" id="deportes" name="intereses" value="deportes">
    <label for="deportes">Deportes</label><br>
    <input type="checkbox" id="musica" name="intereses" value="musica">
    <label for="musica">Música</label><br>
    <input type="checkbox" id="tecnologia" name="intereses" value="tecnologia">
    <label for="tecnologia">Tecnología</label><br><br>

    <!-- Botón de envío -->
    <input type="submit" value="Enviar">
</form>
```

## Métodos de envío.

### Método GET
- Concatenación de variables en URL.
- Como máximo el envío de unos 500 bytes de información.
- No permite el envío de archivos adjuntos con el formulario.
- Los datos enviados se ven en la barra de direcciones del navegador.
- El símbolo **?** indica dónde empiezan los parámetros que se reciben desde el formulario que ha enviado los dtos a la página.
- Después del símbolo **?** aparecen parejas de datos con su nombre y valor separados por el símbolo **&** 
- Las parejas dato1=valor1, dato2=valor2... reflejan el bombre y el valor de los campos enviados por el formulario.
- Tener en cuenta que para separar la primera pareja de la dirección web en sí se usa el símbolo **?** y para separar las restantes parejas **&**
- Determinados caracteres no son recibidos en la URL de la forma exacta en que fueron escritos en el formulario.
- Se utilizan para formularios de consulta.
- No se usan para modificar ni crear registros.
- Ejemplo:
    ```url 
        www.facebook.com/registro?firstname=Pablo&lastname=Sanchez
    ```
    ```url 
        http://www.example.com:80/path/to/myfile.html?key1=value1&key2=value2#SomewhereInTheDocument
    ```
<div style="text-align: center;">
  <img src="http.png"/>
</div>

<div style="text-align: center;">
  <img src="domain.png"/>
</div>

<div style="text-align: center;">
  <img src="port.png"/>
</div>

<div style="text-align: center;">
  <img src="path.png"/>
</div>

<div style="text-align: center;">
  <img src="parameters.png"/>
</div>
<br>

### Método POST
- Se envían de forma "oculta"
- Se pueden enviar una gran cantidad de datos a la vez.
- Permite enviar documentos adjuntos.
- Se usarán para acciones de creación, edición y borrado.
---
### CRUD
    Create -> método POST
    Read   -> método GET
    Update -> método POST
    Delete -> método POST

---
### Etiqueta `<input>`
- Elemento princpal donde poremos escribir la información que queremos enviar al servidor.
- Dependiendo de la naturaleza de los datos utilizaremos input de un tipo u otro.

    [Ver documentación etiqueta input "W3C"](https://www.w3schools.com/tags/tag_input.asp)

---

- Código ejemplo:
```html
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input ty
```
- [Ver código formulario Google](formulario_google.html)
- [Ver código formulario](formulario_sencillo.html)

