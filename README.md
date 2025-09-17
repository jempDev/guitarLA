# GuitarLA

GuitarLA es una tienda virtual de guitarras desarrollada con **React**. Permite
a los usuarios explorar una colección de guitarras, agregarlas a un carrito de
compras, modificar cantidades y simular una experiencia de compra sencilla. El
estado del carrito se mantiene persistente usando **localStorage**.

## Características

- **Catálogo de guitarras:** Visualiza una lista de guitarras con imagen,
  nombre, descripción y precio.
- **Carrito de compras:**
  - Agrega guitarras al carrito.
  - Aumenta o disminuye la cantidad de cada guitarra (máximo 5, mínimo 1).
  - Elimina guitarras del carrito.
  - Vacía el carrito completamente.
- **Persistencia:** El carrito se guarda automáticamente en el navegador usando
  localStorage.
- **Cálculo automático:** El total a pagar se actualiza dinámicamente según el
  contenido del carrito.
- **Interfaz responsiva:** Utiliza Bootstrap para un diseño adaptable a
  diferentes dispositivos.

## Características de React Utilizadas

- **Componentes funcionales:** Toda la aplicación está construida usando
  componentes funcionales para una estructura moderna y reutilizable.
- **Hooks de React:**
  - `useState`: Para manejar el estado del carrito y los datos de la tienda.
  - `useEffect`: Para sincronizar el carrito con localStorage y ejecutar efectos
    secundarios.
  - `useMemo`: Para optimizar cálculos derivados como el total del carrito y
    verificar si está vacío.
- **Props:** Comunicación entre componentes para pasar datos y funciones.
- **Renderizado condicional:** Para mostrar diferentes vistas según el estado
  del carrito.
- **Mapeo de listas:** Para renderizar dinámicamente la colección de guitarras y
  los productos en el carrito.

## Estructura del Proyecto

```
src/
│
├── components/
│   ├── Guitar.jsx      # Componente para mostrar cada guitarra y agregarla al carrito
│   └── Header.jsx      # Encabezado con logo y carrito de compras
│
├── data/
│   └── db.js           # Base de datos local de guitarras
│
├── App.jsx             # Componente principal, maneja el estado global y lógica del carrito
└── index.js            # Punto de entrada de la aplicación
```

## Tecnologías Utilizadas

- **React** (con hooks: useState, useEffect, useMemo)
- **JavaScript**
- **Bootstrap** (para estilos y diseño responsivo)
- **localStorage** (para persistencia del carrito)

## Instalación y Uso

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/jempDev/guitarLA.git
   cd guitarLA
   ```

2. **Instala las dependencias:**

   ```bash
   npm install

   ```

3. **Inicia la aplicación:**

   ```bash
   npm run dev
   ```

4. Abre [http://localhost:5173](http://localhost:5173) en tu navegador.

## Personalización

- Puedes modificar el archivo `src/data/db.js` para agregar, quitar o editar
  guitarras.
- Las imágenes de las guitarras deben estar en la carpeta `public/img/` y
  coincidir con el nombre definido en la propiedad `image` de cada guitarra.

## Créditos

Desarrollado como parte de un curso de React + TypeScript en Udemy.

---

¡Explora, agrega guitarras a tu carrito y disfruta de la experiencia GuitarLA!
