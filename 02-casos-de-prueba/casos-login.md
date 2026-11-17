# Casos de prueba: Login

| ID | Requisito | Título | Pasos | Resultado esperado | Prioridad |
|----|-----------|--------|-------|--------------------|-----------|
| TC-LOG-01 | RF-LOG-01 | Login con credenciales válidas | 1. Abrir la web en inglés. 2. Introducir standard_user y su contraseña. 3. Pulsar Login. | Se accede al catálogo de productos. | Alta |
| TC-LOG-02 | RF-LOG-02 | Login con usuario vacío | 1. Dejar el usuario vacío. 2. Introducir contraseña válida. 3. Pulsar Login. | Mensaje de error de usuario obligatorio. No se accede. | Alta |
| TC-LOG-03 | RF-LOG-03 | Login con contraseña vacía | 1. Introducir standard_user. 2. Dejar la contraseña vacía. 3. Pulsar Login. | Mensaje de error de contraseña obligatoria. No se accede. | Alta |
| TC-LOG-04 | RF-LOG-04 | Login con contraseña incorrecta | 1. Introducir standard_user. 2. Introducir una contraseña inventada. 3. Pulsar Login. | Mensaje de error de credenciales incorrectas. No se accede. | Alta |
| TC-LOG-05 | RF-LOG-04 | Login con usuario inexistente | 1. Introducir un usuario inventado. 2. Introducir contraseña válida. 3. Pulsar Login. | Mensaje de error de credenciales incorrectas. No se accede. | Media |
| TC-LOG-06 | RF-LOG-05 | Login con usuario bloqueado | 1. Introducir locked_out_user y su contraseña. 2. Pulsar Login. | Mensaje: "Sorry, this user has been locked out." No se accede. | Alta |
| TC-LOG-07 | RF-LOG-01 | Login con ambos campos vacíos | 1. Dejar usuario y contraseña vacíos. 2. Pulsar Login. | Mensaje de error. No se accede. | Media |
