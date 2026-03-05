## Registro de Estudiante (Edad)

El sistema debe permitir el registro de estudiantes cuya edad esté entre **16 y 65 años inclusive**.

**Técnica usada:** Partición de Equivalencia

Considero que es la técnica más adecuada porque ayuda a **reducir la cantidad de casos de prueba necesarios**.

| Variable        | Clases válidas                          | Clases inválidas                                   |
|-----------------|------------------------------------------|----------------------------------------------------|
| Edad del usuario| Cualquier número entre 16 y 65. (19)     | Cualquier número menor a 16 (14)<br>Cualquier número mayor a 60 (75) |
