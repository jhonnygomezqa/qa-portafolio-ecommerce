# Login: análisis de requisitos

**Aplicación:** https://www.saucedemo.com
**Fecha de análisis:** 16/11/2026
**Método:** exploración manual de la aplicación

## Requisitos funcionales

| ID | Requisito |
|----|-----------|
| RF-LOG-01 | El usuario puede iniciar sesión con usuario y contraseña válidos. |
| RF-LOG-02 | El sistema no permite iniciar sesión con el usuario vacío. |
| RF-LOG-03 | El sistema no permite iniciar sesión con la contraseña vacía. |
| RF-LOG-04 | El sistema rechaza credenciales incorrectas con un mensaje de error. |
| RF-LOG-05 | El sistema impide el acceso a usuarios bloqueados. |

## Criterios de aceptación

**RF-LOG-01**
- Dado que estoy en la página de login
- Cuando introduzco un usuario y contraseña válidos y pulso Login
- Entonces accedo al catálogo de productos

**RF-LOG-02 y RF-LOG-03**
- Dado que estoy en la página de login
- Cuando dejo un campo vacío y pulso Login
- Entonces el sistema muestra un mensaje indicando que el campo es obligatorio y no permite el acceso

**RF-LOG-04**
- Dado que estoy en la página de login
- Cuando introduzco credenciales que no coinciden con ningún usuario
- Entonces el sistema muestra un mensaje de error y no permite el acceso

**RF-LOG-05**
- Dado que estoy en la página de login
- Cuando intento entrar con el usuario bloqueado (locked_out_user) y su contraseña
- Entonces el sistema no permite el acceso y muestra el mensaje: "Sorry, this user has been locked out."

## Notas del entorno
- La aplicación debe probarse en **inglés**. Con la traducción automática del navegador, los nombres de usuario aparecen traducidos y el login falla. Esto es un problema de entorno de prueba, no un defecto de la aplicación.
