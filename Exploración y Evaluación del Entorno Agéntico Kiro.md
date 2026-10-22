# Exploración y Evaluación del Entorno Agéntico Kiro

## Visión General de la Herramienta
Kiro es un entorno de desarrollo agéntico (*Agentic AI IDE*) construido sobre la base de Code OSS e impulsado por modelos de lenguaje avanzados vía Amazon Bedrock y conectores agénticos. Kiro fue diseñado para operacionalizar el paradigma de *Spec-Driven Development* (SDD), asegurando que la IA trabaje bajo contratos formales.

---

## Cuadro Resumen del Flujo de Trabajo en Kiro

```mermaid
flowchart LR
    A["Incepción Prompt / Idea"] --> B["1. requirements.md EARS & Criterios"]
    B --> C["2. design.md Arquitectura & APIs"]
    C --> D["3. tasks.md Tareas Atómicas"]
    D --> E{"Modo de Ejecución"}
    E -->|Autopilot| F["Ejecución Autónoma & Terminal"]
    E -->|Supervised| G["Aprobación Humana Paso a Paso"]
    F --> H["4. Correctness Pruebas de Propiedades"]
    G --> H
    H --> I["Código de Producción Auditable"]
