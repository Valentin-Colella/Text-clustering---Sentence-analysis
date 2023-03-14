# Text-clustering---Sentence-analysis


El notebook se utiliza para realizar clustering sobre oraciones y un análisis básico sobre las mismas. Permitiendo probar con diversas técnicas:
1) Primero que nada se realiza una limpieza sobre los textos, se normalizan (se eliminan puntuaciones, se reduce todo a minúsculas), se pueden eliminar stopwords, se puede realizar stemming o lemmatization, reemplazar sinónimos. 
2) Para armar los embeddings de texto se puede usar TFIDF o modelos preentrenados de sentences transformers  (en el notebook hay uno entrenado en español).
3) Para armar los clusters se puede utilizar kmeans con silhouette score (esto último para determinar la cantidad de grupos a formar). UMAP y HDBSCAN, el primero para reducir la dimensionalidad y el segundo para armar los clusters. Para estos dos modelos se utilizan funciones de la librería chatintents que permiten realizar una búsqueda de hiperparámetros. Por último, agglomerative clustering.
4) Una vez que se obtienen los clusters se los puede visualizar, en este caso se reduce la dimensión con PCA (acá también se podrían usar otras técnicas). Se realiza un análisis sobre los mismos, por ejemplo detección de outliers con text similarity, búsqueda de la oración más representativa de cada cluster. Bigramas, unigramas, porcentaje que representan en cada grupo. Búsqueda de verbos, sustantivos. 
