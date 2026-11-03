# Registros de Decisiones Arquitectónicas (ADRs) - Paniko

## ADR 01: Selección de MySQL como Base de Datos Relacional
* **Estado:** Aprobado y Adoptado.
* **Contexto:** El proyecto requiere una trazabilidad estricta y relaciones estrictas entre fichas técnicas, insumos, lotes de producción y mermas.
* **Decisión:** Utilizar MySQL como motor de base de datos relacional debido a su solidez en la integridad referencial y su compatibilidad con Node.js.
* **Consecuencias:** Facilita las consultas complejas de costos e inventario en tiempo real.

## ADR 02: Elección de Vercel para el Despliegue del Frontend
* **Estado:** Aprobado.
* **Contexto:** Necesitamos un entorno web público y accesible con despliegues continuos rápidos para las revisiones e hitos evaluativos.
* **Decisión:** Desplegar la aplicación en la plataforma Vercel.
* **Consecuencias:** Integración fluida con el repositorio de GitHub y despliegue automatizado ante cada Pull Request.
