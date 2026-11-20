# Pedagogías Digitales (rediseño)

Sitio informativo construido con Astro. El contenido (textos e imágenes) se edita desde un panel visual en `/admin`.

## Editar el contenido (para el cliente)

1. Entrar a `https://<su-sitio>.netlify.app/admin/`.
2. Iniciar sesión con la cuenta invitada.
3. Elegir **Contenido del sitio → Textos e imágenes**.
4. Editar los textos o subir imágenes y presionar **Publicar**. El sitio se actualiza en un par de minutos.

## Configuración inicial (para el desarrollador)

1. Subir este proyecto a un repositorio nuevo de GitHub (rama `main`).
2. Crear el sitio en Netlify conectado a ese repositorio. Netlify lee `netlify.toml` para compilar.
3. En Netlify, activar **Identity** y **Git Gateway** (sección Site configuration → Identity). Invitar al cliente por correo. Verifica los pasos actuales en la documentación de Netlify, porque la interfaz cambia con el tiempo.
4. Confirmar que `/admin/` carga y que el cliente puede publicar un cambio de prueba.

## Desarrollo local

```bash
npm install
npm run dev
```

El contenido está en `src/data/contenido.json`. La apariencia está en `src/styles/global.css` y la estructura en `src/pages/index.astro`.
