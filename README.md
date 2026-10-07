# Albaranes La Mina de Chamartín 2, S.L.

Control mensual de albaranes de proveedores (CIF B75506477). Cada mes se generan 4 Excel con el mismo formato que La Mina de Velázquez.

## Estructura

```
2026/
  3t/JULIO/ALBARANES/     4 Excel de julio
  3t/AGOSTO/ALBARANES/    4 Excel de agosto
  3t/SEPTIEMBRE/ALBARANES/  4 Excel de septiembre
  COMPARATIVO PRECIOS 2026 LA MINA CHAMARTIN.xlsx    comparativo anual (solo productos que suben)
  formato-anterior/       versiones antiguas con el formato de Adri (se conservan)
index.html                web "Compras y precios" (la misma que la de La Mina de Velázquez, con los datos de Chamartín)
```

## Web

**https://curroariza.github.io/ALBARANES-LA-MINA-CHAMARTIN/** — publicada con GitHub Pages desde `index.html`. Es una página privada de los socios: pide contraseña al entrar (el contenido va cifrado en el propio archivo) y recuerda el dispositivo. Una página única que se abre en cualquier navegador: resumen del mes, precios que suben y bajan, precios iguales, productos que ya no se compran, total por proveedor e incidencias (con filtro por departamento: Gonzalos, Marcos / Financiero, Administración WIT y sin asignar), con selector de mes (julio, agosto y septiembre de 2026). Precios netos; si un producto tiene varios precios en el mes se toma el más alto.

## Los 4 Excel de cada mes

| Archivo | Qué contiene |
|---|---|
| `ALBARANES <MES> LA MINA CHAMARTIN 2026 vN.xlsx` | RESUMEN (KPIs, bases por tipo de IVA, compras por proveedor comparadas con el mes anterior con datos), TOTAL del mes (proveedor, albarán, base, IVA, total), CUADRE ALBARANES (líneas de producto vs albaranes vs TOTAL, OK/REVISAR con tolerancia de 0,05 €) y una hoja por proveedor con un bloque por mes |
| `COMPARATIVA PRECIOS LA MINA CHAMARTIN <MES> 2026.xlsx` | Últimos 3 meses con datos: qué productos suben, bajan, se mantienen o son nuevos, con observaciones (los frescos fluctúan) |
| `INCIDENCIAS LA MINA DE CHAMARTIN <MES> 2026.xlsx` | Incidencias con prioridad (ALTA/MEDIA/BAJA/INFO), acción sugerida, estado (PENDIENTE/REVISADO/CORREGIDO), lo que decide la asesoría (ACCION), el DEPARTAMENTO que se encarga y el RESULTADO. Arrastra lo pendiente de meses anteriores |
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

### Septiembre 2026 — `ALBARANES SEPTIEMBRE LA MINA CHAMARTIN 2026 v2.xlsx`
- Base 73.621,92 € · total con IVA 82.901,46 € · 308 albaranes (344 líneas) · 41 proveedores, 10 de ellos nuevos.
- v2 (07/10/2026), tras la revisión de incidencias de la asesoría: detalle línea a línea de los tres tickets de Voldis que no se leían (reescaneados; las bases no cambian), ticket de Hielos Angel Ice del 29/08 (50,00 €) y las dos cargas de tanque de Mahou con **importe estimado** a 4,00 €/l (7.740,00 € de base) hasta que llegue la factura. La `v1` (65.831,92 €) se conserva.
- Control: 303 páginas revisadas en 8 PDF (2 son reescaneos). 308 albaranes de Chamartín en el Excel; 1 de Velázquez y 4 documentos no incluidos (dos hojas de pedido, una factura y una muestra). Dos albaranes tapados por otro en el escaneo están solo por el importe.
- Cuadre: los 41 de septiembre dan OK; siguen los 3 de julio y agosto.
- Comparativa (julio · agosto · septiembre): 15 productos suben y 7 bajan.
- Incidencias: 32 pendientes de 48; 16 cerradas el 07/10/2026. Cada pendiente lleva su departamento (Gonzalos 7, Marcos / Financiero 2, Administración WIT 2, sin asignar 21). Numeración estable: las de septiembre van de la 39 a la 68.

## Procedimiento mensual

1. Los PDF escaneados se dejan en la carpeta `ALBARANES` del mes; una vez metidos en el Excel, el PDF completo pasa a `ALBARANES/procesados`.
2. Los albaranes de La Mina de Velázquez, de ANGOMI o dudosos se separan en un PDF aparte que se queda en `ALBARANES` y se anotan en incidencias como NO INCLUIDO.
3. Cada tanda nueva de albaranes genera una versión nueva del Excel (v2, v3, v4…); no se borra nada.

## Nombres de proveedor

Unificados con La Mina de Velázquez, comprobados en los propios albaranes: PATATAS YAGO (I Love Potato S.L.), CONS. SELEC. SANTO (Conservas Selección Santoñesa, marca Don Bocarte), ESCRIBANO SANZ (El Escribano), CONS. Y SAL. JIMENEZ (Jiménez Torres), DIST. TENA MTNEZ (Distribuciones Tena Martínez), EIF DISTRIBUCIONES, COCACOLA y TOMATERIA DE CEA.
