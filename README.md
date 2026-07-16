# Proyecto Vite + React (ejemplo)

Pequeña plantilla creada con Vite y React. Contiene una app de ejemplo con HMR y configuración para desplegar en GitHub Pages (observa la opción `base` en `vite.config.js`).

**Requisitos**
- Node.js 16+ y npm

**Instalación**
```bash
npm install
```

**Desarrollo**
- Inicia el servidor de desarrollo con:

```bash
npm run dev
```

Accede a la app en `http://localhost:5173` (puerto por defecto de Vite).

**Compilación y vista previa**
- Generar build para producción:

```bash
npm run build
```

- Probar la build localmente:

```bash
npm run preview
```

**Scripts**
- `dev`: inicia Vite en modo desarrollo
- `build`: construye la aplicación para producción
- `preview`: sirve la build para pruebas locales
- `lint`: ejecuta `oxlint` (herramienta de lint)

**Estructura relevante**
- [index.html](index.html)
- [vite.config.js](vite.config.js)  (nota: `base` está configurado en `/test_github_actions_2_h_3/`)
- [package.json](package.json)
- [src/](src/) (código fuente: `main.jsx`, `App.jsx`, estilos y assets)

**Despliegue en GitHub Pages**
La configuración `base` en `vite.config.js` está pensada para publicar en GitHub Pages en el repositorio `/<nombre-repo>/`. Para desplegar:

1. Ejecuta `npm run build`.
2. Publica la carpeta `dist/` en la rama `gh-pages` (por ejemplo usando `gh-pages` o una GitHub Action).

Si quieres, puedo añadir un workflow de GitHub Actions para automatizar el despliegue.

**Más información**
- Documentación de Vite: https://vite.dev/
- Documentación de React: https://react.dev/

