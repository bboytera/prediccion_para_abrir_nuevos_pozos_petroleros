# Predicción_para_abrir_nuevos_pozos_petroleros
Creacion de un modelo de Regresión Logistica para predecir la region  en donde el riesgo es menor y hay mayores ganancias
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
# Descripción de los datos
Los datos de exploración geológica de las tres regiones se almacenan en estos 3 archivos:

- 'geo_data_0.csv'. 
- 'geo_data_1.csv'. 
- 'geo_data_2.csv'. 


  - `id`  — identificador único de pozo de petróleo
  - `f0, f1, f2` — tres características de los puntos (su significado específico no es importante, pero las características en sí son significativas)
  -`product`— volumen de reservas en el pozo de petróleo (miles de barriles).
# Habilidades técnicas
- `Phyton`
- `Numpy`
- `Pandas`
- `Matplotlib`
- `Scikit-learn`
- `Scipy`
-  bootstrapping`
- `Validación cruzada`
# Conclusiones generales
- Realizamos un (EDA) de cada una de las regiones asi como un preprocesamiento de los datos
- Separamos las caracteristicas y obtetivos con un 75% en el conjunto de entrenamiento y un 25% en el conjunto de validación
- Creamos un modelo para cada región de Regresión Logogistica y lo entrenamos
- Obtuvimos el volumen medio en las predicciones en el conjunto de validación de cada modelo (para calcular las ganancias)y calculamos el RECM y R2_score para cada región
- analizamos los riesgos y las ganancias parta cada region usando bootstrapping
- La región con menos riesgos y mayores ganacias mayores a 4 millones de dolares fue la **Región 2!!**
