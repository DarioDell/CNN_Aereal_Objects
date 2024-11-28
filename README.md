# CNN_Aereal_Objects
El objetivo del proyecto es el desarrollo de una red neuronal convolucional para la clasificación de imágenes de diferentes objetos aéreos.<br>

La red neuronal convolucional clasificará las imágenes en 7 clases diferentes (asociadas a cada uno de los subdirectorios) y posteriormente, en función de esta clasificación, se le asignará un riesgo a la imágen que se ha detectado:
- NO HAY RIESGO: Imágenes de pájaros 
- POCO RIESGO: Imágenes de aviones civiles, paracaídas, dirigibles, globos, parapentes, transbordadores espaciales
- RIESGO MEDIO: Imágenes de drones y helicópteros. 
- RIESGO ALTO: Imágenes de aeronaves militares y misiles.

Para la elaboración del presente trabajo se han utilizado diferentes librerías del lenguaje de programación Python como pueden ser TensorFlow, Keras, Matplotlib, Scikit-Learn o Pandas entre otras.<br>
El dataset que utilizo está compuesto por más de 41600 imágenes de diferentes resoluciones que he descargado de distintas fuentes y se han almacenado en un directorio local --> FLY.zip<br>

Dentro de este directorio se han agrupado las imágenes por clases teniendo los siguientes subdirectorios: 
- plane (imágenes de aviones civiles),
- military_plane (imágenes de aeronaves militares como cazas o aviones de transporte, incluye helicópteros militares),
- dron (incluye imágenes de cualquier tipo de dron por estar considerados un posible riesgo sea cual sea su tamaño),
- helicopter (incluye imágenes de helicópteros de uno y dos rotores),
- missile (incluye imágenes de diferentes tipos de misiles),
- bird (incluye imágenes de diferentes tipos de pájaros),
- others (incluye diferentes imágenes de paracaídas, dirigibles, globos, parapentes, transbordadores espaciales).<br>

Las más de 41600 imágenes se han distribuído de la siguiente forma:
- 8165 imágenes para plane. 
- 7330 imágenes para military_plane. 
- 5103 imágenes para bird. 
- 3289 imágenes para others. 
- 5116 imágenes para helicopter 
- 5149 imágenes para dron
- 7449 imágenes para missile

<u>Organización del proyecto:</u>
- Elección correcta del dataset. Ajustar la cantidad y calidad de las imágenes obtenidas de repositorios públicos de diferentes páginas web
- Realizar el preprocesamiento del dataset de imágenes. Normalizar los datos, conversión de los datos al tipo correcto, elección de la resolución de las imágenes y si estas serán a color o en blanco y negro. 
- Establecer la arquitectura general que tendrá la red neuronal. Decidir cuántas capas convolucionales tendrá la red. 
- Realizar el ajuste de los hiperparámetros de la red. Realizar diferentes pruebas para establecer el tamaño de los filtros de las convoluciones, el tamaño de pooling, el optimizador, la tasa de aprendizaje y el tamaño de normalización por lotes. 
- Prevenir sobreajuste con regularización, Early Stopping o Dropout. 
- Comparar los resultados obtenidos del modelo con alguna otra red.

  *DIFICULTADES*
  Uno de los principales desafíos que enfrenté al realizar el siguiente análisis con redes neuronales convolucionales aplicadas a imágenes aéreas fue la limitada cantidad y calidad de las imágenes disponibles en los datasets de fuentes como Kaggle o roboflow. Aunque 
  estos conjuntos de datos 
  proporcionaron un punto de partida valioso, muchos presentaban imágenes de baja resolución o insuficientes para capturar la variabilidad necesaria para entrenar un modelo robusto. Estoy convencido de que, con un mayor volumen de imágenes y una resolución más alta, el 
  modelo habría alcanzado un mejor desempeño, ya que estos factores son cruciales para extraer características más precisas y representativas durante el entrenamiento.
