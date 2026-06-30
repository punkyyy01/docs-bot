# Política de Privacidad (Privacy Policy)

Última actualización: Junio de 2026

Esta Política de Privacidad describe cómo Purgatory Bot ("el bot") recopila, utiliza y protege la información de los usuarios y servidores de Discord donde está instalado.

## 1. Datos que recopilamos
Para funcionar correctamente, el bot recopila y almacena la siguiente información:
* **IDs de Discord:** Almacenamos IDs de usuarios, IDs de canales e IDs de servidores[cite: 1].
* **Contenido de los mensajes:** El bot almacena el contenido de los mensajes de texto en texto plano en una base de datos local SQLite[cite: 1].
* **Multimedia:** Almacenamos URLs de GIFs y de imágenes enviadas por los usuarios (incluyendo aquellas subidas a la CDN de Discord)[cite: 1]. 
* **Nombres de usuario:** Se guarda el nombre de visualización (display name) de los usuarios junto a sus mensajes[cite: 1].

El bot **no** almacena contraseñas, correos electrónicos ni otros datos personales identificables fuera del contexto de Discord[cite: 1].

## 2. Uso de la información
Los datos recopilados se utilizan estrictamente para las funcionalidades principales del bot:
* **Cadenas de Markov y Generación de Texto:** El contenido de los mensajes se utiliza para entrenar un modelo local de cadenas de Markov que permite al bot generar respuestas automáticas e imitar el estilo de escritura de los usuarios (comandos `/generar` e `/imitar`)[cite: 1].
* **Generación de Memes:** Las imágenes guardadas en el pool del servidor se procesan para generar memes automáticos o mediante el comando `/momo`[cite: 1].
* **Galería de GIFs:** Las URLs de GIFs recopiladas se utilizan para alimentar una galería web pública[cite: 1].

## 3. Servicios de Terceros
El bot interactúa con servicios externos para ciertas funciones, lo que implica el procesamiento temporal de datos fuera de nuestra infraestructura:
* **Cloudflare R2:** Utilizamos este servicio para almacenar de forma persistente los GIFs e imágenes que de otro modo expirarían en la CDN de Discord[cite: 1].
* **Groq API:** Las imágenes y una muestra de los mensajes del servidor se envían a los modelos de inteligencia artificial de Groq (específicamente `llama-4-scout-17b-16e-instruct`) para generar el texto de los memes[cite: 1].
* **Servicios de Música:** Las URLs de música se procesan mediante `yt-dlp` interactuando con plataformas como YouTube y SoundCloud[cite: 1].

## 4. Control y Retención de Datos
* Los administradores del servidor pueden purgar completamente el historial de mensajes recopilados por el bot utilizando el comando `/corpus_wipe`[cite: 1].
* Los administradores pueden evitar que el bot lea y almacene mensajes de canales específicos usando el comando `/corpus_ignorar add`[cite: 1].

## 5. Contacto
Si tienes preguntas sobre esta política o deseas solicitar la eliminación manual de tus datos, por favor contacta al administrador del bot a través de Discord.