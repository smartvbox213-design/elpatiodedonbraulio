# El patio de Don Braulio · Formosa

Escena 3D de un patio de campo formoseño con tres personajes digitales de estética de cómic nacional, creados con IA:

- **Don Braulio** (El Colorado): sabelotodo de la provincia y cebador oficial de tereré.
- **Paco** (loro hablador): experto en flora del monte, chismoso y quejoso.
- **Cacho** (mono carayá): experto en fauna, travieso y glotón.

## Cómo se usa

- Arrastrá para girar la cámara y usá la rueda (o pellizcá) para acercar.
- Tocá un personaje, o usá los botones de abajo, para enfocarlo y ver su presentación.
- **Hablar con Don Braulio / Paco / Cacho:** conversación por voz en vivo con su agente de ElevenLabs. El navegador pide permiso para usar el micrófono.
- **Que dialoguen:** tres episodios guionados en los que los personajes se hablan entre sí, con subtítulos y cámara que sigue a quien habla.

## Tecnología

Una sola página (`index.html`) con [three.js r128](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) cargado desde cdnjs. Las ilustraciones van incrustadas, así que no hacen falta otros archivos ni un paso de compilación.

## Publicar con GitHub Pages

1. En el repositorio: **Settings → Pages**.
2. En *Build and deployment*, elegí **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. Esperá un minuto y abrí `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Cómo funciona la voz

- **Conversación en vivo:** usa el SDK `@elevenlabs/client` (cargado desde jsDelivr, versión fija) y los IDs públicos de los agentes, que están en `index.html`. No hay claves de API en el código. Los agentes aceptan conversaciones solo desde `smartvbox213-design.github.io` y `localhost` (se configura en ElevenLabs, en *Security → Allowlist*).
- **Diálogo entre personajes:** usa las voces en español del propio navegador (Web Speech API). Suenan distinto según el dispositivo y no son las voces de ElevenLabs. Si el navegador no tiene voces en español, el episodio se muestra solo con subtítulos.
