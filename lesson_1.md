# Clase №1

## Creación de componentes (sin estilización)

### Tarea №1

Separa [la plantilla](<https://www.figma.com/file/mfsNEI7Nv5i5fkdseWbFn7/Lesson-(Copy)?node-id=8701%3A11194>) en componentes

**Por ejemplo**

```jsx
<Sidebar>
<Menu>
<MenuItem>
<Main>
<Paper>
<Card>
<TutorsList>
<Tutor>
<CitiesList>
<City>
<DepartmentsList>
<Department>
```

### Tarea №2

Crear un archivo menu.js con un array para dibujar el menú

```jsx
export const menuConfig = [
  {
    name: "Universidad",
  },

  {
    name: "Facultades",
  },
];
```

Dibujar el menú de la barra lateral usando `menuConfig` y mostrar su funcionamiento con `props` y `key`.

![Menú](/images/sidebar.png)

### Tarea №3

Crear un componente ` <Paper>` - componente con fondo blanco y sangría que utiliza `props.children` y renderiza cualquier diseño que se le pase

![Paper](/images/paper.png)

### Tarea №4

Dibujar el componente de la tarjeta y la descripción utilizando ` <Paper>` y mostrar cómo importar las imágenes en el componente

Tarjeta

![Card](/images/Card.png)

Descripción

![description](/images/description.png)

### Tarea №5

Dibuja colecciones de profesores, ciudades, facultades utilizando este json

```json
{
  "name": "MIT",
  "description": "Experiencia, una concentración de conocimientos y la capacidad de evitar la mayoría de errores de contratación. Sabemos lo que quieren la mayoría de las empresas locales y extranjeras, y podemos dárselo. Ademas, estamos constantemente mejorando nuestros cursos de programación, agregando algo nuevo allí. Podrá ver personalmente los casos de éxito de nuestros alumnos egresados para comprobar la eficacia de nuestra metodología de enseñanza. Sí, comenzaremos con lo básico y la información fundamental. Sabemos que la mayoría de las personas acuden a nosotros sin ningún conocimiento previo.",
  "tutors": [
    {
      "firstName": "Diego",
      "lastName": "Martínez",
      "patronymic": "",
      "phone": "+ 52 55 4166 2620",
      "email": "diegomartinez@goit.global",
      "city": "Ciudad de México",
      "options": "Creación de grupos"
    },
    {
      "firstName": "Carlos",
      "lastName": "Valverde",
      "patronymic": "",
      "phone": "+52 55 4166 2136",
      "email": "cvalverde@gmail.com",
      "city": "Acapulco",
      "options": "Creación de grupos,
      creación de países, edición de perfiles de profesores"
    }
  ],
  "cities": ["Buenavista", "Acapulco", "Ciudad de México"],
  "department": [
    { "name": "Facultad de Informática" },
    { "name": "Facultad de Redes Neuronales" },
    { "name": "Facultad de Automatización" }
  ]
}
```

![collection](/images/collection.png)

### Tarea №6

Crear un componente de botón universal que tenga 3 props `text`, `icon` y `onClick` (en el futuro)

![button](/images/button.png)

### Tarea №7

Hacer una descripción de los props dentro de todos los componentes utilizando `propTypes`.
