# PredicciÓn_para_abrir_nuevos_pozos_petroleros
Creacion de un modelo de regresion logistica para predecir la region  en donde el riesgo es menor y hay mayores ganancias
# Introducción
Encontrar los **mejores lugares para abrir 200 pozos nuevos** de petróleo en la compañía de extacción de petróleo OilyGiant
- Vamos a crear un modelo para predecir el volumen de reservas en pozos nuevos.
- Elegir los pozos petrolíferos que tienen los valores estimados más altos.
- Elegir la región con el **beneficio total** más alto para los pozos petrolíferos seleccionados.

- Crear un modelo que ayude a elegir la región con **el mayor margen de beneficio**. Analizar los beneficios y riesgos potenciales utilizando la técnica bootstrapping.
**Condiciones:**
- Al explorar la región, se lleva a cabo un estudio de 500 puntos con la selección de los mejores 200 puntos para el cálculo del beneficio.
- El presupuesto para el desarrollo de 200 pozos petroleros es de 100 millones de dólares.
- Un barril de materias primas genera 4.5 USD de ingresos. El ingreso de una unidad de producto es de 4500 dólares (el volumen de reservas está expresado en miles de barriles).
- Después de la evaluación de riesgo, mantendremos solo las regiones con riesgo de pérdidas inferior al 2.5%. De las que se ajustan a los criterios, se debe seleccionar la región con el beneficio promedio más alto.
- Los datos son sintéticos: los detalles del contrato y las características del pozo no se publican.
