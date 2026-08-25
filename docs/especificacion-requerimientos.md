# Especificación de Requerimientos



## 1. Descripción del sistema



## 2. Integrantes



- Nombre:Luis Felipe Sanchez Rodriguez

- Nombre: Sofia Navia Crespo

- Nombre: Carlos Andres Artunduaga Galarza

- Nombre: Camilo Alejandro Bermeo Zorrilla

- Nombre: Juan Manuel Ospina Riascos 



## 3. Requerimientos Funcionales



### RF-01 - \[Nombre del requerimiento]



#### Resumen



#### Entradas



| Entrada | Tipo de dato | Descripción |
|---|---|---|



#### Reglas o condiciones



#### Salidas



| Salida | Tipo de dato | Descripción |
|---|---|---|



#### Resultado esperado





### RF-02 - \[Nombre del requerimiento]



#### Resumen



#### Entradas



| Entrada | Tipo de dato | Descripción |
|---|---|---|



#### Reglas o condiciones



#### Salidas



| Salida | Tipo de dato | Descripción |
|---|---|---|



#### Resultado esperado





### RF-03 - \[Nombre del requerimiento]



#### Resumen



#### Entradas



| Entrada | Tipo de dato | Descripción |
|---|---|---|



#### Reglas o condiciones



#### Salidas



| Salida | Tipo de dato | Descripción |
|---|---|---|



#### Resultado esperado





### RF-04 - Cancelar participación



#### Resumen
El sistema deberá permitir a un estudiante cancelar su inscripción en una tutoría previamente registrada, proporcionando su código estudiantil y el identificador único de la tutoría.

#### Entradas



| Entrada | Tipo de dato | Descripción                                                                                            |
|---|---|--------------------------------------------------------------------------------------------------------|
| idEstudiante | String | Código estudiantil que identifica de forma única al estudiante dentro de la Universidad.               |
| idTutoria | String | Identificador único de la tutoría, generado automáticamente por el sistema al momento de su creación.  |



#### Reglas o condiciones
Para que la cancelación sea exitosa, deben cumplirse todas las siguientes condiciones:

1. El estudiante debe encontrarse registrado como inscrito en la tutoría especificada.
2. La fecha y hora actual deben ser anteriores a la fecha y hora de inicio de la tutoría.
3. El estudiante debe encontrarse en estado activo dentro de la Universidad. 
Si alguna de estas condiciones no se cumple, la cancelación no debe realizarse.

#### Salidas

| Salida       | Tipo de dato | Descripción                                                                                         |
|--------------|---|-----------------------------------------------------------------------------------------------------|
| mensajeExito | String | Mensaje de confirmación que indica que la cancelación de la inscripción fue realizada exitosamente. |
| mensajeError | String | Mensaje descriptivo que informa al estudiante el motivo específico por el cual no fue posible realizar la cancelación.|




#### Resultado esperado
En caso de éxito:
- El sistema debe eliminar el registro de inscripción asociado al estudiante y a la tutoría.
- El sistema debe incrementar en 1 la cantidad de cupos disponibles para esa tutoría.
- El sistema debe mostrar un mensaje de confirmación al estudiante.

En caso de fallo:
- No se debe modificar ningún dato en el sistema.
- El sistema debe mostrar un mensaje de error indicando claramente la causa del rechazo.


### RF-05 - \[Nombre del requerimiento]



#### Resumen



#### Entradas



| Entrada | Tipo de dato | Descripción |
|---|---|---|



#### Reglas o condiciones



#### Salidas



| Salida | Tipo de dato | Descripción |
|---|---|---|



#### Resultado esperado





## 4. Gestión de Versiones



### Ramas utilizadas



### Proceso de integración



### Conflictos encontrados

