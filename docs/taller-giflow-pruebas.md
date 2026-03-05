# Documento de Pruebas

## 1. Descripcion del Sistema

## 2. Requerimientos a Evaluar

## 3. Tecnicas de Prueba Aplicadas

RF-03: Inscripcion a evento
Tabla de Decisiones
Seleccionamos esta debido a que hay varias condiciones que afectan a la inscripcion del evento

## 4. Casos de Prueba Diseñados
| Esta registrado | Hay Cupos disponibles | Está previamente inscrito | Resultado    |
|-----------------|-----------------------|---------------------------|--------------|
| Si              | Si                    | No                        | Permitido    |
| No              | Si                    | No                        | No Permitido |
| Si              | No                    | No                        | No Permitido |
| No              | No                    | No                        | No Permitido |
| Si              | Si                    | Si                        | No Permitido |

## 5. Trazabilidad

## 6. Gestion de Versiones (GitFlow)
