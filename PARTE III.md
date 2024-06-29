# Propuesta del Caso de Negocio
a. Solución de Machine Learning
   Algoritmo de clasificación supervisado que permita identificar clientes con mayor probabilidad de ingresar en mora
   
b. Preguntas clave del framework
   Que: 
   - ¿Por que ingresan en mora los clientes de una entidad financiera? Por reducción de sus ingresos, incremento de sus gastos, mala cultura financiera
   - ¿Qué se viene haciendo para mitigar el ingreso en mora en una entidad financiera? Llamando a todos los clientes el dia de su pago
   - ¿Cómo impactan en las finanzas los clientes morosos en la entidad financiera? Disminuye el recaudo, además de aumentar el gasto de provisión
  Entonces que:
   - ¿Cómo se usará el modelo en la gestión preventiva? Se clasificaran y se gestionará con mayor intensidad a los clientes de alto riesgo, además de ofrecerles campañas de cobranzas
   - ¿Que tal un sorteo para los clientes al dia?  Incentivar a los clientes puede evitar la mora.
  Ahora que:
   - Evaluación continua del rendimiento del modelo: Mantenimiento y actualización del algoritmo.
   - ¿Cuando se empezará con la nueva estrategia? Una vez realizada la segmentación de clientes (bajo riesgo vs alto riesgo), se escogerá un porcentaje de estos para la prueba piloto.
   - ¿Qué áreas necesitan estar involucradas? Área de marketing, área de finanzas
c. Considere las suposiciones necesarias y elija la métrica adecuada
-Beneficios esperados: Disminución de clientes que entran en mora en un 20%.
-Costo de provisión de los clientes que ingresan en mora.
d. Estime el valor monetario incremental basado en las suposiciones y la acción o palanca implementada.
PALANCA: Ofrecer campaña de descuento de 10% de la cuota para los clientes de alto riesgo
Suposición sin modelo:
  Base de clientes al dia: 1000
  Tasa de ingreso a mora (mensual): 10%
  Recaudo promedio: 200
  Recaudo de la cobranza: 1000*90%*200=180000

Suposición con modelo:
  Base de clientes al dia: 1000
  Tasa de ingreso a mora (mensual): 8%
  Recaudo promedio: 200
  Recaudo de la cobranza : 1000*92%*200=184000

Beneficio: 184000-180000=4000
 Costos falso positivos: De los 1000 clientes, el 15% son clasificados como alto riesgo. De estos 150 clientes 10 eran de bajo riesgo, por lo que no era necesario darle el descuento de la cuota

10*0.1*200 = 200


Costos falsos negativos: 5 clientes malos, no fueron clasificados como alto riesgo
5*200 = 1000
