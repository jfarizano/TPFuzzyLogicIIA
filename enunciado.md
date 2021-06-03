TP Fuzzy Logic - Introducción a la Inteligencia Artificial 

# Enunciado

- Variables de entrada
  - Edad actual {niño, joven, adulto, persona mayor} (0, 15) (14, 24) (18, 65) (60, +)
  - Nivel de estrés {bajo, mediano, alto}
  - Nivel de actividad física {bajo, mediano, alto}
  - Nivel de salud {muy saludable, saludable, poco enfermo, enfermo}

- Variables de salida
  - Esperanza de vida {pobre, baja, media, alta}
  (0, 20), (18, 50), (45, 70), (65, +)

Reglas:

-- Si edad es persona mayor entonces esperanza de vida es alta
----------------
-- Si edad es niño, nivel de salud es saludable o muy saludable, entonces esperanza es alta
-- Si edad es niño, nivel de salud es poco enfermo, entonces esperanza es media
-- Si edad es niño, nivel de salud es enfermo, entonces esperanza es pobre
----------------
-- Si edad es adulto, nivel de estres es bajo o mediano y nivel actividad fisica no es bajo y nivel de salud no es enfermo, entonces esperanza es alta
-- Si edad es adulto, nivel de estres es no bajo y nivel actividad fisica es bajo o mediano y nivel de salud es enfermo o poco enfermo, entonces esperanza es media
--Si edad es adulto, nivel de estres es alto, nivel de actividad fisica es bajo, y nivel de salud es enfermo o poco enfermo, entonces esperanza es baja
----------------
-- Si edad es joven, nivel de estres es cualquiera, nivel activida fisica es cualquiera y nivel de salud es muy saludable o saludable, entonces esperanza es alta
-- Si edad es joven, nivel de estres es no alto, nivel actividad fisica es no alto y nivel de salud es no enfermo, entonces esperanza es media
-- Si edad es joven, nivel de estres es mediano, nivel activida fisica es no alto y nivel de salud es enfermo o poco enfermo, entonces esperanza es baja
-- Si edad es joven, nivel de estres es alto, nivel actividad fisica es bajo, nivel de salud es enfermo, entonces esperanza es pobre