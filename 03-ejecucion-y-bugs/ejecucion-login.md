# Ejecución de pruebas: Login

- **Aplicación:** https://www.saucedemo.com (en inglés)
- **Fecha de ejecución:** 23/11/2026
- **Tester:** Jhonny Gómez Campero
- **Navegador:** Chrome, con la traducción automática desactivada

## Resultados

| ID | Título | Resultado obtenido | Estado |
|----|--------|--------------------|--------|
| TC-LOG-01 | Login con credenciales válidas | Se accede al catálogo de productos. | Pasa |
| TC-LOG-02 | Login con usuario vacío | "Epic sadface: Username is required". No se accede. | Pasa |
| TC-LOG-03 | Login con contraseña vacía | "Epic sadface: Password is required". No se accede. | Pasa |
| TC-LOG-04 | Login con contraseña incorrecta | "Epic sadface: Username and password do not match any user in this service". No se accede. | Pasa |
| TC-LOG-05 | Login con usuario inexistente | "Epic sadface: Username and password do not match any user in this service". No se accede. | Pasa |
| TC-LOG-06 | Login con usuario bloqueado | "Epic sadface: Sorry, this user has been locked out." No se accede. | Pasa |
| TC-LOG-07 | Login con ambos campos vacíos | "Epic sadface: Username is required". No se accede. | Pasa |

## Resumen
- Casos ejecutados: 7
- Pasan: 7
- Fallan: 0

## Observaciones
- Con ambos campos vacíos, la aplicación valida primero el usuario y no muestra el aviso de contraseña hasta que el usuario está informado.
- Con usuario inexistente o contraseña incorrecta se muestra el mismo mensaje, lo que evita revelar qué usuarios existen.
- La aplicación debe probarse en inglés: con la traducción automática del navegador, los nombres de usuario cambian y el login falla (problema de entorno, no defecto).

## Bugs encontrados
Ninguno en el módulo de Login.
