
# Integrantes
- Javier Chen 22153
- Gustavo Cruz 22779
---
## Preguntas

1. ¿Existen cambios de arquitectura en las 2 redes implementadas?
  - Sí, para el modelo en numpy usamos 2 neuronas de entrada, 3 ocultas y una de salida, y en pytorch usamos 2 de entrada, 16 ocultas y una salida.
2. ¿Exiten diferencias en la velocidad de convergencia entre las 2 redes?
  - Sí, la red de pytorch es más rápida, y puede deberse a la diferencia de arquitectura anteriormente mencionada, además que implementa un optimizador de Adam y se ve en la gráfica de pytorch que la curva es más suave que la de numpy y alcanza un nivel de error cercano a 0 con menos pasos de tiempo que numpy.
3. En la función init_parameters, ¿qué sucede si inicializamos los pesos en 0 en
lugar de valores aleatorios? ¿y los bias?
  - Todos los nodos de una capa van a hacer el mismo cálculo de propagación y van a recibir el mismo gradiente y no van a aprender nada útil. Por el contrario, el bias inicializado en 0, no afectará al aprendizaje, por que no están conectados entre sí, y cada neurona al final aprenderá algo diferente. Lo único es que al principio las neuronas no van a tener su "opinion" pero con cada iteración se va a ir corrigiendo.



