# Documento de Pruebas

## 1. Descripcion del Sistema
1️⃣ Análisis del Enunciado

El requerimiento establece que el código del estudiante debe cumplir las siguientes condiciones:

- Tener exactamente 8 caracteres.
- Iniciar con la letra “E”.
- Los 7 caracteres restantes deben ser numéricos.

Se trata de una validación de formato sobre un campo de texto.

---

## 2. Requerimientos a Evaluar
## 2️⃣ Técnica de Prueba Seleccionada

### Partición de Equivalencia

---


## 3. Tecnicas de Prueba Aplicadas
## 3️⃣ Justificación de la Técnica

Se selecciona Partición de Equivalencia porque el requerimiento define reglas claras que permiten dividir las entradas en clases válidas e inválidas.
Cada clase representa un grupo de valores que deberían comportarse igual.
Esto permite reducir la cantidad de pruebas manteniendo buena cobertura.

---

## 4. Casos de Prueba Diseñados
### Clases de Equivalencia Identificadas

| ID  | Clase                                               | Tipo      |
|-----|----------------------------------------------------|----------|
| CE1 | Código válido (E + 7 números)                      | Válida   |
| CE2 | Longitud menor a 8                                 | Inválida |
| CE3 | Longitud mayor a 8                                 | Inválida |
| CE4 | No inicia con E                                    | Inválida |
| CE5 | Los últimos 7 caracteres no son todos numéricos    | Inválida |

---

### Casos de Prueba

| CP     | Entrada     | Clase cubierta | Resultado Esperado |
|--------|------------|---------------|--------------------|
| CP-01  | E1234567   | CE1           | Código válido |
| CP-02  | E123456    | CE2           | Error: longitud incorrecta |
| CP-03  | E12345678  | CE3           | Error: longitud incorrecta |
| CP-04  | A1234567   | CE4           | Error: debe iniciar con E |
| CP-05  | E1234A67   | CE5           | Error: debe contener solo números después de E |
| CP-06  | E123-567   | CE5           | Error: debe contener solo números después de E |

---
## 5. Trazabilidad
## 5️⃣ Cobertura

- Se cubre la clase válida (CE1).
- Se cubren todas las clases inválidas identificadas (CE2–CE5).
- Se valida cada regla del requerimiento de manera independiente.

Se garantiza cobertura completa del requerimiento RF-02 mediante partición de equivalencia.


## 6. Gestion de Versiones (GitFlow)



