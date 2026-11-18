# Nexus Coallition

Página estática e independiente para `coallition.nexuscollective.app`.

## Contenido

- `index.html`: página completa, con CSS y JavaScript integrados.
- `favicon.svg`: icono vectorial del sitio.

No necesita Workers, servidor propio, base de datos, dependencias, compilación ni proceso de build.

## Publicación

Sube el contenido de esta carpeta a la raíz del repositorio que desplegará `coallition.nexuscollective.app`. En el proveedor de páginas estáticas, configura el directorio raíz como salida del sitio. El archivo de entrada es `index.html`.

## Solicitudes

El formulario es deliberadamente estático: valida los datos y copia el texto de la solicitud al portapapeles, pero no transmite ni almacena datos. Para recibir solicitudes automáticamente habría que conectar un canal público de contacto o un backend/formulario externo.

En el bloque JavaScript del final de `index.html` existen dos constantes para futuras vías públicas de contacto:

```js
const PUBLIC_CONTACT_EMAIL = "";
const PUBLIC_DISCORD_URL = "";
```

Se han dejado vacías. Al rellenarlas con un correo dedicado al proyecto o una invitación pública de Discord, la página mostrará automáticamente esos botones en el pie. No uses un correo personal ni una cuenta privada.
