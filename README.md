# Biblioteca de Libros - Proyecto de React

**Descripción**  
Este proyecto es una aplicación de biblioteca interactiva desarrollada en React, diseñada para principiantes. La aplicación permite a los usuarios administrar una lista de libros, incluyendo funcionalidades para agregar, buscar, marcar como leídos y eliminar libros.

---

## Características Principales

1. **Agregar Libros**  
   - Permite a los usuarios añadir libros con detalles como título, autor y género.  
   - Validación básica para asegurarse de que no se dejen campos vacíos.

2. **Buscar Libros**  
   - Una barra de búsqueda en tiempo real que filtra libros por título o autor.  
   - Implementación eficiente utilizando `useState` y `useEffect`.

3. **Marcar como Leídos**  
   - Los usuarios pueden marcar libros como leídos o no leídos.  
   - El estado de lectura se muestra visualmente en la interfaz.

4. **Eliminar Libros**  
   - Función para eliminar libros de la biblioteca.  
   - Confirmación opcional antes de borrar un libro.

---

## Prohibición del Uso de Inteligencia Artificial

**Es estrictamente obligatorio que todo el código y las soluciones implementadas en este proyecto sean creadas únicamente por el desarrollador sin ayuda de herramientas de inteligencia artificial.**  
El propósito de esta regla es fomentar el aprendizaje y la comprensión profunda de los conceptos básicos de React y la programación. 

Cualquier violación de esta norma se considerará un incumplimiento de los objetivos del proyecto.

---

## Hooks Utilizados

- **`useState`**  
  Utilizado para administrar el estado local del formulario, la lista de libros y la barra de búsqueda.

- **`useEffect`**  
  Implementado para realizar acciones secundarias como filtrar libros o guardar los datos en el almacenamiento local del navegador.

- **`useContext`**  
  Proporciona un contexto global para compartir el estado de la biblioteca en toda la aplicación.

- **`useReducer`**  
  Administra operaciones complejas en la lista de libros, como añadir, eliminar o actualizar su estado.

---

## Arquitectura del Proyecto

```
src/
├── components/
│   ├── BookForm.js        # Componente para añadir nuevos libros
│   ├── BookList.js        # Lista interactiva de libros
│   ├── SearchBar.js       # Barra de búsqueda
├── context/
│   ├── BookContext.js     # Contexto global para la biblioteca
├── App.js                 # Componente principal
└── index.js               # Punto de entrada del proyecto
```

---

## Funcionalidades Técnicas

1. **Estado Global**  
   Utiliza `useContext` para compartir el estado de la biblioteca entre componentes sin necesidad de pasar props.

2. **Persistencia Local**  
   Los datos de los libros se almacenan en `localStorage`, permitiendo que los usuarios vean su biblioteca después de cerrar y reabrir la aplicación.

3. **Filtrado en Tiempo Real**  
   La barra de búsqueda utiliza `useEffect` para actualizar dinámicamente los resultados.

4. **Estilización**  
   Usa CSS modular o una biblioteca como TailwindCSS para estilizar componentes.

---

## Mejores Prácticas y Extensiones

- **Prácticas:**
  - Modulariza componentes para mantener un código limpio.
  - Implementa un diseño responsivo para adaptarse a diferentes dispositivos usando bootstrap.
