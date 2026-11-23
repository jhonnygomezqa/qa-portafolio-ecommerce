# Casos de prueba: Checkout

| ID | Requisito | Título | Pasos | Resultado esperado | Prioridad |
|----|-----------|--------|-------|--------------------|-----------|
| TC-CHK-01 | RF-CHK-01 | Checkout con todos los campos vacíos | 1. Entrar con standard_user. 2. Añadir un producto y ir al carrito. 3. Pulsar Checkout. 4. Dejar todo vacío y pulsar Continue. | "Error: First Name is required". No se avanza. | Alta |
| TC-CHK-02 | RF-CHK-02 | Checkout solo con nombre | 1. Ir al formulario de checkout. 2. Informar solo First Name. 3. Pulsar Continue. | "Error: Last Name is required". No se avanza. | Alta |
| TC-CHK-03 | RF-CHK-03 | Checkout sin código postal | 1. Ir al formulario de checkout. 2. Informar nombre y apellido. 3. Pulsar Continue. | "Error: Postal Code is required". No se avanza. | Alta |
| TC-CHK-04 | RF-CHK-04 | Checkout con todos los datos | 1. Ir al formulario de checkout. 2. Informar nombre, apellido y código postal. 3. Pulsar Continue. | Se accede a "Checkout: Overview". | Alta |
| TC-CHK-05 | RF-CHK-05 | Total del resumen correcto | 1. Añadir 2 productos. 2. Llegar al resumen. 3. Sumar los precios a mano y comparar con el total. | Los productos coinciden y el total es la suma correcta. | Alta |
| TC-CHK-06 | RF-CHK-06 | Finalizar la compra | 1. En el resumen, pulsar Finish. | Se muestra "Thank you for your order!". | Alta |
| TC-CHK-07 | RF-CHK-04 | Completar el formulario con problem_user | 1. Entrar con problem_user. 2. Ir al formulario de checkout. 3. Escribir nombre, apellido y código postal en sus campos. 4. Pulsar Continue. | Cada texto se escribe en su campo y se accede al resumen. | Alta |
