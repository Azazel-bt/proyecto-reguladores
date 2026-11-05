# Reguladores de tensión LM7805 (lineal) vs. LM2596 (conmutado buck)

Comparación experimental de dos topologías de regulación de 5 VDC a 1 A
a partir de una etapa común de rectificación y filtrado.

## 📋 Especificaciones

| Parámetro            | Requerido         |
|----------------------|-------------------|
| Tensión de entrada   | 10 VDC            |
| Tensión de salida    | 5 VDC             |
| Corriente de salida  | Hasta 1 A         |
| Rizado de salida     | < 50 mV pico      |

## 📁 Contenido del repositorio

- `docs/` — Informe en PDF y fuentes LaTeX.
- `fotos/` — Registro fotográfico del montaje y las mediciones.
- `videos/` — Grabaciones de las pruebas de laboratorio.
- `simulaciones/` — Circuitos y resultados de LTspice.
- `datos/` — Hojas de cálculo con las mediciones.
- `codigo/` — Scripts de cálculo y generación de gráficas.

## 🎬 Videos destacados

| Video | Descripción |
|-------|-------------|
| [Rizado LM7805](videos/01_medicion_rizado_lm7805.mp4) | Medición con osciloscopio en la salida del regulador lineal |
| [Rizado LM2596](videos/02_medicion_rizado_lm2596.mp4) | Medición con osciloscopio en la salida del buck |
| [Prueba de carga LM2596](videos/04_prueba_carga_lm2596.mp4) | Comportamiento con carga de 5,1 Ω |

## 📊 Resultados principales

| Métrica              | LM7805      | LM2596               |
|----------------------|-------------|----------------------|
| V_out medida         | 4,99 V      | 5,0 V (reg.) / 4,3 V (carga) |
| I_out medida         | 197,1 mA    | 710 mA               |
| Rizado de salida     | 12 mV pico  | ≈ 49 mV pico         |
| Eficiencia           | 48,7 %      | 61,1 % / 71,0 %      |
| Disipación           | ≈ 0,99 W    | ≈ 0,42 W             |

## 🛠️ Herramientas

- **Simulación**: LTspice XVII
- **Instrumentación**: Multímetro UNI-T UT58A, osciloscopio GWINSTEK GDS-1062
- **Documentación**: LaTeX (Overleaf)
- **Control de versiones**: Git + Git LFS
