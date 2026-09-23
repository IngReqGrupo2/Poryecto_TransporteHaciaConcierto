# Clasificación de requisitos

## Requisitos de producto

| ID | Requisito | Tipo (funcional/no funcional) | Actividad TO-BE asociada |
|----|-----------|--------------------------------|---------------------------|
| RP-01 | El sistema debe permitir al administrador crear un viaje registrando la información necesaria para su publicación, incluyendo nombre del evento, fecha, hora de salida y regreso, conductor, asistente, vehículo y patente. | Funcional | Crear viaje en el sistema |
| RP-02 | El sistema debe generar y mostrar una cartelera de los viajes disponibles a partir de los viajes registrados por el administrador. | Funcional | Crear viaje en el sistema |
| RP-03 | El sistema debe permitir al cliente explorar la cartelera y seleccionar un viaje para consultar su información y disponibilidad. | Funcional | Explorar cartelera y seleccionar viaje |
| RP-04 | El sistema debe validar automáticamente la disponibilidad de cupos de un viaje antes de permitir una reserva, respetando la capacidad máxima definida para el vehículo. | Funcional | Validar disponibilidad de cupos |
| RP-05 | El sistema debe informar al cliente cuando un viaje no posea cupos disponibles e impedir que se realicen nuevas reservas para dicho viaje. | Funcional | Notificar indisponibilidad |
| RP-06 | El sistema debe permitir al pasajero registrar una reserva ingresando los datos requeridos para la nómina: RUT, nombre, apellidos y teléfono de contacto. | Funcional | Registrar reserva y pasajero |
| RP-07 | El sistema debe registrar automáticamente al pasajero y asociarlo al viaje seleccionado una vez realizada la reserva. | Funcional | Registrar reserva y pasajero |
| RP-08 | El sistema debe permitir al pasajero realizar el pago en línea asociado a su reserva mediante los medios de pago habilitados en la plataforma. | Funcional | Procesar pago en línea |
| RP-09 | El sistema debe registrar el estado del pago asociado a cada reserva para que la administración pueda identificar los pasajeros con pago confirmado. | Funcional | Procesar pago en línea |
| RP-10 | El sistema debe generar una lista digital de pasajeros para cada viaje a partir de las reservas registradas. | Funcional | Visualizar lista digital de pasajeros |
| RP-11 | El sistema debe permitir al administrador consultar la lista digital de pasajeros correspondiente a cada viaje. | Funcional | Visualizar lista digital de pasajeros |
| RP-12 | La interfaz utilizada por los clientes debe ser compatible con dispositivos móviles, considerando que estos utilizan principalmente teléfonos al realizar las reservas. | No funcional | Explorar cartelera y seleccionar viaje / Registrar reserva y pasajero |
| RP-13 | La vista de administración debe presentar la información de los viajes y pasajeros mediante una estructura tipo agenda, manteniendo una organización familiar para el administrador. | No funcional | Crear viaje en el sistema / Visualizar lista digital de pasajeros |

## Requisitos de proyecto

| ID | Requisito |
|----|-----------|
| RY-01 | El sistema debe tener como meta de implementación enero de 2027. |
| RY-02 | El desarrollo debe considerar como alcance inicial la cartelera de viajes a conciertos, la reserva autónoma de cupos y el registro automatizado de los pasajeros y asientos reservados. |
| RY-03 | El desarrollo del proyecto deberá utilizar como fuente de requisitos la información obtenida mediante la entrevista al stakeholder y la revisión de la documentación operativa de la empresa. |

## Requisito derivado

**Requisito origen:** RP-04 — El sistema debe validar automáticamente la disponibilidad de cupos de un viaje antes de permitir una reserva, respetando la capacidad máxima definida para el vehículo.

**Requisito derivado:** RP-D01 — Cuando una reserva sea registrada correctamente, el sistema debe descontar automáticamente los cupos correspondientes de la disponibilidad del viaje antes de permitir una nueva reserva.

**Justificación:** Para validar correctamente la disponibilidad y evitar que un viaje supere la capacidad máxima del vehículo, el sistema necesita mantener actualizada la cantidad de cupos disponibles después de cada reserva. Este requisito se deriva de RP-04, ya que sin la actualización automática de cupos no sería posible garantizar que la validación de disponibilidad utilice información vigente.
