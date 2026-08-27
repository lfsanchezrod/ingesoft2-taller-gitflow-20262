# Especificación de Requerimientos



## 1. Descripción del sistema



## 2. Integrantes



- Nombre:Luis Felipe Sanchez Rodriguez

- Nombre: Sofia Navia Crespo

- Nombre: Carlos Andres Artunduaga Galarza

- Nombre: Camilo Alejandro Bermeo Zorrilla

- Nombre: Juan Manuel Ospina Riascos 



## 3. Requerimientos Funcionales



### RF-01 - \Registrar tutoria


#### Resumen

El docente proporcionará los datos necesarios para establecer un espacio de tutoria como lo son fecha, hora,
tema, cantidad de estudiantes y su codigo, de ahi se dará un mensaje al docente confirmando su espacio

#### Entradas



| Entrada   | Tipo de dato | Descripción                                           |
|-----------|---|-------------------------------------------------------|
| Codigo    |String| El identificador unico del profesor en la universidad |
| Tema      |String| El tema que se tratará la tutoria                     |
| Fecha     |LocalDate| La fecha que se dará la tutoria                       |
| HoraInicio|int| La hora en que inicia la tutoria                      |
|Cantidad|int|La cantidad de estudiantes que pueden asistir a la tutoria |


#### Reglas o condiciones

- La fecha no puede ser una anterior a la fecha actual
- La cantidad maxima de estudiantes es de 10

#### Salidas


| Salida       | Tipo de dato | Descripción |
|--------------|---|---|
| Confirmación |String|Mensaje que confirma la asignacion "Su tutoria ha sido creada"|




\#### Resultado esperado





\### RF-02 - Consultar tutorias



\#### Resumen

Los estudiantes podrán consultar las tutorias que se encuentran disponibles, se buscan indicando una fecha especifica,
y opcionalmente, indicar una asignatura o temas de interes.

\#### Entradas



| Entrada   | Tipo de dato | Descripción                                                |
|-----------|---|------------------------------------------------------------|
| Fecha     |LocalDate| La fecha que se dará la tutoria                            |
| Tema      |String| El tema de interés que se tratará la tutoria               |



\#### Reglas o condiciones

- La fecha debe ser una fecha válida.
- La fecha es obligatoria.
- La asignatura o tema es opcional.
- Solo se deben mostrar tutorías que correspondan con la fecha indicada.
- Si se proporciona una asignatura o tema, la tutoría debe coincidir con este criterio de búsqueda.

\#### Salidas



| Salida        | Tipo de dato | Descripción                                                                        |
|---------------|---|------------------------------------------------------------------------------------|
| Identificador |String| El identificador único de cada tutoria                                             |
| Tema          |String| El tema que se tratará la tutoria                                                  |
| Fecha         |LocalDate| La fecha que se dará la tutoria                                                    |
| Hora          |int| La hora de la tutoria                                                              |
| Cupos         |int| La cantidad de estudiantes que pueden asistir a la tutoria                         |
| Mensaje       |String| Mensaje que informa que no se encontaron tutorias que correspondan con su búsqueda |


\#### Resultado esperado





\### RF-03 - \[Nombre del requerimiento]



\#### Resumen



\#### Entradas



| Entrada | Tipo de dato | Descripción |

|---|---|---|



\#### Reglas o condiciones



\#### Salidas



| Salida | Tipo de dato | Descripción |

|---|---|---|



\#### Resultado esperado





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


\### RF-05 - \[Nombre del requerimiento]



\#### Resumen



\#### Entradas



| Entrada | Tipo de dato | Descripción |

|---|---|---|



\#### Reglas o condiciones



\#### Salidas



| Salida | Tipo de dato | Descripción |

|---|---|---|



\#### Resultado esperado





\## 4. Gestión de Versiones



\### Ramas utilizadas



\### Proceso de integración



\### Conflictos encontrados

