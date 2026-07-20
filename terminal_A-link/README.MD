# Terminador A-Link APC

## Descripción

El terminador A-Link es un accesorio pasivo utilizado para finalizar el bus de comunicación A-Link de los dispositivos APC NetBotz. Su propósito es proporcionar la impedancia de terminación necesaria para garantizar la integridad de la señal y evitar reflexiones en el bus.

Durante el proceso de ingeniería inversa no se identificaron componentes activos, únicamente resistencias de terminación.

---

# Hardware

- Conector RJ-45 (8P8C)
- 2 resistencias de 120 Ω
- Sin componentes activos

---

# Pinout

| Pin | Función |
|-----|---------|
| 1 | Resistencia de 120 Ω hacia Pin 2 |
| 2 | Resistencia de 120 Ω hacia Pin 1 |
| 3 | Sin conexión |
| 4 | Sin conexión |
| 5 | Sin conexión |
| 6 | Sin conexión |
| 7 | Resistencia de 120 Ω hacia Pin 8 |
| 8 | Resistencia de 120 Ω hacia Pin 7 |

---

# Esquema obtenido

```
           120 Ω
Pin 1 o---/\/\/\---o Pin 2

Pin 3 o--------------- NC
Pin 4 o--------------- NC
Pin 5 o--------------- NC
Pin 6 o--------------- NC

           120 Ω
Pin 7 o---/\/\/\---o Pin 8
```

---

# Mediciones

Las siguientes mediciones fueron realizadas utilizando un multímetro digital sobre un terminador original APC.

| Medición | Valor |
|----------|------:|
| Pin 1 ↔ Pin 2 | 120 Ω |
| Pin 7 ↔ Pin 8 | 120 Ω |
| Pin 3 | Sin conexión |
| Pin 4 | Sin conexión |
| Pin 5 | Sin conexión |
| Pin 6 | Sin conexión |

---

# Componentes internos

| Cantidad | Componente |
|----------|------------|
| 2 | Resistencia de 120 Ω |

No se detectaron componentes activos durante las mediciones.

---

# Ingeniería inversa

Las mediciones muestran que el terminador está compuesto únicamente por dos resistencias independientes de 120 Ω.

Una resistencia conecta los pines **1 y 2**, mientras que la segunda conecta los pines **7 y 8**.

Los pines **3**, **4**, **5** y **6** permanecen completamente desconectados.

Hasta el momento no se han observado resistencias de polarización, diodos, condensadores ni otros componentes electrónicos.

---

# Estado

- ✅ Pinout identificado
- ✅ Valores de resistencias medidos
- ✅ Esquema eléctrico obtenido
- ✅ Ingeniería inversa completada

---

# Trabajo futuro

- Confirmar la función de cada par diferencial mediante un analizador lógico u osciloscopio.
- Verificar el comportamiento del terminador durante el funcionamiento del bus A-Link.
