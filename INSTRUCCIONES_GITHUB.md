Guía de Sincronización y Actualización con Git

Al empezar a trabajar o al intentar ejecutar git pull o git push, es probable que aparezca un aviso de conflicto si otro colaborador ha subido cambios recientemente a la rama principal.
Instrucciones para Sincronizar el Repositorio

    Abre una terminal en Visual Studio Code. Para ello, dirígete al menú superior izquierdo, haz clic en Terminal y selecciona Nueva Terminal (o New Terminal).

    Ejecuta el siguiente comando:

git pull origin main --rebase

Nota: El comando utiliza la opción --rebase para aplicar los cambios del repositorio remoto (origin main) sobre tu copia local de forma ordenada. Esto te permite integrar el trabajo previo del equipo antes de publicar tus propios cambios.
Normas de Trabajo en Equipo

    Sincronización previa: Ejecuta siempre git pull origin main --rebase antes de enviar tus cambios para asegurar que tu entorno de trabajo contenga la versión más reciente del código.

    Protección contra sobrescritura: Si tu copia local no está actualizada, Git bloqueará la ejecución de git push. Este mecanismo de seguridad evita sobrescribir de forma accidental el código publicado por otros miembros del equipo.