SIERRA ADALE — PROYECTO WEB Y APLICACIÓN WINDOWS
Creador: Johann Sebastian Moreno

CONTENIDO
- index.html: estructura y textos.
- styles.css: diseño adaptable negro mate, verde fosforescente y azul.
- script.js: menú interactivo, año y navegación.
- electron-main.js / package.json: opción para empaquetar la web como aplicación Windows.

PROBAR LA PÁGINA
1. Extrae el ZIP en una carpeta.
2. Abre la carpeta en Visual Studio Code.
3. Haz doble clic en index.html para abrirla en tu navegador, o instala la extensión Live Server y pulsa "Go Live".

CREAR UN INSTALADOR .EXE EN WINDOWS 10/11
Necesitas tener Node.js LTS instalado desde https://nodejs.org/ y conexión a internet.
1. Abre esta carpeta en Visual Studio Code.
2. Abre Terminal > Nueva terminal.
3. Ejecuta: npm.cmd install
4. Ejecuta: npm.cmd start
   Se abrirá SIERRA ADALE como una aplicación de escritorio.
5. Para construir el instalador, ejecuta: npm.cmd run build:win
6. Busca el instalador dentro de la carpeta release.

IMPORTANTE
- El ZIP contiene el código fuente; no es por sí mismo un instalador .exe.
- Si npm no se reconoce o PowerShell bloquea scripts, usa los comandos con npm.cmd tal como aparecen arriba.
- El paquete no incluye icono personalizado. Para evitar errores, si el proceso informa que falta assets/icon.ico, elimina temporalmente la línea "icon": "assets/icon.ico" de package.json y vuelve a ejecutar el comando.
- La página no conecta todavía con un servicio real de IA. Es una presentación web interactiva para usar como base del proyecto.
- Revisa y prueba la aplicación antes de distribuirla a otras personas.


DESCARGA DEL INSTALADOR
-----------------------
Se añadió el instalador proporcionado por el usuario en:
downloads/JARVIS-HRZ-3.1.3.exe
El botón “Descargar para Windows” apunta a ese archivo relativo. Si publicas la web en un hosting, también debes publicar la carpeta downloads.

IMPORTANTE SOBRE EL HOSTING
---------------------------
El instalador pesa aproximadamente 149 MB. Algunos servicios de hosting estático, incluido Netlify, pueden rechazar archivos individuales de ese tamaño. En ese caso, sube el .exe a Google Drive u otro servicio de archivos, configura el enlace para que cualquier persona con el enlace pueda descargarlo y cambia en index.html el href del botón por ese enlace público. No ejecutes el instalador si no confías en su origen; analiza el archivo con Microsoft Defender primero.
