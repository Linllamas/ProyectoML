# Resultados y conclusiones 

## Resultados de los modelos

-	**AdaBoost**: Este modelo tiene un RMSE de 0.012404 y un R^2 de 0.899520. Si bien muestra un buen ajuste a los datos, es superado en términos precisión (RMSE) y capacidad explicativa de la variabilidad de los datos (R^2) por otros modelos tradicionales como SVM y Random Forest. 
-	**Ridge**: El modelo Ridge tiene un RMSE de 0.025393 y un R^2 de 0.794298, este fue el modelo tradicional que tuvo los peores resultados en términos de RSME y R^2, es decir, es el que menos confiabilidad nos brinda al momento de predecir las calificaciones de los libros. 
-	**Random Forest**: Este modelo destaca con un RMSE sorprendentemente bajo de 0.002106 y un alto R^2 de 0.982939. De los modelos tradicionales, es el que mejor precisión y capacidad explicativa de los datos y la explicación de los mismos. 
-	**SVM (Support Vector Machine)**: El SVM tiene un RMSE de 0.004392 y un R^2 de 0.964418, lo que indica un buen rendimiento en la predicción, aunque es un buen modelo, Random Forest tiene mejores resultados. 
-	**Stacking**: El modelo de Stacking es el claro ganador con un RMSE excepcionalmente bajo de 0.000300 y un R^2 de 0.997566. Esto significa que el modelo de Stacking tiene un ajuste casi perfecto a los datos y es altamente preciso en la predicción de las calificaciones de los libros en la plataforma Goodreads.

## Interpretación

El modelo de Stacking, que combina los resultados de varios modelos de regresión, demuestra ser el más efectivo para predecir las calificaciones de libros en la plataforma Goodreads. Su RMSE cercano a cero y su R^2 cercano a uno indican que es altamente preciso y puede explicar la variabilidad en las calificaciones de los libros de manera excepcional. 

## Conclusiones

La implementación del modelo de Stacking es fundamental para mejorar las métricas de predicción de la calificación de los libros en Goodreads. Esto proporciona a la editorial Pluma una herramienta poderosa para evaluar el potencial de éxito de los libros antes de su publicación.

El uso de modelos de machine learning, especialmente el modelo de Stacking, puede ayudar a las editoriales a tomar decisiones informadas sobre qué libros publicar, cuándo hacerlo y qué características deben tener para maximizar su popularidad en Goodreads y, en última instancia, en el mercado en general.

La capacidad del modelo de Stacking para predecir con precisión las calificaciones de los libros sugiere que las editoriales pueden optimizar sus estrategias de publicación y marketing en función de estas predicciones, lo que podría llevar a un aumento en las ventas y la visibilidad de los libros.

```{Note}
En resumen, el modelo de Stacking es una herramienta valiosa para las editoriales que desean evaluar y maximizar el potencial de éxito de sus libros en la plataforma Goodreads, lo que puede tener un impacto positivo en su desempeño en el mercado editorial.
```

## Limitaciones

Los resultados se basan en datos hasta el año 2020 y pueden no ser aplicables a futuros cambios en el comportamiento de los usuarios o en la plataforma Goodreads.
Los resultados se centran en las calificaciones de libros en Goodreads y no garantizan el éxito en el mercado en general. Otros factores, como la promoción y la calidad de la obra, también son importantes.


## Futuras líneas de investigación

Al haber realizado este análisis, encontramos también otras oportunidades de investigación que pueden llevarse a cabo. Entre estas, realizar *web scrapping* de las reseñas escritas y a partir de ellas, llevar a cabo un análisis de sentimientos para clasificar los mejores libros reseñados; también, agregar la columna de géneros literarios y construir un sistema clasificación de libros por autor, que serviría para identificar el estilo y temática propia de cada escritor.

Esto ayudaría a nuestro cliente, la Editorial Pluma, a entender la dinámica del mercado y tener un panorama más amplio sobre los autores y la forma en la que los usuarios interactúan en estas plataformas, para así crear estrategias de mercadeo acordes con su propósito como editorial y lograr posicionarse en el mercado.