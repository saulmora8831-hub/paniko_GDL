# Registro de Bloqueos, Impedimentos y Deudas Técnicas

## 1. Bloqueos Encontrados y Resueltos
* **Bloqueo 01: Incompatibilidad inicial en conversiones de unidades (Gramos vs. Kilogramos)**
  * *Descripción:* Durante las primeras pruebas de integración, el motor de recetas arrojaba errores al mezclar unidades de gramos con kilogramos.
  * *Solución aplicada:* Se estandarizó una capa intermedia de normalización matemática que convierte todas las unidades a gramos como base interna antes de realizar el cálculo del lote.

## 2. Deudas Técnicas Identificadas
* **Deuda 01: Refactorización de estilos CSS**
  * *Descripción:* Actualmente algunos componentes del panel de control utilizan estilos incrustados o clases repetidas.
  * *Plan de atención:* Planificado para resolverse en el refactor previo a la entrega final (Semana 17).
