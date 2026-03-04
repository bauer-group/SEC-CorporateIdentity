# Canva — Design-Workflow

Die BAUER GROUP nutzt **Canva** als zentrale Design-Plattform für Print-Materialien, Werbemittel und digitale Inhalte. Fertige Entwürfe werden über Canva-Embed-Links direkt in diese Brand Guide eingebettet.

## Warum Canva?

| Vorteil | Details |
|---------|---------|
| **Zentrales Design-Tool** | Alle Entwürfe an einem Ort — Visitenkarten, Flyer, Social Media, Banner |
| **Team-Zugriff** | Gemeinsamer Workspace für alle Gestaltungsvorlagen |
| **Brand Kit** | Farben, Schriften und Logos zentral hinterlegt |
| **Live-Einbettung** | Änderungen in Canva werden automatisch im Brand Guide sichtbar |
| **Export** | PNG, PDF (Print-ready), MP4 — direkt aus dem Editor |

## Einsatzbereiche

| Bereich | Materialien | Beispiel |
|---------|-------------|----------|
| **Print** | Visitenkarten, Briefpapier, Briefumschläge, Flyer | Doppelseitige Visitenkarten mit QR-Code |
| **Werbemittel** | Block-Layouts, Mappen-Gestaltung, Etiketten | Schreibblock-Design mit Raster und Logo |
| **Digital** | Social Media Posts, Web-Banner, Newsletter-Header | Instagram-Story im Corporate Design |

## Einbettung im Brand Guide

Canva bietet native Embed-Links, die als iframe in VitePress-Seiten eingebettet werden können. Änderungen am Design in Canva werden **automatisch live** übernommen — kein manueller Export oder Re-Upload nötig.

### Schritt-für-Schritt

1. Design in Canva öffnen
2. **Teilen** (oben rechts) klicken
3. **Mehr …** → **Einbetten** wählen
4. **Smart Embed** Link kopieren
5. In die entsprechende Markdown-Seite einfügen

### Embed-Code Vorlage

```html
<!-- Canva Embed — 16:9 (Standard) -->
<div style="position:relative;width:100%;height:0;padding-bottom:56.25%;">
  <iframe src="https://www.canva.com/design/DESIGN_ID/view?embed"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"
    allowfullscreen></iframe>
</div>
```

### Seitenverhältnisse

| Format | `padding-bottom` | Anwendung |
|--------|-------------------|-----------|
| 16:9 | `56.25%` | Präsentationen, Banner |
| 4:3 | `75%` | Klassische Formate |
| 1:1 | `100%` | Social Media, Quadrate |
| A4 Hochformat | `141.4%` | Briefpapier, Flyer |
| Visitenkarte (85×55) | `64.7%` | Business Cards |

### Beispiel: Visitenkarte einbetten

```markdown
## Aktueller Entwurf

<div style="position:relative;width:100%;max-width:500px;height:0;
  padding-bottom:64.7%;margin:24px auto;">
  <iframe src="https://www.canva.com/design/DEIN_DESIGN_ID/view?embed"
    style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;
    border-radius:12px;box-shadow:0 4px 24px rgba(0,0,0,0.12);"
    allowfullscreen></iframe>
</div>
```

## Regeln & Hinweise

::: warning Öffentlich zugänglich
Eingebettete Designs werden **öffentlich** sichtbar. Nur finale, freigegebene Entwürfe einbetten — **keine** internen Entwurfsstufen, vertrauliche Daten oder Personendaten.
:::

::: tip Best Practices

- **Benennung**: Canva-Designs nach Schema benennen: `BAUER GROUP, [Material], [Format], Version [Datum]`
- **Brand Kit**: Immer die hinterlegten Markenfarben verwenden (#FF8500, Warm-Gray Skala, Neutral-Gray Skala)
- **Schriften**: System Font Stack verwenden — keine Canva-exklusiven Schriften
- **Export für Druck**: PDF (Print) mit Beschnittzugabe, CMYK-Farbprofil ISO 12647-2
- **Versionen**: Entwurfsversionen in Canva über den Versionsverlauf nachverfolgbar

:::

## Referenzen

Seiten mit Canva-Einbettungen:

- [Visitenkarten](/de/print/visitenkarten) — Doppelseitige Visitenkarten (DE/EN, CN/EN)
- [Werbemittel-Übersicht](/de/werbemittel/) — Übersicht aller Werbemittel

## Canva Brand Kit

Das BAUER GROUP Brand Kit in Canva enthält:

| Element | Wert |
|---------|------|
| **Primärfarbe** | #FF8500 (BAUER Orange) |
| **Warm-Gray** | #F9F8F6 – #231F1C (Skala) |
| **Neutral-Gray** | #F7F7F7 – #1C1C1C (Skala) |
| **Logo** | Wide + Square Variante (SVG) |
| **Schriften** | System Font Stack (Segoe UI / SF Pro / Roboto) |
