# El patio de Don Braulio · Formosa

Escena 3D de un patio de campo formoseño con tres personajes digitales de estética de cómic nacional, creados con IA:

- **Don Braulio** (El Colorado): sabelotodo de la provincia y cebador oficial de tereré.
- **Paco** (loro hablador): experto en flora del monte, chismoso y quejoso.
- **Cacho** (mono carayá): experto en fauna, travieso y glotón.

## Cómo se usa

- Arrastrá para girar la cámara y usá la rueda (o pellizcá) para acercar.
- Tocá un personaje, o usá los botones de abajo, para enfocarlo y ver su presentación.

## Tecnología

Una sola página (`index.html`) con [three.js r128](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) cargado desde cdnjs. Las ilustraciones van incrustadas, así que no hacen falta otros archivos ni un paso de compilación.

## Publicar con GitHub Pages

1. En el repositorio: **Settings → Pages**.
2. En *Build and deployment*, elegí **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. Esperá un minuto y abrí `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Nota

Los personajes tienen agentes de voz en ElevenLabs, pero esta página no los conecta. Para conversar por voz hay que sumar el SDK de ElevenLabs con los IDs de tus agentes, sin poner nunca tu clave de API en el código.
