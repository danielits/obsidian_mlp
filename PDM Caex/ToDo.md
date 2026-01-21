
- [x] Info en excel en caex
- [ ] Posibilidad de que la aplicación determine el orden de ingreso de los camiones a mantención por prioridades (Contactar con Jaime Rojo)
- [ ] Parámetro "Horometro de Motor (Hr)" ingestar desde Sesion Vehicle Hours Collection
- [x] responder correo soporte sobre camion CA104 con estado efectivo, pero sin datos en minecare. Reportado por usuario Jaime
- [ ] Responder correo cambion CA104 con respecto a cambiar el icono para indicar que no hay data
- [ ] responder correo a Oscar Ducret sobre camión CA95
- [x] CA87 no tiró el error de carter cuando 28-10 ll
- [ ] Corroborar camiones MTU sacados filtrando por ParameterName




Fernando Antonio es el administrador de contrato con cummins? quien es?


Engine Injector Metering Rail 1 Pressure'',

''Engine Injector Timing Rail 1 Pressure''

''Pre-Filter Oil Pressure (QSK60)''
''Engine Pre-filter Oil Pressure''

''Post-Filter Oil Pressure''
''Post-Filter Oil Pressure (QSK60)''
''Post-Filter Oil Pressure (FF08) - Byte 1''



Reu con pablo y nacho para entender el flujo de aprobacion de alertas

rechazo viene de los moncon
el rechazo en el punto 9 del flujo se refiere al cierre de la alertas, osea si sigue con condicion mala y ejecucion dijo que estaba listo, moncon puede rechazar el cierre

definir nombres nuevos con oscar y cambiar la historia

AVISO LUEGO OT; aviso es aviso q hay un problema y despues alguien crea una OT en base a ese aviso

añadir glosario de los estados




Supervisor [son 7x7 y debiesen haber 4], no supervisan a los viejos, sino al contrato (nexo directo con supervisores de Cummins) > Jefe de turno [7x7 son 2, solo turno dia] > Senior de mantenimiento (Luis Cid, por confirmar)      **Quizas no hay jefes de turno en la figura y es solo jefe de los supervisores




fugas de refrigerante y de aceite son los que dejan detenidos los caex en la mina, o fallas electricas

oscar dice q actualmente no podemos prevenir camiones parados porque no tenemos eso parámetros, pero es mucho mas fácil q los viejos revisen los niveles.

Falta incorporar camiones MTU, mejor actualización de horómetros, que te avisen cuando han cambiado los motores. orden de criticidad o prevenir casos tiene q ver mas con los moncon q con la herramienta

ejecución nunca ha tenido la herramienta en su proceso, por otro lado, nadie pesca lo que dice moncon. procesos podría hacer sinergia con los de ejecución, acabar con lo de q alguien dice q es buen aviso, otro con mal aviso. necesitamos el feedback de gestion de las alertas, entonces no podemos mejorar el patron de alerta. nos piden mejorarlo pero no tenemos feedback

pedir las causas de detención en pista del año pasado


el espíritu de la herramienta actual es gestion de alerta y prevenir fallas catastróficas, detenciones en pista ya lo tiene minecare

seria bueno saber donde emiten las alertas minecare y contar por ejemplo las de refrigerante


Fernando quiere generar avisos, Luis cid no quiere porque les pega en sus kpis. aviso sap sirve pa meter presión. falta aliado para esto, puede ser super de confiabilidad, Fernando (principal), Claudio quizas. Mas que enfocarnos en que no quieren el aviso por pegarle al kpi deberiamos hacer una conversacion del tipo de alertas lleguen para no spamear y que genere valor tanto para ellos como para nosotros

baja presión de combustible por filtro saturado es el motivo principal de baja potencia en los camiones MCRS. por semana unos 3 o 4 camiones caen por baja potencia. baja potencia se avisan por códigos, de aviso a mas criticidad