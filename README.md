# BodyMap para Masajistas (TriggerPoints PRO • Medical Grade)

Plataforma anatómica y de mapeo miofascial de grado médico basada en la semiología de Travell & Simons, cadenas miofasciales de Thomas Myers y osteopatía funcional.

## Características

- **Fotogrametría Anatómica Real**: Modelos de estudio de alta definición masculinos y femeninos en postura neutral clínica.
- **Transiluminación & Disección Tisular Profunda**: Control deslizante interactivo de profundidad (0% Piel real a 100% Plano profundo y esquelético) para visualizar estructuras profundas como Piriforme, Cuadrado Lumbar y Multífidos.
- **Reparos Óseos Palpables (*Palpable Bony Landmarks*)**: Guías óseas anatómicas (C7, Acromion, EIPS, Trocánter, EIAS, Rótula) para orientación palpatoria manual.
- **Mapeo Térmico de Dolor Referido**: Visualización en tiempo real de zonas esenciales primarias y satélites secundarias.
- **Dossier Clínico para Terapeutas**: Protocolos de tratamiento manual (Compresión isquémica progresiva, MET / Energía muscular, liberación fascial) y banderas rojas médicas.

## Estructura del Proyecto

```
bodymap-para-masajistas/
├── index.html                  # Aplicación clínica interactiva
├── analyze_landmarks.js        # Utilidad de análisis de puntos de referencia
├── assets/
│   └── images/                 # Fotogrametría anatómica de estudio
│       ├── female_anterior.jpg
│       ├── female_posterior.jpg
│       ├── male_anterior.jpg
│       └── male_posterior.jpg
├── .gitignore
└── README.md
```

## Despliegue en Vercel

Este proyecto es una aplicación estática optimizada que no requiere proceso de compilación (*zero-config*). Puede desplegarse directamente ejecutando:

```bash
vercel
```
o conectando el repositorio de GitHub en el panel de control de Vercel.
