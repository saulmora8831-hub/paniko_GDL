# Documentación de Casos de Prueba - Proyecto Paniko

A continuación se enlistan los casos de prueba unitarios, de integración y de aceptación desarrollados para validar los flujos críticos del sistema (Must y Should).

## 1. Casos de Prueba Unitarios (Tests Unitarios)
* **Ubicación en el repositorio:** `/tests/unit/`
* **CP-U01: Validación del Motor de Escalado de Recetas**
  * **Descripción:** Comprueba que al modificar la cantidad de piezas deseadas (ej. de 100 a 350 piezas), los ingredientes se multipliquen de manera proporcional sin errores de redondeo.
  * **Estado:** Aprobado / Implementado.
* **CP-U02: Cálculo Unitario de Costos por Insumo**
  * **Descripción:** Verifica que el sistema derive correctamente el costo por kilogramo basándose en el precio de compra del bulto o empaque.

## 2. Casos de Prueba de Integración
* **Ubicación en el repositorio:** `/tests/integration/`
* **CP-I01: Conexión y Descuento de Inventario por Lote**
  * **Descripción:** Valida que al abrir un nuevo lote de producción (`LOTE-2026-0042`), el sistema se comunique con la base de datos MySQL para descontar de forma automática los insumos requeridos del stock disponible.
  * **Estado:** Aprobado.
* **CP-I02: Autenticación JWT y Restricción de Roles**
  * **Descripción:** Comprueba que un usuario con rol de operario no pueda acceder a los módulos administrativos (Dueño/Supervisor).

## 3. Casos de Prueba de Aceptación (User Acceptance Testing - UAT)
* **Ubicación en el repositorio:** `/tests/acceptance/`
* **CP-A01: Cierre de Lote y Registro Formal de Mermas**
  * **Descripción:** Simula el cierre de un lote de producción ingresando piezas terminadas y el registro de mermas en masa (kg), validando que el panel financiero refleje el impacto monetario.
  * **Estado:** Validado por el Product Owner.
