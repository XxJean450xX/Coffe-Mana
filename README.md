# Proyecto Cafetería - React + Vite

Este proyecto es una aplicación web desarrollada con **React + Vite** para la gestión y visualización de un sistema de cafetería.  
Su arquitectura está basada en **módulos escalables (features)** para facilitar el mantenimiento, la organización y la expansión del código a medida que el proyecto crece.

---

## Arquitectura del Proyecto

La estructura del proyecto sigue un modelo modular inspirado en las mejores prácticas de React:
~~~
src/
│
├── assets/ → Imágenes, íconos, fuentes y otros recursos estáticos.
├── components/ → Componentes globales reutilizables (Navbar, Button, Footer...).
├── context/ → Contextos globales (Autenticación, Carrito, Tema, etc.).
├── features/ → Módulos o requerimientos específicos del sistema.
│ ├── menu/
│ │ ├── components/
│ │ ├── hooks/
│ │ ├── services/
│ │ └── MenuPage.jsx
│ └── orders/
│ ├── components/
│ ├── hooks/
│ ├── services/
│ └── OrdersPage.jsx
├── hooks/ → Custom hooks reutilizables en todo el proyecto.
├── pages/ → Páginas principales de la aplicación (Home, Menu, Contact, Admin...).
├── routes/ → Configuración de rutas usando React Router.
├── services/ → Conexiones a APIs, Firebase o lógica de datos externos.
└── utils/ → Funciones auxiliares (helpers, validaciones, formateadores...).
~~~

**Idea clave:**  
Los componentes que se usan en muchas partes del sistema van en `src/components`.  
Los componentes específicos de una funcionalidad van dentro de `src/features/<feature>/components`.

---

## Tecnologías principales

- [React](https://react.dev/) – Biblioteca para la creación de interfaces de usuario.
- [Vite](https://vitejs.dev/) – Bundler moderno y rápido para proyectos React.
- [React Router](https://reactrouter.com/) – Navegación entre páginas.
- [Context API](https://react.dev/reference/react/useContext) – Manejo de estados globales.
- [Tailwind CSS](https://tailwindcss.com/) o CSS Modules – Sistema de estilos (opcional según preferencia).

---

## Cómo ejecutar el proyecto

~~~
# 1. Clonar el repositorio
git clone https://github.com/tuusuario/cafeteria.git

# 2. Entrar en el proyecto
cd cafeteria

# 3. Instalar dependencias
npm install

# 4. Ejecutar el entorno de desarrollo
npm run dev
~~~

## Próximos pasos

- Definir requerimientos funcionales y de usuario.

- Crear las primeras features: menú, pedidos y usuarios.

- Configurar conexión con API o base de datos (Firebase o Express).

- Implementar diseño responsivo y estilos globales.

- Documentar componentes y hooks importantes.