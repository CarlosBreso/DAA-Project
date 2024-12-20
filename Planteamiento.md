### Movilidad Urbana Multimodal

Se quiere extender el uso de una aplicación de transporte urbano. Esta aplicación no solo muestra las rutas de autobuses, metros y otros medios de transporte, sino que también sugiere al usuario la mejor combinación de transportes (a pie, metro, autobús, taxi callejero, bicicletas compartidas) que en el menor tiempo posible lo lleven a su destino según el presupuesto y preferencias del viajante. Para lograr esto, se deben considerar las siguientes variables adicionales:

- Horarios y Frecuencias: Horarios de salida y llegada de autobuses, metros y otros transportes.

- Costo monetario:  Posibilidad de que exista un presupuesto no superable por la ruta recomendada. Tener en cuenta Tarifas de cada medio de transporte y tarifas dinámicas en taxis callejeros o vehículos privados (uber).

- Distancias y Velocidades: Velocidades promedio para cada medio de transporte, que pueden variar según la hora del día, las condiciones de tráfico y del clima.

- Preferencias en términos de costos vs. tiempo (algunos usuarios pueden preferir opciones más económicas, aunque tomen más tiempo).

- Preferencias sobre la comodidad (preferencia por menos transbordos, preferencias por transporte con aire acondicionado, etc.).

- Puntos de Interés y Paradas: Paradas intermedias que el usuario quiera incluir en su ruta.

- Cantidad de Personas Viajando Juntas: Disponibilidad de espacio en vehículos para grupos grandes. Preferencias sobre mantenerse juntos durante todo el viaje.


### Solución

El desarrollo de un sistema que integre estas variables puede lograrse mediante la utilización de una combinación de datos históricos y en tiempo real. Inicialmente, se propone emplear el algoritmo A* para determinar la ruta de menor costo. No obstante, esta aproximación requiere la definición de diversas heurísticas en caso de que existan múltiples funciones de costo, derivadas de las preferencias del usuario. El aspecto de mayor relevancia radica en la modelación y en el análisis de la complejidad del problema, dependiendo de las variables adicionales que se decidan incluir.