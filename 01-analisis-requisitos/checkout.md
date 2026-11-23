# Checkout: análisis de requisitos

- **Aplicación:** https://www.saucedemo.com (en inglés)
- **Fecha de análisis:** 23/11/2026
- **Método:** exploración manual con standard_user

## Requisitos funcionales

| ID | Requisito |
|----|-----------|
| RF-CHK-01 | El sistema exige el nombre para continuar con el checkout. |
| RF-CHK-02 | El sistema exige el apellido para continuar con el checkout. |
| RF-CHK-03 | El sistema exige el código postal para continuar con el checkout. |
| RF-CHK-04 | Con todos los datos informados, el usuario avanza a la pantalla de resumen del pedido. |
| RF-CHK-05 | El resumen muestra los productos añadidos y un total correcto. |
| RF-CHK-06 | Al finalizar, el sistema muestra un mensaje de confirmación del pedido. |

## Criterios de aceptación

**RF-CHK-01**
- Dado que estoy en el formulario de checkout con el carrito con productos
- Cuando dejo todos los campos vacíos y pulso Continue
- Entonces no avanzo y se muestra el mensaje: "Error: First Name is required"

**RF-CHK-02**
- Dado que estoy en el formulario de checkout
- Cuando informo solo el nombre y pulso Continue
- Entonces no avanzo y se muestra el mensaje: "Error: Last Name is required"

**RF-CHK-03**
- Dado que estoy en el formulario de checkout
- Cuando informo nombre y apellido, sin código postal, y pulso Continue
- Entonces no avanzo y se muestra el mensaje: "Error: Postal Code is required"

**RF-CHK-04**
- Dado que estoy en el formulario de checkout
- Cuando informo nombre, apellido y código postal y pulso Continue
- Entonces accedo a la pantalla "Checkout: Overview"

**RF-CHK-05**
- Dado que estoy en la pantalla de resumen
- Cuando reviso los productos y el total
- Entonces los productos coinciden con los que añadí y el total es la suma correcta

**RF-CHK-06**
- Dado que estoy en la pantalla de resumen
- Cuando pulso Finish
- Entonces se muestra el mensaje: "Thank you for your order!"

## Observaciones
- La validación de campos sigue un orden fijo: primero nombre, luego apellido y luego código postal. Solo se muestra un error cada vez.
