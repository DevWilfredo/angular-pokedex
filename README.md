# Angular PokeDex

Aplicación web desarrollada en Angular que consume la API pública de
Pokémon (PokeAPI) para mostrar un listado interactivo de Pokémon con
búsqueda, filtros y vista detallada.

## 🎯 Objetivo del Proyecto

Este proyecto tiene como objetivo:

-   Practicar arquitectura moderna en Angular.
-   Consumir APIs externas correctamente.
-   Manejar estados de carga y errores.
-   Implementar buenas prácticas de organización y control de versiones.
-   Aplicar seguimiento profesional mediante GitHub Projects (Kanban +
    Issues).

------------------------------------------------------------------------

## 🚀 Funcionalidades Planeadas (MVP)

-   Listado de Pokémon (paginado).
-   Skeleton loaders mientras carga la información.
-   Búsqueda por nombre.
-   Filtro por tipo.
-   Página de detalle por Pokémon.
-   Manejo de estados de error.
-   Diseño responsive.

------------------------------------------------------------------------

## 🏗️ Arquitectura del Proyecto

El proyecto utiliza una arquitectura organizada por responsabilidades:

```text
angular-pokedex/
├─ src/
│  ├─ app/                                 # Código principal de la aplicación
│  │  ├─ app.config.ts                     # Configuración (standalone)
│  │  ├─ app.routes.ts                     # Rutas principales
│  │  ├─ app.ts                            # Componente raíz (AppComponent)
│  │  ├─ shared/                           # Reutilizable en toda la app
│  │  │  └─ ui/                            # Componentes UI genéricos (skeletons, empty-states, etc.)
│  │  ├─ features/                         # Funcionalidades del producto
│  │  │  └─ pages/                         # Páginas (rutas) del PokeDex
│  │  │     ├─ pokemon-list/               # Home / listado
│  │  │     │  ├─ pokemon-list.ts
│  │  │     │  ├─ pokemon-list.html
│  │  │     │  ├─ pokemon-list.css
│  │  │     │  └─ pokemon-list.spec.ts
│  │  │     └─ pokemon-details/            # Detalle de un Pokémon
│  │  │        ├─ pokemon-details.ts
│  │  │        ├─ pokemon-details.html
│  │  │        ├─ pokemon-details.css
│  │  │        └─ pokemon-details.spec.ts
│  │  ├─ services/                         # Servicios (consumo de PokeAPI, lógica de datos)
│  │  ├─ models/                           # Interfaces/tipos del dominio (Pokemon, Type, Ability, etc.)
│  │  └─ adapters/                         # Adaptadores/mappers (API → modelos internos)
│  ├─ main.ts                              # Bootstrap del cliente
│  ├─ styles.css                           # Estilos globales
│  └─ index.html
├─ public/                                 # Estáticos
│  └─ favicon.ico
├─ angular.json
├─ package.json
├─ tsconfig.json
└─ README.md
```

------------------------------------------------------------------------

## 🧩 Convención de Commits

Se utiliza el estándar Conventional Commits.

Ejemplos:

-   feat: agregar listado de pokemones
-   fix: corregir error en respuesta de API
-   refactor: mejorar separación de responsabilidades
-   chore: configurar estructura inicial
-   docs: actualizar README

------------------------------------------------------------------------

## 🛠️ Tecnologías Utilizadas

-   Angular 21
-   TypeScript
-   CSS
-   PokeAPI
-   TailwindCss

------------------------------------------------------------------------

## 📦 Instalación y ejecución

1.  Clonar repositorio:

git clone `https://github.com/DevWilfredo/angular-pokedex`

2.  Instalar dependencias:

npm install

3.  Ejecutar en entorno local:

ng serve

4.  Abrir en navegador:

http://localhost:4200

------------------------------------------------------------------------

## 📌 Roadmap del Proyecto

-   v0.1 -- Configuración inicial
-   v0.2 -- Integración básica con API
-   v0.3 -- Listado funcional
-   v0.4 -- Página de detalle
-   v1.0 -- MVP completo y deploy

------------------------------------------------------------------------

## 🔮 Mejoras Futuras

-   Cacheo de resultados
-   Optimización de rendimiento
-   Mejoras de accesibilidad
-   Tests unitarios adicionales
-   Animaciones

------------------------------------------------------------------------

## 📄 Licencia

Proyecto educativo.
