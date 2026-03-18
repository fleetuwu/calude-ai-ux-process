# UX Skill System for Claude.ai

A set of 4 skills that guide Claude through a complete UX design process — from research to clickable prototype. Each skill builds on the previous one.

---

## Skills

| Skill | Was es tut |
|-------|-----------|
| **UXP-01 Research** | Golden Circle, Sinus-Milieu, 3 Personas, Empathy Map, JTBD, Interview-Guides, HMW, Opportunity-Solution-Tree, Research Readout |
| **UXP-02 Flows** | User Flows, Customer Journey Maps, Scenario Maps, Service Blueprints — als SVG + Mermaid-Code |
| **UXP-03 Wireframes** | Screen Inventory, Mid-Fi, High-Fi Wireframes mit Layer-Annotationen, Figma-Handoff |
| **UXP-04 Prototyping** | Klickbare iOS/Web Prototypen mit Light/Dark Mode, iOS-Transitions, Download als HTML |

---

## Beispiel-Output

**UXP-01** generiert automatisch Sinus-Milieu-Verortung, 3 Personas und JTBD-Statements.

**UXP-02** liefert immer einen SVG-Flow (direkt im Chat sichtbar) + vollständigen Mermaid-Code zum Copy-Pasten in Figma oder Confluence.

**UXP-03** baut ein klickbares Screen Inventory mit Layer-Panel, Komponenten-Annotationen und Props-Inspektion.

**UXP-04** generiert einen vollständig verdrahteten Prototyp mit iOS-Transitions, Light/Dark Switcher und Browser-Download-Hinweis.

---

## Installation

### Voraussetzung
- Claude.ai Account (Free, Pro oder Team)

### Schritte

1. Lade die gewünschten `.skill`-Dateien aus dem [Releases](../../releases)-Tab herunter
2. Öffne [claude.ai](https://claude.ai)
3. Gehe zu **Einstellungen → Skills**
4. Klicke auf **Skill hochladen** und wähle die `.skill`-Datei
5. Wiederhole für jeden Skill den du installieren möchtest

Die Skills sind unabhängig voneinander – du kannst einzelne oder alle 4 installieren.

---

## Verwendung

Starte einfach ein Gespräch mit deinem Projektkontext. Claude erkennt automatisch welcher Skill relevant ist:

```
"Ich baue eine Food Delivery App für iOS. 
Kannst du mir helfen die Zielgruppe zu analysieren?"
→ UXP-01 Research wird aktiviert

"Zeig mir den Bestellflow als Diagramm"
→ UXP-02 Flows wird aktiviert

"Erstell mir ein Screen Inventory für die App"
→ UXP-03 Wireframes wird aktiviert

"Bau mir einen klickbaren Prototyp des Checkout-Flows"
→ UXP-04 Prototyping wird aktiviert
```

---

## Kompletter Durchlauf

Die Skills sind aufeinander abgestimmt – ein typischer Durchlauf sieht so aus:

```
UXP-01  →  Sinus-Milieu + 3 Personas + JTBD
   ↓
UXP-02  →  User Flow als SVG + Mermaid-Code
   ↓
UXP-03  →  Screen Inventory mit Layer-Panel
   ↓
UXP-04  →  Klickbarer Prototyp + HTML-Download
```

---

## Technische Details

- **Plattform:** Claude.ai (Free, Pro, Team)
- **Format:** `.skill` (Claude.ai Skill-Format)
- **Sprache:** Deutsch (Outputs auf Deutsch, anpassbar)
- **Plattformen:** iOS und Web

### Geteilte Referenzen

UXP-03 und UXP-04 teilen sich eine gemeinsame Referenzdatei (`chat-patterns.md`) mit:
- Chat-Safe CSS-Regeln (iframe-kompatibel)
- Dark/Light Mode Token-System
- iOS + Web Device Frame Templates
- Transition Engine für Prototypen

---

## Changelog

### v1.0
- Initiale Veröffentlichung aller 4 Skills
- Dark/Light Mode in Prototypen
- Browser-Download-Hinweis in UXP-04
- `outline` statt `box-shadow` für Layer-Highlights (kein Clipping)
- Geteilte `chat-patterns.md` zwischen UXP-03 und UXP-04
- Pflicht: 3 Personas auf Basis Sinus-Milieu in UXP-01
- Pflicht: Mermaid-Code immer in UXP-02

---

## Lizenz

MIT — frei verwendbar und anpassbar.
