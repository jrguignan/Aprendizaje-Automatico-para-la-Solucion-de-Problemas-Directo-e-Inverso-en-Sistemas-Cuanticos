# Aprendizaje automático para la solución de problemas directo e inverso en sistemas cuánticos

<p align="center">
<img src="images/banner.jpg"  height=300>
</p>

# Índice

* [Objetivos del TEG](#Objetivos-del-TEG)
* [Resumen](#Resumen)
* [Justificación del proyecto](#Justificación-del-proyecto)
* [Palabras claves](#Palabras-claves)
* [Referencias bibliográficas](#Referencias-bibliográficas)
* [Autor](#Autor)

<br>[Volver al Índice](#Índice)

---

## Objetivos del TEG

**Objetivo principal:**  
Resolver el problema directo y un problema inverso en el caso de la ecuación de Schrödinger para sistemas cuánticos simples.

**Objetivos específicos:**
1. Obtener soluciones aproximadas de la densidad de probabilidad electrónica para el átomo de Helio usando el Método de Perturbaciones y el Método del Funcional de Densidad (DFT).
2. Resolver el problema directo usando aproximaciones con kernel.
3. Resolver el problema inverso de determinación del potencial a partir de la distribución de densidad de probabilidad electrónica para el átomo de Hidrógeno usando métodos de kernel.
4. Explorar estrategias similares a las usadas anteriormente para el caso del átomo de Helio.

[Volver al Índice](#Índice)

---

## Resumen

El problema inverso de obtener el potencial a partir de la distribución de densidad de probabilidad electrónica ρ(r₁, r₂) es fundamental en la mecánica cuántica y en la química computacional. Este problema es la base teórica de la **Teoría del Funcional de la Densidad (DFT, por sus siglas en inglés)**.

Según el **primer teorema de Hohenberg-Kohn**: para un sistema de partículas interactuantes en un potencial externo, el potencial externo (y, por lo tanto, el Hamiltoniano y todas las propiedades del sistema en el estado fundamental) está unívocamente determinado (salvo por una constante aditiva) por la densidad de probabilidad del estado fundamental.

En otras palabras, la densidad electrónica del estado fundamental ρ(r) para un sistema de N electrones contiene toda la información sobre el sistema. Esto es revolucionario porque la densidad es una función de solo 3 coordenadas espaciales, mientras que la función de onda de N electrones es una función de 3N coordenadas. Reducir la complejidad de 3N a 3 es un avance computacional y conceptual enorme.

El teorema garantiza que, en principio, existe una correspondencia uno a uno entre el potencial externo y la densidad del estado fundamental, permitiendo reformular el problema de muchos cuerpos en términos de la densidad. Sin embargo, no proporciona un método explícito para invertir la relación, es decir, para calcular el potencial externo Vₑₓₜ(r) a partir de una ρ(r) dada. Este es el núcleo del *problema inverso* en DFT.

Aunque la existencia de la correspondencia está garantizada, su obtención práctica sigue siendo un desafío. En este contexto, el **aprendizaje automático**, en particular las **redes neuronales** y los **métodos de kernel**, han mostrado un gran potencial para modelar relaciones no lineales complejas en espacios de alta dimensionalidad.

Este proyecto propone explorar el uso de métodos de kernel para abordar este problema inverso.

[Volver al Índice](#Índice)

---

## Justificación del proyecto

El proyecto plantea resolver el problema inverso de encontrar el potencial a partir de la densidad electrónica para los átomos de Hidrógeno y Helio utilizando **aprendizaje automático (ML)**. Este enfoque está respaldado por razones clave:

- Representa un paso innovador en la intersección de la mecánica cuántica computacional y la inteligencia artificial.
- Propone soluciones a desafíos que los métodos tradicionales no han resuelto de manera óptima.
- Sus implicaciones prácticas incluyen avances en el diseño de materiales con propiedades específicas (*materiales a la carta*), ingeniería molecular y desarrollo de fármacos.

[Volver al Índice](#Índice)

---

## Palabras claves

Problemas directo e inverso, DFT, Métodos de kernel.

[Volver al Índice](#Índice)

---

## Referencias bibliográficas

1. Parr, R. G., & Yang, W. *Density-Functional Theory of Atoms and Molecules*. Oxford University Press (1989).  
2. Ghosh, S. K., & Parr, R. G. *The Density-Potential Relationship in Density Functional Theory*. The Journal of Chemical Physics, 84(6), 3352–3356, (1986).  
3. Jensen, D. S., & Wasserman, A. *Numerical methods for the inverse problem of density functional theory*. International Journal of Quantum Chemistry, 118(1), e25425, (2018). [https://doi.org/10.1002/qua.25425](https://doi.org/10.1002/qua.25425)
4. Martinetto, V., Shah, K., Cangi, A., & Pribram-Jones, A. *Inverting the Kohn–Sham equations with physics-informed machine learning*. Machine Learning: Science and Technology, 5(1), 015050, (2024). [https://doi:10.1088/2632-2153/ad3159](https://doi:10.1088/2632-2153/ad3159)  
5. Huang, C., Johnson, E. R., Sun, J., & Perdew, J. P. *Exchange-correlation potential built on the derivative discontinuity of electron density*. Nature Communications, 10(1), 4467, (2019). [https://doi.org/10.1038/s41467-019-12467-0](https://doi.org/10.1038/s41467-019-12467-0)  
6. García, P. *Modeling systems with machine learning based differential equations*. Chaos, Solitons & Fractals, 165(Part 2), (2022). [https://doi.org/10.1016/j.chaos.2022.112872](https://doi.org/10.1016/j.chaos.2022.112872)

[Volver al Índice](#Índice)

---




# Autor
José R. Guignan
- Mail: joserguignan@gmail.com
- Linkedin: [https://www.linkedin.com/in/jrguignan/](https://www.linkedin.com/in/jrguignan)
- Portafolio: [https://jrguignan.github.io/](https://jrguignan.github.io/)