# Sensor de Puerta Compatible NetBotz NBES0303 o NBES0303s

## Descripción

Este documento recopila la información obtenida durante la ingeniería inversa del sensor de puerta utilizado por los equipos APC NetBotz.

El objetivo es comprender completamente su funcionamiento para desarrollar un reemplazo compatible utilizando componentes comerciales.

Actualmente la información presentada corresponde a mediciones realizadas sobre un sensor original.

---

## Estado del proyecto

| Estado              | Descripción                                   |
| ------------------- | --------------------------------------------- |
| ✅ Verificado        | Mediciones realizadas sobre hardware original |
| 🟡 En investigación | Funcionamiento interno del puerto universal   |
| 🔄 Desarrollo       | Diseño del reemplazo DIY                      |

---

# Compatibilidad

Actualmente se está validando con:

* NetBotz 150

Se espera compatibilidad con otros equipos que utilicen el mismo puerto universal de sensores.

---

# Funcionamiento

El sensor está compuesto por:

* Un interruptor magnético (Reed Switch).
* Una resistencia de identificación de **2 kΩ**.
* Una resistencia de **1 kΩ** en serie con el interruptor.

No se encontraron componentes activos.

---

# Pinout RJ45

| Pin | Función                   |
| --- | ------------------------- |
| 1   | Identificación del sensor |
| 2   | Sin conexión              |
| 3   | Identificación del sensor |
| 4   | Sin conexión              |
| 5   | Sin conexión              |
| 6   | Entrada del sensor        |
| 7   | Entrada del sensor        |
| 8   | Sin conexión              |

---

# Esquemático obtenido

```text
             Identificación

Pin 1 o------[2 kΩ]------o Pin 3


                 Sensor

Pin 6 o------[1 kΩ]------o/ o------o Pin 7
                          Reed
```

---

# Mediciones

## Resistencia de identificación

| Entre pines | Valor |
| ----------- | ----: |
| 1 - 3       |  2 kΩ |

---

## Sensor

| Estado         |              Medición |
| -------------- | --------------------: |
| Puerta abierta | Circuito abierto (OL) |
| Puerta cerrada |                  1 kΩ |

---

# Componentes identificados

| Componente                    |                             Valor |
| ----------------------------- | --------------------------------: |
| Resistencia de identificación |                              2 kΩ |
| Resistencia serie             |                              1 kΩ |
| Reed Switch                   | Contacto normalmente abierto (NO) |

---

# Observaciones

* Los pines 2, 4, 5 y 8 no presentan conexión.
* No se observaron circuitos integrados ni componentes activos.
* El sensor es completamente pasivo.
* La resistencia de 2 kΩ probablemente identifica el tipo de sensor ante el NetBotz.
* La resistencia de 1 kΩ podría actuar como limitador de corriente o formar parte del método de detección utilizado por el equipo.

---

# Estado de la información

| Elemento                                  | Estado              |
| ----------------------------------------- | ------------------- |
| Pinout                                    | ✅ Verificado        |
| Valores de resistencias                   | ✅ Verificado        |
| Funcionamiento del reed switch            | ✅ Verificado        |
| Método de detección utilizado por NetBotz | 🟡 En investigación |

---

# Próximos pasos

* Medir tensiones del puerto universal.
* Analizar la corriente de detección.
* Diseñar un PCB compatible.
* Validar un sensor DIY.
* Probar compatibilidad con otros modelos NetBotz.

---

# Historial

| Fecha      | Cambio                                                               |
| ---------- | -------------------------------------------------------------------- |
| 2026-07-15 | Primera documentación basada en mediciones sobre un sensor original. |
