# QA Portafolio E-commerce

Proyecto práctico de QA manual sobre una tienda online de prueba
(https://www.saucedemo.com). Cubre el ciclo completo: análisis de
requisitos, casos de prueba, ejecución y reporte de bugs.

## Alcance
- Login
- Checkout (incluye el carrito)

## Resultados

| Módulo | Casos ejecutados | Pasan | Fallan |
|--------|------------------|-------|--------|
| Login | 7 | 7 | 0 |
| Checkout | 7 | 6 | 1 |

**Bugs encontrados:** 3, todos con el usuario de prueba `problem_user`
(2 de severidad alta y 1 media).

## Estructura del repositorio

| Carpeta | Contenido |
|---------|-----------|
| [01-analisis-requisitos](01-analisis-requisitos) | Requisitos y criterios de aceptación (formato Dado/Cuando/Entonces) |
| [02-casos-de-prueba](02-casos-de-prueba) | Casos de prueba con trazabilidad a los requisitos |
| [03-ejecucion-y-bugs](03-ejecucion-y-bugs) | Resultados de la ejecución, reportes de bugs y evidencias |

## Herramientas
GitHub, Markdown, Chrome.

## Estado
En progreso. Próximos pasos: pruebas del catálogo y del carrito con
standard_user, y pruebas de API con Postman.

## Autor
Jhonny Gómez Campero, QA Tester Manual (Málaga).
