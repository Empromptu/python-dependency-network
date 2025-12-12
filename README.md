📊 Análisis de la Red de Dependencias del Ecosistema Python (2016 vs. 2025)
🎯 Objetivo

Este proyecto analiza cómo evolucionó la red de dependencias de paquetes de Python entre 2016 y 2025. A partir de datos de PyPI y herramientas de teoría de grafos, se estudian los cambios estructurales del ecosistema, las comunidades temáticas y los paquetes más influyentes.

🛠 Metodología

Datos: Se construyeron dos datasets de dependencias (2016 y 2025).

Grafos: Se generaron grafos dirigidos donde los nodos son paquetes y las aristas representan dependencias.

Métricas estructurales: grado, centralidades (closeness, betweenness, PageRank), componentes y conectividad.

Comunidades: Detección con Louvain + análisis temático mediante Wordclouds.

📈 Principales Hallazgos
1. Crecimiento y complejidad

De 26.234 → 295.898 paquetes y

De 72.252 → 1.606.337 dependencias.
El ecosistema es más denso y las librerías modernas dependen de más paquetes.

2. Conectividad estable pero más masiva

Muchos componentes fuertemente conexos pequeños.

Una gran componente débilmente conexa sostiene la red
(25.169 nodos en 2016 → 291.204 en 2025).

3. Cambios en centralidades

Requests sigue siendo clave, pero el núcleo cambió:

↓ Menor centralidad relativa: Django, Six, Distribute.

↑ Mayor influencia: NumPy, Pandas, Pytest, Typing-Extensions, Pydantic.

Se observa una transición hacia ciencia de datos, cómputo científico y testing.

4. Comunidades más mezcladas

La modularidad cae 0.538 → 0.426.

Más aristas ⇒ fronteras entre comunidades menos marcadas.

La comunidad científica pasa a ocupar posiciones más centrales.

Palabras frecuentes cambian de api, django, client a data, api, tool.

📝 Conclusión

El ecosistema Python se volvió más grande, más denso y más interdependiente.
Los paquetes históricos pierden centralidad relativa mientras que la ciencia de datos, las prácticas de testing y el tipado estático redefinen el núcleo del ecosistema.
La estructura global sigue organizada alrededor de una gran componente conectada que integra la mayoría de los paquetes.
