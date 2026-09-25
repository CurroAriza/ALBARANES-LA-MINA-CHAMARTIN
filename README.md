# Albaranes La Mina de Chamartín 2, S.L.

Control mensual de albaranes de proveedores (CIF B75506477). Cada mes se generan 4 Excel con el mismo formato que La Mina de Velázquez.

## Estructura

```
2026/
  3t/JULIO/ALBARANES/     4 Excel de julio
  3t/AGOSTO/ALBARANES/    4 Excel de agosto
  COMPARATIVO PRECIOS 2026 LA MINA CHAMARTIN.xlsx    comparativo anual (solo productos que suben)
  formato-anterior/       versiones antiguas con el formato de Adri (se conservan)
```

## Los 4 Excel de cada mes

| Archivo | Qué contiene |
|---|---|
| `ALBARANES <MES> LA MINA CHAMARTIN 2026 vN.xlsx` | RESUMEN (KPIs, bases por tipo de IVA, compras por proveedor comparadas con el mes anterior con datos), TOTAL del mes (proveedor, albarán, base, IVA, total), CUADRE ALBARANES (líneas de producto vs albaranes vs TOTAL, OK/REVISAR con tolerancia de 0,05 €) y una hoja por proveedor con un bloque por mes |
| `COMPARATIVA PRECIOS LA MINA CHAMARTIN <MES> 2026.xlsx` | Últimos 3 meses con datos: qué productos suben, bajan, se mantienen o son nuevos, con observaciones (los frescos fluctúan) |
| `INCIDENCIAS LA MINA DE CHAMARTIN <MES> 2026.xlsx` | Incidencias con prioridad (ALTA/MEDIA/BAJA/INFO), acción sugerida y estado (PENDIENTE/REVISADO/CORREGIDO). Arrastra lo pendiente de meses anteriores |
| `CONTROL PDF LA MINA CHAMARTIN <MES> 2026.xlsx` | Control página a página de los PDF escaneados: qué albarán es cada página y si está en el Excel |

## Estado

### Julio 2026 — `ALBARANES JULIO LA MINA CHAMARTIN 2026 v4.xlsx`
- Base 63.628,05 € · 271 líneas · 37 proveedores. Se compara con mayo (junio no tiene datos de Chamartín).
- Control: 168 páginas revisadas en 4 PDF. 139 albaranes de Chamartín, todos en el Excel. 28 no incluidos por ser de otro cliente (27 de Velázquez y 1 de ANGOMI) y 3 pendientes de revisar.
- 127 líneas (36.340,97 €) venían del Excel de Adri y no tienen PDF en la carpeta (hoja SIN PDF).
- Comparativa (abril · mayo · julio): 18 productos suben y 13 bajan. Incidencias: 21.

### Agosto 2026 — `ALBARANES AGOSTO LA MINA CHAMARTIN 2026 v2.xlsx`
- Base 24.271,19 € · 131 líneas · 29 proveedores.
- Control: 120 páginas, 120 albaranes, todos en el Excel (35 con alguna incidencia).
- Cuadre: 3 a revisar — Pescarum agosto (70 €), Peñalastallas julio (67,29 €) y Carnicas Meat julio (0,06 €).
- Comparativa (mayo · julio · agosto): 10 productos suben y 3 bajan. Incidencias: 38.

## Procedimiento mensual

1. Los PDF escaneados se dejan en la carpeta `ALBARANES` del mes; una vez metidos en el Excel, el PDF completo pasa a `ALBARANES/procesados`.
2. Los albaranes de La Mina de Velázquez, de ANGOMI o dudosos se separan en un PDF aparte que se queda en `ALBARANES` y se anotan en incidencias como NO INCLUIDO.
3. Cada tanda nueva de albaranes genera una versión nueva del Excel (v2, v3, v4…); no se borra nada.

## Nombres de proveedor

Unificados con La Mina de Velázquez, comprobados en los propios albaranes: PATATAS YAGO (I Love Potato S.L.), CONS. SELEC. SANTO (Conservas Selección Santoñesa, marca Don Bocarte), ESCRIBANO SANZ (El Escribano), CONS. Y SAL. JIMENEZ (Jiménez Torres), DIST. TENA MTNEZ (Distribuciones Tena Martínez), EIF DISTRIBUCIONES, COCACOLA y TOMATERIA DE CEA.
