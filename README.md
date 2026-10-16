# Simulador · Mejores de Carrera 2026

Simulador de la prueba de conocimientos del concurso «Mejores Empleados y Empleadas de Carrera Administrativa 2026» de la Personería de Bogotá.

- 271 preguntas sobre los 20 temas del Anexo Técnico, cada una etiquetada con su tema.
- Series de estudio de máximo 20 preguntas, por tema o por aspecto (institucional, función pública, derechos humanos).
- Diagnóstico acumulado que señala qué temas reforzar, y biblioteca de documentos y enlaces por tema.
- Metodología Tipo I (única respuesta), Tipo II (opciones combinadas) y Tipo III (afirmación–razón).
- Tres simulacros fijos de 50 preguntas (cuadernillos A, B y C, sin preguntas repetidas entre ellos), un simulacro aleatorio, práctica por tema y repaso de preguntas falladas.
- Acta de calificación con puntaje sobre 100, umbral de 70 puntos y desempeño por tema y por tipo.
- Funciona en celular y computador, con modo claro y oscuro. El progreso se guarda en el navegador.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo, `simulador-mejores-2026`).
2. Sube el archivo `index.html` (y este `README.md`) a la raíz del repositorio.
3. Ve a **Settings → Pages**, en *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
4. En uno o dos minutos la página quedará en `https://TU-USUARIO.github.io/simulador-mejores-2026/`.

## Agregar preguntas

Las preguntas están dentro de `index.html`, en los arreglos `Q1` a `Q5`. Formato:

```js
// Tipo I: la opción correcta va PRIMERO (la app baraja el orden)
{tm:"T9",t:1,q:"Enunciado",o:["Correcta","Distractor","Distractor","Distractor"],e:"Justificación",f:"Fuente"}
// Tipo II: a = 0:A(1,2,3) · 1:B(1,3) · 2:C(2,4) · 3:D(solo 4)
{tm:"T9",t:2,q:"Enunciado",s:["Afirmación 1","Afirmación 2","Afirmación 3","Afirmación 4"],a:1,e:"...",f:"..."}
// Tipo III: a = 0:A(V,V,explica) · 1:B(V,V,no explica) · 2:C(V,F) · 3:D(F,V)
{tm:"T9",t:3,af:"Afirmación",rz:"Razón",a:0,e:"...",f:"..."}
```

Los códigos de tema van de `T1` a `T20` y están listados en la constante `TEMAS`.

## Aviso

Herramienta de estudio personal; no es material oficial de la Personería de Bogotá ni de la Universidad Distrital. Verifica la normativa vigente antes de la prueba.
