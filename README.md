# Polla Mundial 2026

App interactiva para una polla del Mundial FIFA 2026 (Canadá / México / USA) con predicciones, dashboard en vivo y sincronización en tiempo real.

**URL en vivo:** https://akiotanaka847.github.io/polla-mundial-2026/

## Features

- **Predicciones de 72 partidos de grupo** con sistema de puntos (exacto/diferencia/ganador)
- **Multiplicadores por ronda** — grupos x1, octavos x1.5, hasta final x4
- **Selección de campeón** — bonus +15 pts, decisión definitiva (no se puede cambiar)
- **Eliminatorias auto-generadas** desde resultados de grupo
- **Bloqueo automático** de predicciones 6h antes de cada partido
- **Dashboard en vivo** con pozo acumulado, top 5, favoritos al título, estadísticas
- **Sistema de pagos** — entrada $30K COP, admin aprueba correos manualmente
- **Gestión de usuarios** — roles Admin/Editor/Participante, reset de claves
- **Resultados en vivo** via football-data.org API (opcional)
- **Sincronización en tiempo real** con Firebase Realtime Database

## Stack

- **HTML + CSS + JS** vanilla (sin frameworks)
- **Firebase Realtime Database** — sincronización entre participantes
- **football-data.org** — resultados en vivo del Mundial
- **GitHub Pages** — hosting gratis

## Configuración

1. Crea un proyecto en [Firebase Console](https://console.firebase.google.com)
2. Activa Realtime Database en modo prueba
3. Reemplaza `firebaseConfig` en `index.html`
4. (Opcional) Obtén una API key gratis en [football-data.org](https://www.football-data.org/client/register)
5. Sube a GitHub Pages o cualquier hosting estático

## Reglas de puntuación

| Acierto | Puntos |
|---|---|
| Marcador exacto | +5 |
| Diferencia y ganador | +3 |
| Solo ganador/empate | +2 |
| Campeón del mundo | +15 |
| Finalista | +8 |
| Semifinalista | +5 |

## Distribución del pozo

- **60%** al 1ro
- **25%** al 2do
- **15%** al 3ro
