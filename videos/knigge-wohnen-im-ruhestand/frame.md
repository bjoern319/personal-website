---
version: alpha
name: KNIGGE Immobilien — Frame (video layer)
description: >
  Video-Designsystem für KNIGGE Immobilien e.K. Abgeleitet aus vorhandenen KNIGGE-Designs:
  rotes, gefaltetes K-Quadrat als Bildmarke, Wortmarke in Montserrat (KNIGGE fett, IMMOBILIEN
  gesperrt), diagonale Schnitte als Gestaltungsmotiv, viel Weiß/Warmweiß. Für die Zielgruppe
  Ruhestand: warm, ruhig, gut lesbar, großzügige Schriftgrößen, sanfte Bewegungen.
unit: the frame — 1920×1080 (YouTube) und 1080×1920 (Reels); Szenen skalieren über cqmin
principle: CI-Atome sind fix · Komposition ist frei · Fakten nur aus dem Brief

colors:
  canvas: "#F5F0E8"        # warmes Leinen – Grundfläche aller Szenen
  canvas-deep: "#ECE3D5"   # Sand – Panels, Flächen
  paper: "#FFFDF9"         # Hauswände, Karten, Pills
  ink: "#2A2725"           # Anthrazit, warm – Text & Linienzeichnung
  ink-muted: "#5F5A54"     # Sekundärtext
  ink-soft: "#8C857C"      # Hilfslinien
  red: "#C8102E"           # KNIGGE-Rot – Bildmarke, Akzente, CTA
  red-deep: "#8E1520"      # Bordeaux – Faltkante der Bildmarke
  red-dark: "#5E0D16"      # Schatten der Bildmarke
  warm-light: "#F2C36B"    # Fensterlicht = Leben/Erinnerung (funktional, nicht dekorativ)
  night: "#AEB6BF"         # Fenster ohne Licht (Szene „Stille“)

radii:
  pill: "999px"
  card: "18px"
  mark: "0"                # Bildmarke ist streng quadratisch

typography:
  voice-serif:  { fontFamily: "Newsreader", style: italic, weight: 400, cqmin: 7.2, lineHeight: 1.12, color: "ink" }   # emotionale Stimme
  headline:     { fontFamily: "Montserrat", weight: 700, cqmin: 6.4, lineHeight: 1.12, tracking: "-0.02em", color: "ink" }
  tagline:      { fontFamily: "Montserrat", weight: 900, cqmin: 10.5, lineHeight: 1.0, tracking: "-0.03em", color: "red" }
  body:         { fontFamily: "Montserrat", weight: 400, cqmin: 4.2, lineHeight: 1.3, color: "ink-muted" }
  list:         { fontFamily: "Montserrat", weight: 700, cqmin: 4.4, lineHeight: 1.2, color: "ink" }
  eyebrow:      { fontFamily: "Montserrat", weight: 700, cqmin: 2.4, tracking: "0.2em", upper: true, color: "red" }
  wordmark:     { fontFamily: "Montserrat", weight: 700, tracking: "0.02em", upper: true }
  wordmark-sub: { fontFamily: "Montserrat", weight: 400, tracking: "0.34em", upper: true }

spacing:
  pad-landscape: "6.5cqw"
  pad-portrait-x: "8cqw"
  pad-portrait-top: "12cqh"     # Reels-UI oben
  pad-portrait-bottom: "20cqh"  # Reels-UI unten
  stroke-illustration: "3.2"    # in SVG-Einheiten (viewBox 800×600)

components:
  k-mark:
    description: "Rotes Quadrat mit drei Facetten (K-Faltung): links hellrot, rechts Bordeaux, unten rot mit Schatten zur Ecke; feine helle Kontur."
  tag-pill:
    backgroundColor: "{colors.paper}"
    border: "0.3cqmin solid {colors.ink}"
    rounded: "{radii.pill}"
    typography: "Montserrat 700"
  step-dot:
    backgroundColor: "{colors.red}"
    textColor: "{colors.paper}"
    rounded: "50%"
  cta-pill:
    backgroundColor: "{colors.red}"
    textColor: "{colors.paper}"
    rounded: "{radii.pill}"
    typography: "Montserrat 700"
  illustration:
    description: "Linienzeichnung in {colors.ink}, Flächen in paper/canvas-deep, Dächer und Akzente in {colors.red}; zeichnet sich per Strich auf (svg-path-draw)."
---

## Overview

Warm, vertrauensvoll, regional. Das Rot ist Signal, nicht Fläche: Bildmarke, Schlüsselwörter,
Dach des Hauses, CTA. Alles andere lebt von Leinen, Papierweiß und warmem Anthrazit.

## Voices

- **Newsreader Italic** = innere Stimme / Gefühl („Erinnern Sie sich …?“).
- **Montserrat 700/900** = KNIGGE spricht: klar, strukturiert, verlässlich (CI-Schrift).

## Do

- Große Schrift (≥ 4 cqmin Fließtext), kurze Zeilen, lange Standzeiten.
- Sanfte Ease-Kurven (power2/power3.out, sine.inOut), keine harten Slams.
- Diagonale K-Faltung als Übergangsmotiv (Brand-Wipe) – sparsam.

## Don't

- Keine Angstappelle, keine Superlative, keine Wettbewerber.
- Kein reines Schwarz/Weiß, kein Rot als Vollfläche außer im Brand-Wipe und CTA.
