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
Se pide crear un formulario de registro que contenga los siguientes campos:

- Nombre completo (obligatorio)
- Correo electrónico (obligatorio, con validación de formato)
- Contraseña (obligatorio, mínimo 8 caracteres, debe incluir al menos una letra mayúscula, una minúscula y un número)
- Confirmación de contraseña (debe coincidir con la contraseña)
- Fecha de nacimiento (opcional)
- Términos y condiciones (checkbox obligatorio)
- Botón de envío
 El formulario debe incluir las siguientes validaciones con Cypress:

- Todos los campos marcados como obligatorios no pueden estar vacíos
- El correo electrónico debe tener un formato válido (usar regex adecuada)
- La contraseña debe cumplir con los requisitos mínimos de seguridad
- Las contraseñas ingresadas deben coincidir
- El checkbox de términos y condiciones debe estar marcado para poder enviar el formulario
- Mostrar mensajes de error específicos para cada validación fallida
- El botón de envío debe deshabilitarse si hay errores de validación
- Después de un registro exitoso, el usuario debe ser redirigido a una página de confirmación que:

Muestre un mensaje de bienvenida personalizado con el nombre del usuario
Incluya un resumen de la información registrada (sin mostrar la contraseña)
Tenga un botón para regresar al inicio o continuar al área de usuario
