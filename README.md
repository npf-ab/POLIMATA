# 📚 Enciclopedia del Conocimiento

Un rastreador de estudio autodidacta: 12 disciplinas (Matemáticas, Física, Química,
Biología, Computación, Psicología, Historia, Filosofía, Economía, Derecho, Geografía
y Lenguas), con cientos de temas y subtemas ya precargados como checklist editable.

Marca lo que dominas, edita o borra cualquier subtema, y añade los tuyos. Todo vive
en un único archivo `index.html`, sin backend ni dependencias que instalar.

## 🚀 Publicarlo en GitHub Pages (gratis, en ~2 minutos)

1. Crea un repositorio nuevo en GitHub (puede ser público o privado, aunque
   GitHub Pages gratuito solo publica repos públicos, o privados si tienes
   plan de pago/organización).
2. Sube estos archivos al repositorio. Desde tu computadora, dentro de esta carpeta:

   ```bash
   git init
   git add .
   git commit -m "Enciclopedia del conocimiento"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/TU-REPOSITORIO.git
   git push -u origin main
   ```

   (También puedes arrastrar los archivos directamente en la web de GitHub,
   sin usar la terminal, con el botón "Add file → Upload files".)

3. En GitHub, entra a **Settings → Pages** de tu repositorio.
4. En "Build and deployment", elige **Deploy from a branch**, rama `main`,
   carpeta `/ (root)`, y guarda.
5. Espera uno o dos minutos. GitHub te mostrará la URL pública, algo como:

   `https://TU-USUARIO.github.io/TU-REPOSITORIO/`

Esa es tu enciclopedia, accesible desde cualquier dispositivo con navegador.

## 💾 Sobre el guardado del progreso

Esta versión guarda tu progreso con `localStorage`, es decir: **queda guardado
en el navegador de ese dispositivo**, no en una cuenta ni en la nube. Ten en cuenta:

- Si entras desde el celular y luego desde la laptop, verás progresos distintos
  (cada navegador guarda el suyo).
- Si borras los datos de navegación / caché del sitio, se pierde el progreso.
- Es privado: nadie más que tú, en ese navegador, puede verlo u modificarlo.

Si más adelante quieres progreso sincronizado entre dispositivos, se puede
añadir un backend simple (por ejemplo, Firebase o Supabase) — avísame y lo
armamos.

## 🛠 Editar el contenido

Todo el contenido (disciplinas, temas y subtemas por defecto) vive dentro de
`index.html`, en la constante `DEFAULT_DATA` cerca del final del archivo.
Puedes editarlo directamente ahí si prefieres cambiar los valores "de fábrica"
en vez de hacerlo desde la interfaz.
