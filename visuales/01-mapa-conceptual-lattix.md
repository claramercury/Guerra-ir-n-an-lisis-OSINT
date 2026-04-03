# Mapa Conceptual Maestro — Proyecto Lattix

## Contexto

Este diagrama representa la arquitectura analítica completa del proyecto. No es un mapa del conflicto: es un mapa de **cómo pensamos el conflicto** y qué estructuras cognitivas están en juego.

## Diagrama principal

```mermaid
graph TD
    TRANS["<b>TRANSICIÓN DE ORDEN INTERNACIONAL</b><br/>Cambio en la gramática de lo pensable"]
    
    TRANS --> E1["<b>Frente 1: Militar-Estratégico</b><br/>Erosión del tabú nuclear"]
    TRANS --> E2["<b>Frente 2: Financiero</b><br/>Erosión del sistema petrodólar"]
    TRANS --> E3["<b>Frente 3: Cognitivo</b><br/>Erosión de la distinción<br/>realidad / interfaz"]
    
    E1 --> CONV["<b>CONVERGENCIA</b><br/>Los tres frentes se refuerzan<br/>mutuamente y están mediados por IA"]
    E2 --> CONV
    E3 --> CONV
    
    KAHN["<b>PARADOJA DE KAHN</b><br/>Democratización de herramientas<br/>≠ democratización de inteligencia"]
    KAHN -.->|"atraviesa"| E1
    KAHN -.->|"atraviesa"| E2
    KAHN -.->|"atraviesa"| E3
    
    GAME["<b>GAMIFICACIÓN</b><br/>Guerra como sistema interactivo:<br/>interfaz + feedback + monetización"]
    SPEC["<b>ESPECTACULARIZACIÓN</b><br/>Propaganda diseñada para<br/>ecosistemas algorítmicos"]
    
    E3 --> GAME
    E3 --> SPEC
    GAME -->|"retroalimenta"| E3
    SPEC -->|"retroalimenta"| E3
    
    TRIP["<b>TRÍPTICO EPISTÉMICO</b><br/>Corresponsal → Dashboard<br/>Testigo → Usuario<br/>Acontecimiento → Flujo"]
    
    GAME --> TRIP
    SPEC --> TRIP
    
    TRIP --> IND["<b>INDICADORES COGNITIVOS</b><br/>Taxonomía de señales tempranas<br/>de transición de orden"]

    style TRANS fill:#1a1a2e,color:#fff,stroke:#e94560
    style CONV fill:#0f3460,color:#fff,stroke:#e94560
    style KAHN fill:#533483,color:#fff,stroke:#e94560
    style E1 fill:#b91d3a,color:#fff
    style E2 fill:#d4a017,color:#000
    style E3 fill:#16537e,color:#fff
    style GAME fill:#1b4332,color:#fff
    style SPEC fill:#1b4332,color:#fff
    style TRIP fill:#2d3436,color:#fff
    style IND fill:#e94560,color:#fff
```

## Cómo leer este mapa

**Estructura vertical**: de arriba (la tesis general) hacia abajo (las herramientas analíticas concretas).

**Los tres frentes** (rojo, amarillo, azul) operan simultáneamente. La novedad no es que exista erosión en uno de ellos — es que los tres convergen al mismo tiempo y se refuerzan mutuamente.

**La Paradoja de Kahn** (violeta) es transversal: afecta a los tres frentes. En cada uno de ellos, la democratización de herramientas genera ilusión de comprensión sin comprensión real.

**Gamificación y espectacularización** (verde) son bucles de retroalimentación que agravan el frente cognitivo. No son consecuencias pasivas del conflicto: son mecanismos activos que modifican cómo se percibe y se procesa la guerra.

**El tríptico epistémico** resume la transformación en la estructura de la experiencia: quién informa (corresponsal → dashboard), quién observa (testigo → usuario), qué se observa (acontecimiento → flujo).

**Los indicadores cognitivos** (rojo inferior) son la contribución operativa: herramientas para detectar cuándo cambia la gramática de lo pensable *antes* de que cambie formalmente el sistema.

## Tesis central

> La novedad no es solo que la guerra sea retransmitida en tiempo real, sino que sea experimentada como sistema interactivo de observación, especulación y participación simbólica. Eso constituye un indicador de cambio de época.
