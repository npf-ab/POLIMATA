# 📚 Enciclopedia del Conocimiento

Un rastreador de estudio autodidacta: 12 disciplinas (Matemáticas, Física, Química,
Biología, Computación, Psicología, Historia, Filosofía, Economía, Derecho, Geografía
y Lenguas), con cientos de temas y subtemas ya precargados como checklist editable,
más una biblioteca con lector de ePub integrado.

## ✨ Qué incluye

- **Checklist editable** por disciplina: marca, edita, borra o añade temas y subtemas.
- **Lecturas recomendadas** por disciplina (libros de referencia, marcables como leídos).
- **Biblioteca personal**: sube tus propios archivos `.epub` (uno general y uno por disciplina).
- **Lector integrado** que:
  - recuerda en qué página te quedaste de cada libro,
  - muestra las imágenes del libro con normalidad,
  - puede **leer en voz alta** (texto a voz) con botón de play/pausa y control de velocidad,
    resaltando la oración que se está leyendo,
  - te deja **seleccionar texto** y guardarlo como 🔖 Marcador (con fecha), 📘 Definición
    o ✏️ Ejercicio, etiquetado opcionalmente con el tema del temario al que pertenece.
- **Conceptualario, Marcadores y Ejercicios** por disciplina, con salto directo de
  vuelta al lugar del libro donde los guardaste.

## 🚀 Publicarlo en GitHub Pages (gratis, en ~2 minutos)

1. Crea un repositorio nuevo en GitHub (público, o privado si tienes plan de pago).
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

Guarda esa URL como favorito (o agrégala a la pantalla de inicio del celular) —
es tu enciclopedia, accesible desde cualquier dispositivo con navegador.

## 💾 Sobre el guardado de datos

Todo se guarda **en el navegador de cada dispositivo**, no en una cuenta ni en la nube:

- El progreso del checklist, tus ediciones, y tus marcadores/definiciones/ejercicios
  se guardan con `localStorage`.
- Los archivos `.epub` que subas se guardan con `IndexedDB` (soporta archivos más
  grandes que `localStorage`).
- Si entras desde el celular y la laptop, cada uno guarda su propio progreso y su
  propia biblioteca — no se sincronizan entre sí.
- Si borras los datos de navegación / caché del sitio para ese dominio, se pierde
  todo lo guardado ahí.
- Es privado: nadie más que tú, en ese navegador, puede verlo o modificarlo.

Si más adelante quieres progreso y biblioteca sincronizados entre dispositivos,
se puede añadir un backend simple (por ejemplo, Firebase o Supabase) — avísame y
lo armamos.

## 🔊 Sobre la lectura en voz alta

Usa la Web Speech API del navegador (funciona en Chrome, Edge y la mayoría de
navegadores modernos; puede no estar disponible en algunos navegadores muy
antiguos o restringidos). La voz utilizada depende de las voces en español
instaladas en tu sistema operativo/navegador, no es algo que la página controle.

## 🛠 Editar el contenido

Todo el contenido por defecto (disciplinas, temas, subtemas y libros recomendados)
vive dentro de `index.html`, en las constantes `DEFAULT_DATA` y `RECOMMENDED_BOOKS`
cerca del inicio del script. Puedes editarlo directamente ahí si prefieres cambiar
los valores "de fábrica" en vez de hacerlo desde la interfaz.
