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

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

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


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Habitacion<br>2. CRUD Servicio<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD Habitación<br>6. CRUD Empleado<br>7. CRUD Cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios|


### Alcance Adicional Voluntario

Diferenciación de Carteras (Portafolios Múltiples): Permitir al usuario crear un portafolio "Real" y otro "De Prueba" (Simulado/Paper Trading). Esto es genial para testing y suma mucha lógica de negocio al código.

Manejo de Multidivisas (Dólar/Peso): Como los activos pueden cotizar en dólares (criptos, acciones de afuera) o en pesos (CEDEARs), un dolor de cabeza real es unificar todo. Si sumás una conversión automática basada en el tipo de cambio del día, estéticamente y a nivel lógico es un golazo.

Alertas de Precios: Un sistema simple donde el usuario configure: "Avisame si Bitcoin baja de USD 60,000". Puede ser una notificación visual en el dashboard o, si te querés pasar de nivel, un bot de Telegram integrado que mande un mensaje.

Exportación de Datos: Un botón para descargar el historial de transacciones en formato CSV o Excel. Es una funcionalidad simple de implementar pero que le da un cierre muy profesional al sistema.


|Req|Detalle|
|:-|:-|
|Listados |1. Muestra un resumen consolidado de todos los activos que posee el usuario en su portafolio. <br>2. Muestra el cálculo de ganancias/pérdidas (ROI) exclusivo de ese activo , junto con la lista histórica de todas las compras y ventas que el usuario realizó sobre ese ticker en particular.|



