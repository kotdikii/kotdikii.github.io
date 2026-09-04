---
title: "Guía del usuario — DeepCheck"
---

DeepCheck es una aplicación para diagnosticar los componentes de hardware de un smartphone: pantalla, sensores, cámara, micrófono, altavoces, almacenamiento, módulos de conectividad y más. Todas las pruebas se realizan **localmente en el dispositivo**, sin transmitir datos a internet.

Esta guía explica cómo usar la aplicación y realizar las pruebas.

---

## Contenido

1. [Principios generales](#principios-generales)
2. [Navegación por la aplicación](#navegación-por-la-aplicación)
3. [Sección «Componentes»](#sección-componentes)
4. [Lista de pruebas](#lista-de-pruebas)
5. [Modo «Serie»](#modo-serie)
6. [Prueba de estrés del procesador](#prueba-de-estrés-del-procesador)
7. [Prueba de RAM](#prueba-de-ram)
8. [Prueba de almacenamiento](#prueba-de-almacenamiento)
9. [Prueba de GPU](#prueba-de-gpu)
10. [Sección «Acerca del dispositivo»](#sección-acerca-del-dispositivo)
11. [Ajustes](#ajustes)
12. [Versión Pro y limitaciones del modo gratuito](#versión-pro-y-limitaciones-del-modo-gratuito)
13. [Permisos](#permisos)
14. [Preguntas frecuentes](#preguntas-frecuentes)

---

## Principios generales

- La mayoría de las pruebas son **interactivas**: la aplicación indica qué hacer (tocar, deslizar el dedo, acercar el dedo, escuchar un sonido, etc.) y tú confirmas el resultado: la prueba **se supera** o **no se supera**.
- Al final de cada prueba se registra el resultado: ✅ superada o ❌ no superada. Esto ayuda a saber qué componentes funcionan correctamente.
- Antes de las pruebas que requieren acceso al hardware (cámara, micrófono, sensores, almacenamiento), la aplicación solicita el **permiso** correspondiente. Sin permiso, la prueba estará limitada.
- La aplicación no recopila ni envía tus datos a ningún sitio.

---

## Navegación por la aplicación

### Menú lateral (☰)

Se abre con el botón de tres líneas en la esquina superior izquierda o deslizando desde el borde izquierdo. Contiene las secciones principales:

- **Componentes** — lista de 24 pruebas individuales de componentes de hardware.
- **Acerca del dispositivo** — información detallada sobre el hardware y las características del smartphone.
- **Prueba de estrés** — prueba de carga del procesador.
- **Prueba de RAM** — benchmark de la memoria RAM.
- **Prueba de almacenamiento** — benchmark de la velocidad de almacenamiento.

### Menú de tres puntos (⋮)

Se abre con el botón de la esquina superior derecha. Contiene:

- **Ajustes** — elección de tema, paleta e idioma.
- **Ayuda** — abre esta guía.
- **Acerca de la app** — versión, funciones e información sobre el desarrollador.

---

## Sección «Componentes»

Es la sección principal con las pruebas individuales. Elige la prueba que quieras de la lista y la aplicación te guiará paso a paso por la comprobación.

**Cómo se realiza una prueba:**

1. Abre la prueba de la lista.
2. Lee la instrucción de la pantalla inicial (qué se va a comprobar y cómo).
3. Inicia la comprobación y realiza las acciones requeridas.
4. Confirma el resultado: si el componente funciona correctamente, márcalo como **superada**; si hay un problema, márcalo como **no superada**.

Al terminar volverás a la lista, donde se verá qué pruebas ya se han realizado y con qué resultado.

---

## Lista de pruebas

La aplicación incluye **24 pruebas**, agrupadas por tipo de componente.

### Pantalla y táctil

- **Prueba de pantalla** — comprobación de la reproducción de color y búsqueda de píxeles muertos (relleno de la pantalla con colores sólidos).
- **Prueba táctil** — comprobación de la respuesta de toda la superficie del táctil.
- **Prueba multitáctil** — comprobación del reconocimiento simultáneo de varios toques.
- **Prueba de brillo** — comprobación del ajuste del brillo de la retroiluminación.

### Botones y biometría

- **Prueba de botones** — comprobación de los botones físicos (volumen, encendido, etc.).
- **Prueba de huella** — comprobación del sensor de huella dactilar (se requiere al menos una huella añadida en los ajustes del sistema).

### Sonido y vibración

- **Prueba de audio** — comprobación de los altavoces.
- **Prueba de auriculares** — comprobación de los auriculares con o sin cable.
- **Prueba de vibración** — comprobación del motor de vibración.

### Cámara y flash

- **Prueba de cámara** — comprobación de las cámaras frontal y principal.
- **Prueba de flash** — comprobación del flash LED.

### Alimentación y almacenamiento

- **Prueba de carga** — control del estado y los parámetros de carga.
- **Prueba de tarjeta SD** — comprobación de la ranura MicroSD (hay que insertar una tarjeta).
- **Prueba de OTG** — comprobación de la compatibilidad con USB-OTG (hay que conectar un dispositivo externo).

### Conectividad

- **Prueba de NFC** — comprobación del módulo NFC.
- **Prueba de tarjetas SIM** — comprobación de la detección de tarjetas SIM.
- **Prueba de Wi-Fi** — comprobación del módulo Wi-Fi.
- **Prueba de Bluetooth** — comprobación del módulo Bluetooth.
- **Prueba de GPS** — comprobación de la recepción de la señal de satélite.

### Sensores

- **Prueba de acelerómetro** — comprobación del sensor de aceleración.
- **Prueba de giroscopio** — comprobación del sensor de velocidad angular.
- **Prueba de magnetómetro** — comprobación de la brújula digital.
- **Prueba de luz** — comprobación del sensor de luz ambiental.
- **Prueba de proximidad** — comprobación del sensor de proximidad (se activa junto a la oreja durante una llamada).

> El conjunto de pruebas disponibles depende de los módulos y sensores que tenga tu dispositivo.

---

## Modo «Serie»

El modo **«Serie»** permite ejecutar varias pruebas seleccionadas seguidas, sin volver cada vez a la lista. Resulta cómodo para una comprobación integral rápida del dispositivo (por ejemplo, antes de comprar o vender un smartphone).

- Selecciona las pruebas que quieras e inicia la serie.
- Durante la serie aparece abajo un panel de control: ir a la prueba anterior/siguiente, omitir y finalizar.
- Al terminar la serie se genera un resumen: qué pruebas se superaron, fallaron, se omitieron o no se llevaron hasta el final.

> El modo «Serie» está disponible en la versión **Pro**.

---

## Prueba de estrés del procesador

Carga todos los núcleos del procesador y supervisa en tiempo real el uso de la CPU, la frecuencia y la temperatura del dispositivo. Sirve para comprobar la estabilidad, la refrigeración y detectar el throttling (reducción de frecuencia por sobrecalentamiento).

**Parámetros:**

- **Duración** — tiempo de ejecución de la prueba.
- **Nivel de carga** — de suave a máximo.
- **Perfil de carga:**
  - **Integral** — operaciones con enteros, aritmética SIMD/FP, matrices y memoria a la vez. Modo universal por defecto, cercano a escenarios reales.
  - **FPU-torch** — carga máxima sobre la unidad de coma flotante. El modo más «caliente»; provoca el throttling más rápido y revela inestabilidad.
  - **Memoria** — trabajo intensivo con el subsistema de memoria. Calienta el controlador de memoria y comprueba el ancho de banda y la estabilidad de la RAM.

**Durante la prueba** se muestran gráficos de carga y temperatura. Si se detecta una reducción de frecuencia bajo carga, la aplicación informará del **throttling detectado**.

**Historial de comprobaciones** — los resultados de las últimas ejecuciones se guardan para poder comparar el comportamiento del dispositivo en distintos momentos o con distintos ajustes.

---

## Prueba de RAM

Benchmark de la memoria RAM. Mide la velocidad de escritura, lectura, copia y la latencia de acceso a la memoria. Los resultados ayudan a evaluar el rendimiento del subsistema de memoria del dispositivo.

> En algunos dispositivos la prueba puede funcionar en **modo limitado**, debido a las restricciones del sistema sobre la cantidad de memoria asignable.

---

## Prueba de almacenamiento

Benchmark de la velocidad de almacenamiento: mide la velocidad real de lectura y escritura.

- El **almacenamiento interno** se prueba gratis.
- Las **unidades externas** (USB-OTG, tarjeta SD) — la comprobación está disponible en la versión **Pro**.

**Precisar la versión de la unidad USB.** Al conectar una unidad externa, la aplicación puede ofrecer permitir el acceso al dispositivo USB para distinguir una unidad USB 3.0 de una USB 2.0 al conectarla a un puerto USB 2.0 del teléfono. Es opcional: la prueba empezará de todos modos, pero la precisión al determinar las características será menor.

> Ten en cuenta: la velocidad real puede estar limitada por el puerto USB del propio dispositivo, no por la unidad.

---

## Prueba de GPU

Benchmark del procesador gráfico para comparar la potencia de los dispositivos con métricas claras —**GFLOPS** y **FPS**— y comprobar el throttling bajo carga prolongada.

Una ejecución es **una única etapa continua** bajo carga:

- **GFLOPS** — rendimiento de cálculo del núcleo gráfico, medido con un cálculo compute puro. Esa misma carga calienta la GPU, por lo que, a partir de la caída de los GFLOPS a lo largo del tiempo, la aplicación detecta el **throttling** (reducción de frecuencia por sobrecalentamiento).
- **Escena 3D (FPS)** — durante la carga de GFLOPS, breves sondeos miden los FPS de una escena 3D (la carga se pausa un instante para que la medición sea precisa). Los FPS muestran la caída de los gráficos por sobrecalentamiento. La escena se puede desactivar en los ajustes de la prueba: entonces solo se mide GFLOPS.

**Parámetros:**

- **Duración** — de 2 a 15 minutos. Las ejecuciones de menos de 2 minutos no se guardan en el historial: hay pocos datos y el throttling no llega a manifestarse.
- **Ejecutar escena 3D (FPS)** — activar/desactivar los sondeos de FPS.

Los primeros ~30 segundos transcurren «en frío»: así se registra el rendimiento máximo antes del calentamiento. La prueba se ejecuta a pantalla completa con la orientación bloqueada; el dispositivo se calentará notablemente. Al finalizar se muestran el pico y los GFLOPS medios, los FPS, el throttling detectado y la temperatura de la GPU. Los resultados se guardan en el **historial de ejecuciones**.

> Cuanto más potente sea el núcleo gráfico, mayores serán los GFLOPS y los FPS. Los resultados son comparables entre dispositivos, pero una sola prueba sintética no clasifica de forma perfecta arquitecturas distintas (por ejemplo, Adreno y Mali); esto es normal en cualquier benchmark.
> Si el dispositivo ya estaba caliente al inicio, el pico y la caída pueden estar infravalorados: déjalo enfriar y reinicia la prueba.

---

## Sección «Acerca del dispositivo»

Un resumen detallado del hardware del smartphone: procesador, memoria, pantalla, cámaras, sensores, módulos de conectividad, versión de Android, parche de seguridad y otras características. Útil para comprobar que se corresponde con las características anunciadas.

---

## Ajustes

Disponibles en el menú de tres puntos → **Ajustes**:

- **Tema** — claro, oscuro o del sistema.
- **Paleta** — los colores de DeepCheck o de una de las aplicaciones hermanas (Deedary, Seriary). Funciona junto con el tema: cada paleta tiene variante clara y oscura.
- **Idioma** — idioma de la interfaz (o el idioma del sistema).

Los ajustes se aplican al instante y se conservan entre reinicios de la aplicación.

---

## Versión Pro y limitaciones del modo gratuito

Las pruebas básicas están disponibles gratis. Parte de las funciones forman parte de la versión **Pro**:

- **Modo «Serie»** — ejecutar varias pruebas seguidas.
- **Exportación de resultados a PDF.**
- **Comprobación de unidades externas** (USB-OTG y tarjetas SD). El almacenamiento interno se prueba gratis.
- **Ejecuciones ilimitadas** de la prueba de estrés, la de RAM, la de almacenamiento y la de GPU (en el modo gratuito el número de ejecuciones es limitado, con el mismo límite para cada una de estas pruebas).
- **Duración ampliada** de la prueba de estrés.

En el modo gratuito, la aplicación muestra cuántas ejecuciones quedan. Al agotar el límite aparecerá una oferta para pasar a Pro.

---

## Permisos

La aplicación solicita permisos únicamente para comprobar un hardware concreto y **solo en el momento** en que son necesarios para la prueba correspondiente:

- **Cámara** — para la prueba de cámara y flash.
- **Micrófono** — para la comprobación de sonido/grabación.
- **Ubicación** — para la prueba de GPS y el escaneo de Wi-Fi.
- **Acceso a archivos/almacenamiento** — para la prueba de almacenamiento.
- **Bluetooth, NFC, etc.** — para las pruebas de conectividad correspondientes.

Si has denegado un permiso, la prueba estará limitada. El permiso se puede conceder más tarde en los ajustes del sistema de la aplicación.

---

## Preguntas frecuentes

**La prueba no se inicia o el módulo «no se encuentra».**
Lo más probable es que tu dispositivo no tenga el módulo de hardware correspondiente (por ejemplo, NFC o magnetómetro), o que no se haya concedido el permiso necesario.

**La velocidad del almacenamiento es más baja de lo esperado.**
La velocidad real puede estar limitada por el puerto USB del dispositivo, el tipo de conexión o el estado de la unidad.

**La prueba de estrés muestra throttling, ¿es una avería?**
No necesariamente. La reducción de frecuencia bajo carga prolongada es un mecanismo normal de protección contra el sobrecalentamiento. Un throttling fuerte y temprano puede indicar problemas de refrigeración.

**¿Dónde están mis datos?**
Todos los resultados y mediciones permanecen en el dispositivo. La aplicación no envía datos a internet. Más detalles en la Política de privacidad.

---

*Si te queda alguna duda, escribe al desarrollador: **kotdikii@gmail.com***
