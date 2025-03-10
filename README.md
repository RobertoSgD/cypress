# cypress

Capturas
![image](https://github.com/user-attachments/assets/52c8a338-2220-499c-83ec-a5adb0c620ba)
![image](https://github.com/user-attachments/assets/48d0170e-1f6b-4fbe-affe-2fe2a0aa5efb)
![image](https://github.com/user-attachments/assets/c2a48546-a6f2-4195-b6e1-43b235a7f8e3)

Sin errores 
![image](https://github.com/user-attachments/assets/9508bd8a-cdbb-4794-a8de-5231fabd76d6)

# Proyecto con Cypress

Este proyecto utiliza Cypress para realizar pruebas automatizadas en una aplicación web. A continuación se explica cómo instalar y abrir Cypress en tu entorno de desarrollo.

## Requisitos previos

Asegúrate de tener **Node.js** instalado en tu sistema. Puedes verificar si lo tienes ejecutando el siguiente comando en tu terminal:

```bash
node -v

crea un proyecto con

- mkdir mi-proyecto
- cd mi-proyecto
- npm init -y

Ejecuta el siguiente comando en la terminal dentro de tu proyecto y abrelo:

bash
Copiar
Editar
npm install cypress --save-dev
npx cypress open

ya solo queda crear tus pruebas cypress
```
## Descripción de las Pruebas

### 1. **Formulario de Registro**

Las pruebas de este formulario verifican lo siguiente:

- **Campos obligatorios vacíos**: Asegura que los campos obligatorios muestren errores si se dejan vacíos.
- **Formato de correo electrónico**: Verifica que el correo electrónico tenga un formato válido y muestra un mensaje de error si es incorrecto.
- **Requisitos de la contraseña**: Asegura que la contraseña cumpla con los requisitos mínimos (longitud, mayúsculas, minúsculas, números) y muestra errores si no los cumple.
- **Contraseñas coincidentes**: Verifica que las contraseñas en los campos de "Contraseña" y "Confirmar contraseña" coincidan.
- **Términos y condiciones**: Asegura que los términos y condiciones sean aceptados antes de enviar el formulario.
- **Habilitación del botón de envío**: Verifica que el botón de envío esté habilitado solo cuando todos los campos sean válidos.
- **Envío del formulario y redirección**: Verifica que el formulario se envíe correctamente y redirija a la página de confirmación.

### 2. **Página de Confirmación**

Las pruebas de la página de confirmación verifican:

- **Mensaje de bienvenida**: Asegura que el nombre del usuario registrado se muestre en el mensaje de bienvenida.
- **Resumen de la información registrada**: Verifica que la información del usuario (nombre, correo y fecha de nacimiento) se muestre correctamente.
- **Botones de navegación**: Verifica que los botones de navegación hacia otras páginas estén presentes y funcionales.
- **Redirección sin datos en `localStorage`**: Si no hay datos de registro en `localStorage`, se redirige al usuario a la página de inicio.
