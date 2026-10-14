# El patio de Don Braulio · Formosa

Escena 3D de un patio de campo formoseño con tres personajes digitales de estética de cómic nacional, creados con IA: **Don Braulio**, **Paco** (loro) y **Cacho** (mono carayá).

## Cómo se usa

La pantalla tiene solo dos botones:

- **Hablar con…**: conversación por voz en vivo con el personaje elegido (por defecto, Don Braulio). Para elegir otro, tocalo en la escena. El navegador pide permiso para usar el micrófono. Para cortar, tocá **Colgar**.
- **Que hablen entre ellos**: los personajes dialogan con un episodio guionado. Cada vez que lo tocás pasa al episodio siguiente (son tres). **Cortar** lo detiene.

Arrastrá para girar la cámara y usá la rueda (o pellizcá) para acercar. Tocar un lugar vacío vuelve a la vista general.

## Cómo funciona

- **Boca sincronizada:** en la conversación en vivo sigue el volumen real de la voz del agente. En el diálogo entre personajes se calcula por sílabas y se re-sincroniza con cada palabra cuando el navegador lo permite.
- **Conversación en vivo:** usa el SDK `@elevenlabs/client` (desde jsDelivr, versión fija) y los IDs públicos de los agentes, que están en `index.html`. No hay claves de API en el código. Los agentes aceptan conversaciones solo desde `smartvbox213-design.github.io` y `localhost` (se configura en ElevenLabs, en *Security → Allowlist*).
- **Diálogo entre personajes:** usa las voces en español del propio navegador (Web Speech API), que suenan distinto según el dispositivo. Sin voces en español, los personajes mueven la boca pero no se escucha nada.
- **Tecnología:** una sola página con [three.js r128](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) desde cdnjs. Las ilustraciones van incrustadas.

## Publicar con GitHub Pages

En el repositorio: **Settings → Pages → Deploy from a branch**, rama `main`, carpeta `/ (root)`.
