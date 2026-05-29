# ⚽ Agenda Deportiva · Bot de Fútbol con IA

> Picks, resúmenes y alertas de partidos en vivo — directo a tu Telegram.

[![Bot Telegram](https://img.shields.io/badge/Telegram-Abrir%20Bot-2CA5E0?...)](https://t.me/agendafutbol_bot)
[![Estado](https://img.shields.io/badge/Estado-En%20vivo-00C851?style=for-the-badge)]()
[![Picks IA](https://img.shields.io/badge/IA-Groq%20%2B%20Gemini-FF6B35?style=for-the-badge)]()

---

## ¿Qué hace?

Recibís análisis generados por IA antes de cada partido, resúmenes en el descanso y al final, y alertas de goles — todo sin salir de Telegram.

| Cuándo | Qué recibís |
|---|---|
| 1h antes del partido | Pick pre-partido con contexto de la llave |
| Descanso | Resumen del primer tiempo |
| Final | Análisis completo del partido |
| Gol | Alerta instantánea |

---

## Comandos disponibles

```
/hoy       → Partidos del día con horarios y estado en vivo
/pick      → Análisis IA del partido (ej: /pick Argentina)
/estado    → Estado de los servicios del bot
```

---

## Cómo empezar

**1.** Abrí el bot → [→ **@agendafutbol_bot**](https://t.me/agendafutbol_bot)

**2.** Escribí `/hoy` para ver los partidos del día

**3.** Escribí `/pick [equipo]` para recibir el análisis IA

Sin registro. Sin contraseña. Sin app.

---

## Cobertura

- 🏆 Copa del Mundo FIFA
- 🌎 Eliminatorias CONMEBOL
- 🇦🇷 Liga Profesional Argentina
- ⚽ Principales ligas europeas
- 📅 Más competiciones en camino

---

## Cómo funciona

```
API-Football → n8n → PostgreSQL → Groq / Gemini → Telegram
                ↓
          GitHub Pages (datos en vivo públicos)
```

Los datos se actualizan cada 60 segundos durante partidos activos.
Los picks se generan automáticamente al detectar cambios de estado.
Si el proveedor de IA primario falla, hay fallback automático.

---

## Stack técnico

| Capa | Tecnología |
|---|---|
| Automatización | n8n |
| Base de datos | PostgreSQL |
| IA primaria | Groq (llama-3.3-70b) |
| IA secundaria | Gemini 1.5 Flash |
| Datos deportivos | API-Football |
| Frontend | GitHub Pages |
| Entrega | Telegram Bot API |

---

## Datos en vivo

Los datos de partidos del día están disponibles públicamente:

- **Partidos:** [`/public/live.json`](https://leitocuba.github.io/agenda-deportiva.github.io/public/live.json)
- **Picks IA:** [`/public/picks.json`](https://leitocuba.github.io/agenda-deportiva.github.io/public/picks.json)

Actualizados automáticamente cada 30 minutos.

---

## ¿Querés contribuir?

El proyecto está en Stage 1 — MVP en validación.

Si encontrás un bug o querés sugerir una competición:
→ Abrí un [Issue](https://github.com/leitocuba/agenda-deportiva.github.io/issues)
→ O escribile directamente al bot con `/feedback`

---

## Roadmap

- [x] Picks pre-partido con IA
- [x] Resúmenes de descanso y tiempo completo
- [x] Alertas de goles
- [x] Datos en vivo públicos (JSON)
- [ ] Suscripción por equipo favorito
- [ ] Estadísticas históricas
- [ ] Más competiciones

---

<div align="center">

[→ **@agendafutbol_bot**](https://t.me/agendafutbol_bot)

Hecho con ⚽ y demasiado café

</div>
