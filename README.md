# Llenado Master ISN

Página web para llenar el **Master ISN** con los acumulados de nómina por empresa y estado.

**Usar:** https://betancourtjair.github.io/llenado-master-isn/

## Cómo se usa

1. Carga el Master ISN vacío (.xlsx).
2. Carga el ZIP con los acumulados (.XLS), uno por empresa y estado (por ejemplo `ACUM_09 Septiembre_CHO_CDMX_prov.XLS`).
3. Revisa la tabla: cada archivo se asigna a su pestaña por el nombre; puedes cambiarla a mano.
4. Genera y descarga el Master lleno.

## Qué hace

- Copia solo las columnas cuyo encabezado coincide entre el acumulado y la pestaña (Clave Empleado, Nom Empleado y conceptos como 1-002 SALARIO o 4-408 PROVISION ISN). Nunca escribe sobre una celda con fórmula.
- Si hay más empleados que filas, inserta filas con las mismas fórmulas; si hay menos, quita las sobrantes. La fila **Total** siempre se conserva y sus rangos se ajustan.
- Las pestañas **Empleados**, **Exento-Grav** y **OC** no se modifican.
- Valida que la suma de cada concepto coincida con el Total del acumulado.
- Todo se procesa en el navegador; los archivos no se suben a ningún servidor.

Creado por Jair Betancourt
