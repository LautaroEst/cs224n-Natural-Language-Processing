# Notas de la Lecture 1

El curso empieza hablando del significado de las palabras: cómo poder representar con un objeto discreto el significado de las palabras de un idioma y cómo automatizar el hecho de que una palabra tiene un significado.

## One-hot vectors

Primero, se propone representar (a partir de un vocabulario de tamaño finito), las palabras con *one-hot vectors*. El principal problema de esto es que, si cada vector representa un significado, todas las palabras son ortogonales, es decir que no hay significado entre ellas.

## Word embedding

Otra idea que tiene resultados un poco mejores es la que propone definir al significado de las palabras según su contexto. Acá se estaría tendiendo a mostrar ejemplos de uso de la palabra, en realidad. No se está dando una explicación, sino que se está buscando aprenderla a partir de los ejemplos, con lo cual la única forma en que esto funcione bien es dando los ejemplos correctos (o sea, más datos).

Esta representación se llama "distribuída" y a los vectores que reprentan palabras se los llama *word vector*, *word representation* o *word embedding*.


## Word2Vec

La primera aplicación de esto es predecir un contexto (es decir una sucesión de palabras que rodean a otra palabra) a partir de una palabra central. Para eso, propone maximizar el likelihood de todos los contextos vistos para cada palabra.

En el desarrollo de las cuentas (que lo hace con softmax) encuentra interpretaciones de qué significa cada término (VER VIDEO LECTURE 1, MINUTO 1:05). 
