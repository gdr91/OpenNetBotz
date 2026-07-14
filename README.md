# OpenNetBotz

> Proyecto de código abierto dedicado a la ingeniería inversa, documentación y desarrollo de sensores y accesorios compatibles con los equipos APC™ NetBotz®.

> **Aviso:** Este proyecto es un esfuerzo independiente de la comunidad y **no está afiliado, respaldado ni patrocinado por Schneider Electric ni APC**. Todas las marcas comerciales pertenecen a sus respectivos propietarios.

---

# Descripción

OpenNetBotz nace con el objetivo de documentar y desarrollar soluciones abiertas para los sistemas de monitoreo ambiental NetBotz.

El proyecto busca crear una base de conocimiento técnica que permita a cualquier persona:

* Fabricar sensores compatibles.
* Reparar sensores originales.
* Diseñar nuevas soluciones para NetBotz.
* Comprender el funcionamiento del puerto universal de sensores.
* Compartir información técnica obtenida mediante ingeniería inversa.

Toda la información publicada intenta estar respaldada por pruebas reales y mediciones realizadas sobre hardware físico.

---

# Objetivos

* Documentar el funcionamiento de los sensores originales.
* Realizar ingeniería inversa de los distintos modelos.
* Diseñar sensores compatibles utilizando componentes comerciales.
* Publicar esquemáticos electrónicos y PCB en KiCad.
* Desarrollar firmware cuando sea necesario.
* Crear adaptadores para sensores externos.
* Reducir el costo de reemplazo de sensores originales.
* Preservar equipos NetBotz antiguos mediante soluciones abiertas.

---

# Equipos compatibles

| Modelo      | Estado              |
| ----------- | ------------------- |
| NetBotz 150 | 🔄 En investigación |
| NetBotz 250 | ⏳ Planificado       |
| NetBotz 450 | ⏳ Planificado       |
| NetBotz 750 | 🔄 En pruebas       |

---

# Sensores

| Sensor                  | Estado                |
| ----------------------- | --------------------- |
| Temperatura (AP9335T)   | 🔄 Ingeniería inversa |
| Temperatura y Humedad   | ⏳ Pendiente           |
| Sensor de puerta        | 🔄 Ingeniería inversa |
| Detector de fugas       | ⏳ Pendiente           |
| Contacto seco           | ⏳ Pendiente           |
| Entrada analógica 0–5 V | ⏳ Pendiente           |

---

# Estructura del repositorio

```text
docs/
    
sensors/
    AP9335T/
    NBES0303/

firmware/
    Código fuente

adapters/

tools/

firmware/

research/
```

---

# Estado de la documentación

Para diferenciar información confirmada de hipótesis, se utilizarán los siguientes indicadores:

| Símbolo | Significado                                        |
| ------- | -------------------------------------------------- |
| ✅       | Verificado mediante pruebas y mediciones           |
| 🟡      | Reportado por la comunidad, pendiente de confirmar |
| 🔴      | Hipótesis o información en investigación           |

---

# Cómo colaborar

Toda colaboración es bienvenida.

Puedes ayudar:

* Compartiendo fotografías de sensores.
* Midiendo componentes.
* Realizando pruebas.
* Diseñando PCB.
* Corrigiendo documentación.
* Reportando compatibilidad.
* Analizando protocolos de comunicación.

El objetivo es construir una base de conocimiento abierta para toda la comunidad NetBotz.

---

# Herramientas utilizadas

Durante el proyecto se utilizarán, entre otras:

* Multímetro digital
* Osciloscopio
* Analizador lógico
* KiCad
* Impresora 3D (opcional)

---

# Hoja de ruta

## Primera etapa

* Ingeniería inversa del AP9335T.
* Ingeniería inversa del sensor de puerta.
* Documentación del puerto universal.

## Segunda etapa

* Primer sensor DIY compatible.
* PCB universal para sensores.
* Sensor de fuga de agua.

## Tercera etapa

* Sensor de temperatura y humedad.
* Adaptadores para sensores analógicos.
* Validación comunitaria.

---

# Licencia

Este proyecto utiliza licencias abiertas. Consulta el archivo **LICENSE** para obtener más información.

---

# Agradecimientos

Gracias a todas las personas que colaboran compartiendo información, mediciones, fotografías y pruebas para ampliar el conocimiento sobre los equipos APC NetBotz.
