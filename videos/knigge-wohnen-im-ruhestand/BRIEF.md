---
workflow: general-video
flow: automation
storyboard: "no"
message: "Nicht weniger Zuhause – mehr Leben: Der Umzug vom großen Haus in eine passende Wohnung ist ein Gewinn, und KNIGGE Immobilien begleitet Sie dabei von Anfang bis Ende."
destination: youtube + instagram-reels
aspect: 1920x1080 + 1080x1920
language: de
audience: "Eigentümer im Ruhestand (ca. 65–85) mit großem Einfamilienhaus in Bergisch Gladbach / Köln-Ost; sekundär deren erwachsene Kinder"
length: 75s
angle: emotional-persuasive brand film (narrative, sound-off-first)
narration: "no"
---

## Intent

Info- und Werbefilm für KNIGGE Immobilien e.K. (Bergisch Gladbach). Ruheständler sollen Lust
bekommen, ihr zu groß gewordenes Haus zu verkaufen und in eine komfortable Wohnung zu ziehen –
vollständig begleitet durch KNIGGE. Ton laut Nutzer: „sympathisch“, „psychologisch aufgebaut für
maximale Überzeugung“. Sie-Ansprache, seriös, lokal-persönlich, keine Superlative ohne Beleg,
keine Wettbewerber-Nennung (KNIGGE-Tonalität).

Psychologischer Bogen (Reihenfolge ist Absicht):

1. **Nostalgie & Identifikation** – Erinnerungen ans Haus (Aufmerksamkeit, „das bin ich“).
2. **Pacing der Gegenwart** – Stille, Treppen, Garten, Heizkosten; empathisch, ohne Angstappell.
3. **Reframing** – Verlust wird Gewinn: „Nicht weniger Zuhause. Mehr Leben.“
4. **Future Pacing** – konkrete Bilder des neuen Alltags (Aufzug, Balkon, Bäcker, Reisen, Kapital).
5. **Autonomie + sanfte Dringlichkeit** – „Solange Sie ihn selbst bestimmen können.“
6. **Einwandbehandlung & Risikoreduktion** – „Und der ganze Aufwand? Den nehmen wir Ihnen ab.“ – 4 klare Schritte.
7. **Sympathie & Autorität** – lokal verwurzelt (Stadtteile), rund 1.600 verwaltete Wohneinheiten.
8. **Reziprozität & kleiner erster Schritt** – kostenloses, unverbindliches Gespräch „bei einer Tasse Kaffee“; Peak-End: warmer Abschluss mit Claim.

## Assets

- assets/brand/knigge-logo.svg — Logo als Vektor **nachgebaut** nach CI-Mustern aus Canva (rotes K-Faltquadrat + Wortmarke Montserrat). Vor Veröffentlichung durch Original-Logodatei ersetzen.
- assets/audio/knigge-theme.m4a — eigens komponierte Musik (Klavier/Streicher, 80 BPM, F-Dur), erzeugt mit tools/music/compose.py.
- assets/fonts/ — Newsreader (OFL) für die emotionale Stimme; Montserrat ist im Renderer gebündelt.

## Customizations

- Zwei Formate aus denselben Szenen: `index.html` (16:9, YouTube) und `formats/9x16.html` (9:16, Instagram Reels). Szenen layouten per Container-Queries.
- Musik-Struktur folgt exakt den Szenengrenzen (1 Takt = 3 s).
- Optionaler Sprechertext in SCRIPT.md (für spätere Aufnahme, z. B. durch Inhaber/Makler).

## Notes

- Website knigge-immobilien.de war aus der Build-Umgebung nicht erreichbar (Netzwerk-Policy) → kein Website-Capture; CI aus vorhandenen KNIGGE-Canva-Designs abgeleitet.
- Zu prüfende Fakten vor Veröffentlichung: Telefonnummer 02202 12 40 300, „kostenlose Wertermittlung“, „rund 1.600 verwaltete Wohneinheiten“.
- Reels-Safe-Zone: keine Pflichtinhalte im unteren ~20 % und oberen ~10 % des 9:16-Formats.
