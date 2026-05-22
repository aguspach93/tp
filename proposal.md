# Propuesta TP DSW

## Grupo
### Integrantes
* 47787 - Pacheco, Agustin Ariel
* 51636 - Vera, Maximiliano

### Repositorios
* [frontend app](http://github.com/aguspach93/frontend)
* [backend app](http://github.com/aguspach93/backend)

## Tema
### Descripción

El proyecto consiste en el desarrollo de una plataforma web interactiva diseñada para la gestión, control y optimización de portafolios de inversión personales. La aplicación centraliza el registro de operaciones de compra y venta de diversos tipos de activos financieros (como acciones de bolsa y criptomonedas), procesando los datos históricos para ofrecer métricas clave de rendimiento en tiempo real.

### Modelo

*Nota*: 

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Transacciones<br>2. CRUD Activos<br>3. CRUD Usuarios.<br>4. CRUD Alertas|
|CRUD dependiente|1. CRUD Alertas {depende de} CRUD Activos<br>2. CRUD Transacciones {depende de} CRUD Usuarios|
|Listado<br>+<br>detalle| 1. Listado de transacciones filtrado por tipo de activo, muestra nro de transaccion => detalle activo|
|CUU/Epic|1. Registrar una transaccion de compra de criptomonedas<br>2. Solicitar un alerta de un activo|



### Alcance Adicional Voluntario

Diferenciación de Carteras: Permite al usuario administrar un portafolio "Real" y uno "Simulado" (Paper Trading). Esto facilita la validación de estrategias en un entorno de pruebas y aporta robustez a la lógica de negocio.

Gestión Multidivisa: Dado que los activos cotizan en distintas monedas (pesos y dólares), el sistema unificará la valoración de la cartera. Se implementará una conversión automática según el tipo de cambio diario, asegurando consistencia técnica y visual.

Alertas de Precios: Sistema que permite al usuario configurar umbrales de cotización personalizados. Las notificaciones podrán visualizarse directamente en el panel de control o enviarse de forma automatizada a través de una integración con Telegram.

Exportación de Datos: Funcionalidad para descargar el historial de transacciones en formato CSV o Excel. Su implementación es eficiente y añade un alto nivel de profesionalismo e interoperabilidad al sistema.


|Req|Detalle|
|:-|:-|
|Listados |1. Muestra un resumen consolidado de todos los activos que posee el usuario en su portafolio. <br>2. Muestra el cálculo de ganancias/pérdidas (ROI) exclusivo de ese activo , junto con la lista histórica de todas las compras y ventas que el usuario realizó sobre ese ticker en particular.|



