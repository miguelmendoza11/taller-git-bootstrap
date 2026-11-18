# Taller Git + Bootstrap — Web de presentación del equipo

Pequeña web estática para presentar a los integrantes del equipo, construida con
HTML y [Bootstrap 5](https://getbootstrap.com/) (cargado por CDN, sin instalar nada).

## Integrantes

| Integrante | GitHub |
|------------|--------|
| Miguel Angel Mendoza | [@miguelmendoza11](https://github.com/miguelmendoza11) |
| Juan | [@JuanMR2006](https://github.com/JuanMR2006) |
| Juan | [@JuanSCC8](https://github.com/JuanSCC8) |

## Estructura

```
proyecto/
├── index.html          # Página principal del equipo
├── profiles/           # Una página por integrante
└── assets/
    └── images/         # Fotos y avatares
```

## Cómo verlo

Abrir `index.html` en el navegador. No necesita servidor ni instalación.

## Flujo de trabajo con Git

- `main`: versión estable. Solo recibe merges desde `develop`.
- `develop`: rama de integración del equipo.
- `feature/<nombre>`: cada funcionalidad nueva. Sale de `develop` y vuelve por Pull Request.
- `fix/<nombre>`: corrección de errores. Sale de `develop` y vuelve por Pull Request.

Nadie hace commit directo en `main` ni en `develop`, y nadie aprueba su propio Pull Request.

### Convención de commits

`tipo: descripción` — tipos: `feat`, `fix`, `style`, `refactor`, `docs`.
