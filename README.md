# Sistema escolar

Sistema de gestión escolar para varios colegios: inscripciones, asistencia, tareas, exámenes, notas, pagos y usuarios.

## Archivos

- `index.html`: la aplicación completa.
- `firebase-config.js`: datos de conexión al proyecto de Firebase y UID del superadministrador.
- `firestore.rules`: reglas de seguridad (copia de lo que está publicado en Firestore → Reglas).

## Probar en tu computadora

La página necesita abrirse con un servidor local; con doble clic sobre el archivo no funciona.

- **Opción A (VS Code):** instala la extensión *Live Server*, abre la carpeta y presiona *Go Live*.
- **Opción B (Node.js):** en la carpeta del proyecto ejecuta `npx serve` y abre la dirección que aparece.

## Primer uso

1. Entra con tu cuenta de superadministrador.
2. Crea un colegio de demostración con su primera cuenta de administración.
3. Cierra sesión y entra con esa cuenta para configurar grados, cursos, maestros y alumnos.

## Publicar

Sube la carpeta a un repositorio privado de GitHub y conéctalo a Netlify (sin comando de compilación; carpeta de publicación: la raíz del repositorio).

## Respaldos

- **Superadministrador:** en la pantalla Colegios, botón *Respaldar* (un colegio) o *Respaldar todos* (un solo archivo). La columna *Respaldo* avisa si pasaron más de 7 días.
- **Administración de cada colegio:** Configuración → *Descargar respaldo*.
- **Restaurar:** solo el superadministrador, con *Restaurar respaldo*. Vuelve a crear lo borrado y reemplaza lo existente con la versión del respaldo; no borra lo creado después. Las cuentas de inicio de sesión (Authentication) no forman parte del respaldo.
- Guarda los archivos en al menos dos lugares (por ejemplo, tu computadora y Google Drive).
