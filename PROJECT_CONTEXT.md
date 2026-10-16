# BodyMap (TriggerPoints PRO) • Dossier de Contexto del Proyecto

Este documento consolida el historial, arquitectura, calibración y despliegue del proyecto desarrollado a lo largo de esta sesión.

---

## 1. Identidad y Enlaces del Proyecto

* **Nombre Oficial:** BodyMap para Masajistas (TriggerPoints PRO • Medical Grade)
* **Directorio Local:** `C:\Users\I-MAG\.gemini\antigravity\scratch\bodymap-para-masajistas`
* **Repositorio GitHub:** [https://github.com/Zzaappaattaa223/triggerpoints-pro](https://github.com/Zzaappaattaa223/triggerpoints-pro)
* **Despliegue en Producción (Vercel):** [https://triggerpoints-pro.vercel.app](https://triggerpoints-pro.vercel.app)

---

## 2. Hitos y Evolución en Esta Sesión

1. **Aprovisionamiento del Entorno:**
   * Instalación de Node.js LTS v24.22.0 y npm v11.19.1.
   * Instalación y registro del servidor MCP **REA** (*Reverse Engineer Anything*) v6.5.0 (`mcp_config.json`).
   * Instalación de **Git** v2.56.0, **GitHub CLI (`gh`)** v2.102.0 y **Vercel CLI** v64.3.1.
   * Vinculación OAuth con la cuenta de GitHub `Zzaappaattaa223`.

2. **Ingeniería Inversa de `triggerpoints.net/es`:**
   * Análisis de la arquitectura Drupal 7 y su limitación gráfica (mapas de imágenes HTML 2D de los años 80-90).
   * Transformación hacia una arquitectura médica moderna con semiología palpatoria (Travell & Simons), cadenas miofasciales (Thomas Myers *Anatomy Trains*) y osteopatía.

3. **Fotogrametría Anatómica Real de Alta Definición:**
   * Sustitución de dibujos animados por 4 fotografías de estudio en pose neutra clínica (655 × 1024 px):
     * `female_posterior.jpg` y `female_anterior.jpg`
     * `male_posterior.jpg` y `male_anterior.jpg`
   * Almacenadas en `assets/images/`.

4. **Motor de Calibración Morfológica Diferenciada:**
   * Generador `ANATOMICAL_LANDMARKS` con datos antropométricos específicos para cada modelo y género (anchura biacromial, C7, ángulo de escápulas, trocánteres, EIPS, rótulas).
   * Superposición de curvas de Bézier orgánicas para musculatura profunda y zonas de dolor referido esencial (rojo) y satélite (ámbar).

5. **Experiencia de Usuario de Grado Estación Médica:**
   * Lienzo anatómico 100% despejado (eliminación del cuadro flotante que obstruía la cabeza/cuello).
   * Módulo de convenciones anatómicas integrado en la barra lateral.
   * Slider de transiluminación continua (0% piel real a 100% disección profunda y plano óseo).
   * Zoom interactivo (80% a 250%) y Pan con el ratón.
