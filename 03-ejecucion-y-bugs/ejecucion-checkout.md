# Ejecución de pruebas: Checkout

- **Aplicación:** https://www.saucedemo.com (en inglés)
- **Fecha de ejecución:** 23/11/2026
- **Tester:** Jhonny Gómez Campero
- **Navegador:** Chrome, con la traducción automática desactivada

## Resultados

| ID | Título | Usuario | Resultado obtenido | Estado |
|----|--------|---------|--------------------|--------|
| TC-CHK-01 | Checkout con todos los campos vacíos | standard_user | "Error: First Name is required". No se avanza. | Pasa |
| TC-CHK-02 | Checkout solo con nombre | standard_user | "Error: Last Name is required". No se avanza. | Pasa |
| TC-CHK-03 | Checkout sin código postal | standard_user | "Error: Postal Code is required". No se avanza. | Pasa |
| TC-CHK-04 | Checkout con todos los datos | standard_user | Se accede a "Checkout: Overview". | Pasa |
| TC-CHK-05 | Total del resumen correcto | standard_user | La suma manual coincide con el total. | Pasa |
| TC-CHK-06 | Finalizar la compra | standard_user | Se muestra "Thank you for your order!". | Pasa |
| TC-CHK-07 | Completar el formulario con problem_user | problem_user | Al escribir el apellido, el texto se escribe de nuevo en First Name. No se puede completar el formulario ni llegar a la confirmación. | Falla (BUG-003) |

## Resumen
- Casos ejecutados: 7
- Pasan: 6
- Fallan: 1

## Observaciones
- Con standard_user, el flujo de checkout funciona correctamente de principio a fin.
- Los defectos BUG-001 (imágenes) y BUG-002 (carrito) se detectaron con problem_user durante la exploración, sin caso de prueba formal asociado.

## Bugs encontrados
Ver bugs-problem-user.md
