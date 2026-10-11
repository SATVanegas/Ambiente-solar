# Módulos en fase posterior

Estos tres módulos salieron de la propuesta de octubre de 2026 y quedan anotados para una fase posterior. Si se retoman, se cotizan aparte.

Los códigos de esta tabla son los que tenían en la propuesta original. Después de sacarlos, la propuesta se renumeró para que no quedaran saltos, así que en la versión actual M8 y M9 son otros módulos (ver el final de este archivo). Si se retoman, se les asigna un código nuevo a partir de M10.

| Código original | Módulo | Plan original |
|---|---|---|
| M8 | Gestión humana | Meses 7–8 |
| M10 | Operación y monitoreo | Ya era fase posterior |
| M11 | Comercial y CRM | Meses 5–6 |

---

## Gestión humana (antes M8)

**Para qué:** las horas de campo llegan solas a nómina, sin llamar a cada ingeniero antes de liquidar.

**Quién lo usa:** gestión humana, ingenieros a cargo de cuadrillas y contabilidad.

**Funciones**

- Tiempo y nómina
  - Registro diario de jornada y horas extras desde la app de campo, aprobado por el ingeniero a cargo.
  - Consolidado listo para nómina, exportable en el formato que use la empresa. La integración directa depende de que el proveedor de nómina lo permita.
  - Asignación de personal a proyectos con el costo de mano de obra cargado al centro de costos.
- Ciclo del empleado
  - Retiro con checklist: devolución de equipos, reasignación de pendientes y accesos, y anticipos abiertos.
  - Hojas de vida y certificaciones compartidas con SST.
- Obligaciones
  - Control de cuotas SENA, personal con estabilidad laboral reforzada y documentos de teletrabajo exigidos por la ARL.

**Vistas:** planilla de horas (por periodo, trabajador y proyecto), asignación (quién está en qué obra y desde cuándo), prenómina (consolidado listo para liquidar) y checklist de retiro (pendientes antes del paz y salvo).

**Alertas:** horas sin aprobar al cierre del periodo; retiro con equipos o anticipos pendientes; obligaciones legales próximas a vencer.

---

## Operación y monitoreo (antes M10)

**Para qué:** el sistema operativo de las plantas en operación. Se construye cuando haya granjas operando y hardware definido.

**Quién lo usa:** operación y mantenimiento, gerencia e inversionistas.

**Funciones**

- Captura y alertas
  - Inversores por Modbus, estación meteorológica, termografía y medidores de frontera, en una base de datos propia.
  - Rendimiento esperado vs real por inversor y planta, caídas de equipos y verificación diaria del reporte a XM/ASIC.
- Mantenimiento y analítica
  - Plan preventivo, órdenes correctivas y costeo de cada visita.
  - Patrones de falla por equipo y antigüedad, y mantenimiento predictivo.

**Vistas:** mapa de plantas (estado en vivo de cada granja), rendimiento (esperado vs real por inversor) y órdenes de trabajo (preventivas y correctivas por planta).

**Alertas:** planta, inversor o telemetría caídos; día sin reporte de frontera.

**Insumo que se pedía:** acceso a los datos de una planta en operación.

---

## Comercial y CRM (antes M11)

**Para qué:** conecta la venta con el proyecto desde la primera visita y concentra los contactos que llegan por la web y la calculadora solar.

**Quién lo usa:** comercial y gerencia.

**Funciones**

- Entrada de leads
  - Registro de los contactos que llegan por la web y la calculadora solar, con su prediseño cuando aplica.
  - Asignación del lead a un comercial con fecha de próximo contacto.
- CRM liviano
  - Oportunidades con etapas, valor estimado, probabilidad y próxima acción.
  - Centro de costos desde la primera visita para cargar gastos comerciales al futuro proyecto.
  - Conversión de oportunidad ganada a proyecto con un clic, con sus datos ya cargados.
  - Integración o reemplazo del CRM actual, según se defina.

**Vistas:** embudo comercial (oportunidades por etapa y valor), ficha de oportunidad (historial de contactos, visitas y cotizaciones) y bandeja de leads (contactos nuevos por canal).

**Alertas:** lead sin contactar; oportunidad sin próxima acción definida.

**Nota:** el servicio opcional "Crecimiento comercial" (bot de licitaciones, web y estrategia digital) sigue en la propuesta; no depende de este módulo.

---

## Qué cambió en la propuesta al sacarlos

- El catálogo pasó de 13 a 10 módulos y se renumeró sin saltos, de M0 a M9:
  - M0 a M7 conservan su código.
  - Tablero gerencial y agente: era M9, ahora es M8.
  - Legal y cumplimiento contractual: era M12, ahora es M9.
- Se quitó la etapa "Operación" del recorrido por etapas, porque solo la cubría Operación y monitoreo.
- Cronograma: se quitaron las barras de los tres módulos. Las entregas de los meses 5, 6 y 7 ya no mencionan comercial, CRM ni gestión humana.
- Preguntas frecuentes: ya no se menciona la integración con nómina, y se quitó la línea de Operación y monitoreo en "Qué queda fuera".
- Insumos solicitados: ya no se pide el CRM ni el software de nómina actuales, ni el acceso a los datos de una planta en operación.
- **No se cambiaron los precios:** siguen siendo $90.000.000 de desarrollo y $3.200.000 al mes de soporte.
- **El mockup (`centro-de-control.html`) no se tocó.** Todavía muestra las páginas de Operación, Gestión humana y Comercial (con prospectos), y el login dice "13 módulos".
