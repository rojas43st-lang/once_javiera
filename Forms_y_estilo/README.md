# Explicación de los cambios realizados en el formulario

1. **Cambio de identidad visual (Reto 1)**
   - En el CSS, modifiqué la variable `--primario` que estaba con azul `#2563eb` y la cambié por un naranja brillante `#f97316`.
   - La variable `--primario-oscuro` también se ajustó para mantener el contraste al hacer hover sobre botones (`#c2410c`).
   - Cambié el radio de los bordes (`--radio`) de 8px a 20px para que todos los campos y botones tengan esquinas más redondeadas.
   - Esto afecta inputs, selects, textareas y botones, dando un estilo más moderno y llamativo.

2. **Nuevo campo “Edad” (Reto 2)**
   - Se agregó un nuevo bloque `.campo` dentro del formulario con un `<label>` y un `<input type="number">`.
   - Se configuró para que solo acepte edades entre 15 y 99 años usando los atributos `min="15"` y `max="99"`.
   - Se agregó `required` para que el usuario deba completarlo.
   - Este campo se colocó **entre Asunto y Mensaje**, manteniendo la estructura lógica del formulario.

3. **Botón primario con sombra exagerada (Reto 3)**
   - Modifiqué `.btn-primario` para que tenga una sombra mucho más intensa:
     ```css
     box-shadow: 0 8px 30px rgba(0,0,0,0.7);
     ```
   - Al hacer hover, la sombra se incrementa aún más:
     ```css
     box-shadow: 0 12px 50px rgba(0,0,0,0.8);
     ```
   - Esto crea un efecto visual de profundidad y resalta el botón sobre el fondo.


# Explicación de los cambios realizados en el CSS

1. **Cambio de colores principales**
   - Se modificó la variable `--primario` a un verde lima `#b6c627`.
   - Se ajustó `--primario-oscuro` a un verde más brillante `#d1de26`.
   - Esto hace que todos los elementos que usan color primario (botones, acentos de radio y checkbox, bordes al enfocar inputs) adopten esta nueva identidad visual.

2. **Bordes más redondeados**
   - La variable `--radio` se aumentó de 8px a 20px.
   - Todos los inputs, selects, textareas y botones ahora tienen esquinas más redondeadas, creando un estilo más moderno y “suave”.

3. **Sombra de botón principal más intensa**
   - `.btn-primario` ahora tiene:
     ```css
     box-shadow: 0 8px 30px rgba(0,0,0,0.6);
     ```
   - Al hacer hover, la sombra se amplifica:
     ```css
     box-shadow: 0 12px 50px rgba(0,0,0,0.7);
     ```
   - Esto da profundidad y hace que el botón destaque sobre el fondo.

4. **Foco en inputs**
   - El borde y sombra al enfocar inputs, selects y textareas se ajustó para usar la nueva variable primaria:
     ```css
     box-shadow: 0 0 0 3px rgba(249, 115, 22, 0.25);
     ```
   - Esto mantiene la coherencia con la paleta de colores actual.

5. **Radios y checkboxes**
   - Los `input[type="radio"]` y `input[type="checkbox"]` ahora usan `accent-color: var(--primario)`, aplicando el verde lima como color de acento.

6. **Otros ajustes menores**
   - Se mantuvo el diseño responsive para `.fila-doble` y `.formulario-contacto`.
   - Se conservaron estilos de labels, ayudas, links y botones secundarios (`.btn-secundario`) sin cambios de color.
   - El resto del CSS permanece igual, manteniendo la consistencia del diseño base.

