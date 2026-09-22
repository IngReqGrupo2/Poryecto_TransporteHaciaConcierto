# Proceso de negocio — AS-IS
 
## Macro-proceso y proceso específico
Gestión de Ventas y Servicios de Transporte → Creación de viajes, reserva manual de asientos, pago y control de pasajeros.
 
## Objetivo de negocio del proceso
Gestionar la inscripción de los clientes a los viajes de conciertos, informando las condiciones del traslado, registrando los cupos solicitados y verificando el pago el día del evento para llenar la capacidad del furgón.

## Participantes y sus objetivos
| Participante | Objetivo en el proceso |
|---------------|------------------------|
| Cliente / Pasajero | Consultar por viajes, reservar asientos de manera sencilla sin abono previo y asistir al evento |
| Administrador | Definir precios basados en los costos, administar los asientos en una libreta, cobrar el dia del viaje y controlar asistencia |
 
## Diagrama AS-IS
![Proceso AS-IS](./diagramas/as-is.png)
 
Archivo fuente: [`./diagramas/as-is.bpmn`](./diagramas/as-is.bpmn)
 
Nota: distingan tareas de usuario, de servicio y manuales con el marcador correspondiente.
 
## Problemas identificados
- Perdida de tiempo y de potenciales clientes al tener que responder respiinder mensajes cuando no hay cupos disponibles.
- Carencia de un registro automatizado, lo que los obliga a depender de libretas manuales para llevar el control de los cupos disponibles de cada concierto.
- Riesgo de inasistencia, dado que no exigen abono previo, dejando el cobro y la verificación de pagos para el mismo día del viaje.
