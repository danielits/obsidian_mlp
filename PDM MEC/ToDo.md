- [ ] Sesión integración mina
- [ ] Definir usuarios y lógica (aprobación superintendente y p&d)
- [x] Definir qué data se necesita de SAP en función de lo que se quiera mostrar
- [x] Confirmar query SQL actual de SAP (solo vemos las revisiones)
- [ ] Sacar Plan Semanal de las opciones del dropdown en el modal
- [ ] RoadMap del front para los usuarios
- [ ] Definir nuevo usuario de Chancado y Correa (Francisco va a averiguar), Cristian Ponce no está hasta fin de mes
- [ ] "segunda ola" con planes semanales desarrollando un formulario para los planes semanales, despues MEC solo usa esa data
- [ ] Añadir filtro de fecha en front


Integración SAP
- [ ] No hay estandar general por el momento en los codigos de mantenciones mayores y menores, asi que por ahora filtrar datos que correspondan a planes semanales
- [ ] Jose Ignacio Moya del area de DAA (analitica avanzada) de amsa pidio la ingesta de la transaccion iw37n. Matias Gallego es de su equipo y puede tener mas informacion
- [ ] Añadir pestaña Overview para visualización indicadores SAP, por ahora tenemos el numero de ordenes por revision. Luego sera cantidad de operaciones, suma de costos estimados (materiales), suma de costos planificados (materiales),  suma de costos reales (materiales)
- [ ] "Replicar" overview de ductos
- [ ] Crear delta para historizar evolucion de las ordenes, por cantidad de datos partamos con historizacion semanal, probar con frecuencia diaria [se podria tener una tabla de snapshot y un historico de modificaciones]
- [ ] Añadir costo de materiales (zpm_014) y HH (iw37n) en (campos obligatorios) la planificacion en el menu de edicion. luego se contrasta y grafica con la data de SAP
- [ ] Incorporar grafico costos por revision (estimado, planificado y real) (ver imagen).
![[Pasted image 20251111105307.png]] *Esto es por revisión, en la iw39 están por orden, hay que sumar las correspondientes a cada revisión*
- [ ] mismo tipo de grafico para trabajo HH son planificadas y reales (solo 2 columnas). columnas trabajo y trabajo_real de la iw37n
- [ ] Añadir en la edicion de revisiones el Presupuesto y HH como input para los planificadores



OIOB - Listado Revisiones SAP
![[Pasted image 20251203150623.png]]
- [ ] cambiar el front para mostrar tablas de revisiones, no por transaccion, distintas transacciones pueden estar en la misma tabla, añadir en la primera todos los campos de la OIOB - Listado Revisiones SAP. concatenar fecha inicio con hora inicio y fecha fin con hora fin
- [ ] graficos en overview no muestran nada si no he seleccionado una revision
- [ ] 

iw37n,
Orden: Borrar ceros a la izquierda (int)
clase_orden
texto_breve
operacion
texto_breve_operacion
estado_sistema
status_de_usuario
trabajo
trabajo_real
fecha_real
hora_real
centro_emplazamiento
pto_trabajo_responsable
grupo_planificacion

Falta la ingesta de la transaccion mb25, la tabla esta vacia. La consultamos de nuevo y tenia datos asi que quizas la leimos justo cuando se estaba escribiendo en ella o algo asi

mb25 y zmm 060 puedo sacar el costo, P * Q, tiene q ver el costo unitario tambien

DEMO ACTUALIZADA



# Integración Mina

Resumen

Fernando COrnejo, SI de Planificacion TFT & Puerto

Cristian Ponce por el area de STMG, Ingeniero senior de planificacion chancado y correa
