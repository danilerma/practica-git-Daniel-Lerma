Practica de Git

Daniel Lerma Martinez
2630285
Creación y sincronización de repositorios con Git y GitHub.
Crear un repositorio local utilizando Git, sincronizarlo con un repositorio remoto en GitHub y comprobar el flujo de trabajo en ambos sentidos:

Repositorio local → GitHub
GitHub → Repositorio local.


# Práctica de Git y GitHub: Mi Experiencia y Flujo de Trabajo

## 1. Descripción del procedimiento realizado
Durante esta práctica puse en marcha un flujo completo de control de versiones utilizando Git de manera local en mi computadora y GitHub en la nube. Comencé creando una carpeta de trabajo, inicializando Git en ella y redactando mis primeros archivos (`README.md` y `datos.txt`). Después de registrar mis cambios de forma local, vinculé el repositorio con un proyecto vacío en GitHub. Para terminar, comprobé que la sincronización funcionara en ambos sentidos: primero enviando cambios de mi computadora hacia GitHub, y luego modificando un archivo directamente en la web de GitHub para descargarlo y sincronizarlo en mi equipo.

---

## 2. Comandos de Git utilizados y explicación de su función
Para llevar a cabo esta práctica, utilicé los siguientes comandos y estas son sus funciones:

*   **`git init`**: Lo usé para convertir mi carpeta de trabajo en un repositorio de Git, activando el sistema para que comience a rastrear los cambios.
*   **`git branch -M main`**: Me sirvió para asegurarme de que la rama principal de mi proyecto se llamara `main`, que es el estándar actual.
*   **`git status`**: Lo consulté en varias ocasiones para revisar el estado actual de mis archivos (saber si había cambios sin guardar o si todo estaba limpio).
*   **`git add .`**: Lo utilicé para preparar todos mis archivos nuevos o modificados, pasándolos al área de preparación (*staging area*) antes de guardarlos.
*   **`git commit -m "mensaje"`**: Es el comando con el que creé un punto de control definitivo en el historial de mi proyecto, acompañándolo de un mensaje corto que describe lo que hice.
*   **`git remote add origin <URL>`**: Me permitió conectar mi repositorio local con el repositorio que creé en internet, asignándole la dirección oficial (`origin`).
*   **`git remote -v`**: Lo ejecuté para verificar rápidamente que la dirección web del repositorio remoto estuviera bien vinculada.
*   **`git push -u origin main`**: Lo utilicé para subir mis archivos locales a GitHub por primera vez. El parámetro `-u` dejó conectadas ambas ramas de manera permanente para el futuro.
*   **`git pull origin main`**: Lo usé para descargar e integrar automáticamente en mi computadora los cambios que realicé previamente desde la página web de GitHub.
*   **`git push`**: Es el comando abreviado que empleé después para enviar mis nuevas modificaciones locales directamente a GitHub sin tener que escribir toda la ruta otra vez.

---

## 3. ¿Cómo creé el repositorio local?
Para empezar, creé una carpeta en mi computadora con el nombre solicitado (`practica-git-nombre-apellido`). Luego, abrí la terminal de PowerShell dentro de esa misma carpeta. Al escribir el comando `git init`, la carpeta dejó de ser un directorio común y corriente y Git comenzó a controlarla. Después, renombré la rama principal a `main` y creé manualmente los archivos de la práctica: este archivo `README.md` y un archivo llamado `datos.txt`, al cual le puse un texto inicial para poder trabajar con él.

---

## 4. ¿Cómo vinculé el repositorio local con GitHub?
Para conectar mi computadora con internet, entré a la plataforma de GitHub, inicié sesión y creé un nuevo repositorio público con el mismo nombre, asegurándome de dejarlo completamente vacío (sin marcar casillas de README o licencias). GitHub me generó una URL única del proyecto. Copié esa dirección, regresé a PowerShell en mi PC y escribí `git remote add origin` junto con el enlace para indicarle a mi computadora dónde debía enviar la información. Comprobé que todo estuviera bien con `git remote -v` y finalmente subí mi contenido local usando `git push -u origin main`.

---

## 5. ¿Cómo realicé la sincronización Local → GitHub?
Este paso consistió en enviar mis avances desde la computadora hacia la nube. Lo hice de la siguiente manera:
1. Abrí el archivo `datos.txt` en mi PC y agregué una nueva línea de texto.
2. Usé `git status` para comprobar que Git detectó la modificación.
3. Preparé el archivo ejecutando `git add .`.
4. Guardé el cambio con un commit escribiendo `git commit -m "Actualización desde repositorio local"`.
5. Envié los cambios a internet con el comando `git push`.
Al entrar a GitHub y actualizar la página, pude comprobar que el texto que escribí en mi computadora apareció reflejado de inmediato en la web.

---

## 6. ¿Cómo realicé la sincronización GitHub → Local?
Este paso simuló el proceso de recibir actualizaciones hechas por otros (o por mí mismo) desde la nube hacia mi equipo. Lo hice así:
1. Entré a la página web de GitHub, abrí el archivo `datos.txt` y lo edité directamente usando el botón de editar (lápiz), agregando una nueva línea.
2. Guardé los cambios haciendo clic en el botón de commit de la web.
3. Abrí mi terminal de PowerShell en la computadora.
4. Ejecuté el comando `git pull origin main`.
Con esto, Git descargó la modificación que hice en internet y la integró de manera automática en mi archivo local `datos.txt` sin perder nada de lo que ya tenía.

---

## 7. Descripción de los archivos contenidos en el repositorio
*   **`README.md`**: Es este documento en formato Markdown. Funciona como la documentación y explicación detallada de todo el procedimiento que realicé en la práctica, redactado con mis propias palabras.
*   **`datos.txt`**: Un archivo de texto plano que utilicé como base para practicar la creación de commits, la edición de contenido y la comprobación de la sincronización en ambos sentidos (de mi PC a GitHub y de GitHub a mi PC).

---

## 8. Conclusión personal sobre lo aprendido
Realizar esta práctica me ayudó a entender que Git y GitHub son herramientas indispensables para cualquier proyecto de desarrollo. Aprendí que no sirven solo como una copia de seguridad en la nube, sino como un sistema muy preciso para llevar el historial exacto de cada cambio. Dominar el flujo de trabajo en ambas direcciones me dio una visión mucho más clara de cómo organizar mi trabajo de forma ordenada, segura y profesional.