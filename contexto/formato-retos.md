# Formato de los retos

Este documento define la estructura común que deben seguir todos los retos de Daily Logic.

El objetivo es que cualquier reto pueda ser creado, leído y resuelto de forma consistente, independientemente de quién lo haya creado.

## Formato

Todos los retos deben estar escritos en Markdown.

Cada reto debe existir en su propia carpeta:

```text
retos/
└── 001/
    └── README.md
```

El archivo del reto debe llamarse siempre `README.md`.

---

## Estructura obligatoria

Cada reto debe seguir esta estructura:

```markdown
# Reto 001 — Título

**Categoría:** LOGICA  
**Formato:** PROBLEMA  
**Dificultad:** 1/5  
**Tiempo estimado:** 15 minutos

## Objetivo

Descripción breve de qué habilidad se pretende entrenar.

## Reto

Enunciado completo del problema.

## Condiciones

Restricciones, reglas o información relevante.

## Ejemplos

Ejemplos que ayuden a comprender el problema sin revelar la solución.

## Tu misión

Descripción concreta de lo que debe entregar o resolver el usuario.

<details>
<summary>Pista</summary>

Pista inicial que ayude a desbloquear el problema sin revelar la solución.

</details>
```

---

## Título

El título debe seguir el formato:

```text
# Reto 001 — Nombre del reto
```

El número debe coincidir con el número de la carpeta.

El nombre debe ser breve y descriptivo, pero no debe revelar la estrategia necesaria para resolver el problema.

---

## Metadatos

Cada reto debe incluir:

* Categoría principal.
* Formato.
* Dificultad.
* Tiempo estimado.

Ejemplo:

```markdown
**Categoría:** DEBUGGING  
**Formato:** CONTRAEJEMPLO  
**Dificultad:** 3/5  
**Tiempo estimado:** 20 minutos
```

Si el reto pertenece a varias categorías, se pueden añadir categorías secundarias:

```markdown
**Categoría:** DEBUGGING  
**Categorías secundarias:** CASOS_LIMITE, CONTRAEJEMPLOS
```

---

## Objetivo

Debe explicar qué habilidad se pretende entrenar.

No debe explicar cómo resolver el reto.

Ejemplo:

> Entrenar la capacidad de identificar supuestos incorrectos y encontrar casos límite.

No sería adecuado:

> Aprender a utilizar búsqueda binaria.

El reto debe entrenar una capacidad de razonamiento, no enseñar directamente una técnica concreta.

---

## Reto

Debe contener el enunciado completo y toda la información necesaria para comenzar a trabajar.

El enunciado debe ser autosuficiente.

No se debe asumir que el usuario conoce el contexto de otros retos.

Cuando sea posible, evitar referencias innecesarias a lenguajes de programación concretos.

---

## Condiciones

Las restricciones deben aparecer explícitamente.

Si una condición es importante para la solución, no debe quedar implícita.

Ejemplo:

```markdown
- Los elementos pueden estar repetidos.
- El orden de entrada no está garantizado.
- Puede haber cero elementos.
- La solución debe funcionar para cualquier tamaño de entrada.
```

No se deben añadir restricciones artificiales únicamente para hacer el problema más difícil.

---

## Ejemplos

Los ejemplos sirven para comprender el problema, no para enseñar la solución.

Debe evitarse que los ejemplos sean tan específicos que permitan deducir inmediatamente el algoritmo.

Cuando sea útil, incluir también ejemplos pequeños o casos aparentemente extraños.

---

## Tu misión

Debe indicar exactamente qué debe hacer el usuario.

Puede pedir, por ejemplo:

* encontrar una solución;
* explicar el razonamiento;
* encontrar un bug;
* encontrar un contraejemplo;
* comparar dos alternativas;
* predecir un resultado;
* diseñar una estrategia;
* identificar casos límite;
* justificar por qué una solución funciona.

Cuando el objetivo sea razonar, no exigir código.

---

## Pista inicial

Todos los retos deben incluir al menos una pista.

La pista debe estar oculta utilizando HTML `<details>`.

Ejemplo:

```markdown
<details>
<summary>Pista</summary>

Empieza intentando resolver el problema con el menor número de elementos posible.

</details>
```

La pista debe cumplir las siguientes reglas:

1. No debe revelar la solución.
2. No debe indicar directamente el algoritmo.
3. Debe ayudar a superar un bloqueo inicial.
4. Debe orientar hacia una forma de pensar.
5. Debe ser suficientemente útil para que el usuario pueda continuar.

La pista debe considerarse una ayuda, no parte del enunciado principal.

---

## Pistas adicionales

Cuando un reto sea especialmente complejo, puede incluir varias pistas progresivas.

Ejemplo:

```markdown
<details>
<summary>Pista 1</summary>

...

</details>

<details>
<summary>Pista 2</summary>

...

</details>

<details>
<summary>Pista 3</summary>

...

</details>
```

Las pistas deben aumentar progresivamente el nivel de ayuda.

La primera pista debe ser sutil.

La última puede acercarse más a la estrategia, pero nunca debería sustituir completamente el razonamiento del usuario.

No todos los retos necesitan más de una pista.

---

## Soluciones

El README del reto no debe contener la solución.

La solución puede mantenerse fuera del repositorio público o añadirse posteriormente mediante un mecanismo separado.

El objetivo es que una persona que encuentre el reto pueda resolverlo sin encontrarse accidentalmente con la respuesta.

---

## Código

Los retos no deben requerir código salvo que el propio reto consista en:

* leer código;
* depurar código;
* analizar una implementación;
* revisar código generado por IA;
* comparar implementaciones.

Cuando se incluya código, debe utilizarse únicamente como herramienta para plantear el problema.

El lenguaje de programación no debe ser relevante para resolver el reto salvo que se indique expresamente.

---

## Lenguaje

Los retos se escribirán en castellano.

Se utilizará un lenguaje claro y directo.

Evitar:

* lenguaje excesivamente académico;
* explicaciones innecesariamente largas;
* jerga técnica cuando no sea necesaria;
* pistas que revelen prematuramente la solución.

---

## Estilo

Los retos no deben utilizar emojis.

La estructura visual debe ser limpia y consistente.

Se pueden utilizar:

* títulos Markdown;
* listas;
* tablas;
* bloques de código;
* diagramas ASCII cuando sean útiles;
* elementos `<details>` para ocultar pistas.

No utilizar emojis como parte del sistema de categorías ni como decoración.

---

## Principio fundamental

El formato debe ayudar a presentar el problema sin resolverlo.

Un buen reto debe dejar al usuario pensando:

> "Sé qué tengo que conseguir, pero todavía no sé cómo hacerlo."

Esa incertidumbre es parte del entrenamiento.
