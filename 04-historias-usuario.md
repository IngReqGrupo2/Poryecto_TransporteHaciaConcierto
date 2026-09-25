# Historias de usuario
 
## HU-01 — Consultar la cartelera de viajes

Como **cliente/pasajero**, quiero **explorar la cartelera y seleccionar un viaje disponible**, para **conocer las alternativas de traslado a conciertos sin tener que consultar por mensaje al administrador**.

**Actividad TO-BE asociada:** Explorar cartelera y seleccionar viaje.

**Criterios de aceptación:**
- CA1: Dado que el administrador ha registrado viajes, cuando el cliente ingresa a la cartelera, entonces el sistema muestra los viajes publicados.
- CA2: Dado que el cliente está en la cartelera, cuando selecciona un viaje, entonces el sistema muestra la información correspondiente al viaje.
- CA3: Dado que el cliente consulta un viaje, cuando se muestra su información, entonces puede conocer su disponibilidad de cupos sin solicitar una respuesta manual al administrador.
 
## HU-02 - Confirmar viaje

Como **cliente/pasajero**, quiero **reservar un cupo para el transporte** para **asistir al concierto al que quiero ir**.

**Actividad TO-BE asociada:** Reservar cupos seleccionados y actualizar cupos

**Criterios de aceptación:**
- CA1: Dado que haya encontrado un viaje de la cartelera disponible, cuando lo escoja, entonces debo poder acceder a un portal para poder pagarlo.
- CA2: Dado que haya hecho el pago de un viaje, cuando se haya realizado la transacción, entonces debe quedar registrada en el sistema la reserva.
- CA3: Dado que haya reservado un viaje, cuando se complete el pago, entonces quiero recibir una notificación con la información de mi reserva.

## HU-03 — Crear un viaje en el sistema

Como **administrador**, quiero **crear y registrar un viaje en el sistema con sus datos correspondientes**, para **publicarlo en la cartelera y gestionar los viajes sin depender de afiches y registros manuales**.

**Actividad TO-BE asociada:** Crear viaje en el sistema.

**Criterios de aceptación:**
- CA1: Dado que el administrador desea crear un viaje, cuando accede al registro de viajes, entonces el sistema permite ingresar el nombre del evento, fecha, hora de salida y regreso, conductor, asistente, modelo del vehículo y patente.
- CA2: Dado que el administrador completa los datos requeridos del viaje, cuando confirma su creación, entonces el sistema registra el viaje.
- CA3: Dado que el viaje fue registrado correctamente, cuando se publica, entonces el sistema lo incorpora a la cartelera para que pueda ser consultado por los clientes.

## HU-04 — Visualizar pasajeros

Como **asistente de viaje**, quiero **tener disponible la lista de pasajeros confirmados**, para **poder saber qué pasajeros asistieron y quiénes no**.

**Actividad TO-BE asociada:** Visualizar lista digital de pasajeros.

**Criterios de aceptación:**
- CA1: Dado que el asistente de viaje está en el día del viaje, cuando acceda a la página, el sistema deberá mostrar la lista de pasajeros registrados para el viaje.
- CA2: Dado que el asistente de viaje tiene la lista, cuando haya confirmado quiénes asistieron, entonces debe poder crearse un registro de las ausencias de la lista.
- CA3: Dado que el asistente de viaje tiene que volver desde el concierto, cuando acceda a la lista, entonces debe poder confirmar en el sistema que estén todos los pasajeros a bordo.
