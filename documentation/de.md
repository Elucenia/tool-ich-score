<!-- ELUCENIA technical documentation · ich-score · de · no clinical/professional/rights approval -->

# ICH-Score

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/ich-score)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Glasgow-Koma-Skala

`gcs`

- `0` — 13 bis 15
- `1` — 5 bis 12
- `2` — 3 bis 4

### Hämatomvolumen ≥ 30 mL (ABC/2-Formel)

`vol`

### Intraventrikuläre Blutung

`ivh`

### Infratentorieller Ursprung

`infra`

### Alter ≥ 80 Jahre

`idade`

## Fassung der Methode

ICH/Hemphill 2001: 5 Faktoren, Gesamt 0–6; Volumen ABC/2; keine automatische Therapieentscheidung

## Dokumentierte Formel

Glasgow 3 bis 4 = 2 · 5 bis 12 = 1 · 13 bis 15 = 0; Volumen ≥ 30 mL = 1; Ventrikeleinbruch = 1; infratentorieller Ursprung = 1; Alter ≥ 80 Jahre = 1. Gesamt: 0 bis 6.

Volumen nach ABC/2: A = größter Hämatomdurchmesser in der flächengrößten Schicht; B = senkrechter Durchmesser zu A; C = Anzahl Hämatomschichten × Schichtdicke (cm). Ergebnis mL.

## Grenzen und Population

Schweregradschätzung bei Erstvorstellung einer intrazerebralen Blutung, in der Originalkohorte mit 30-Tage-Mortalität assoziiert. Alter und Volumen sind Scorekomponenten. Das Abstract belegt nicht, dass eine isolierte Punktzahl eine Therapieentscheidung oder endgültige individuelle Prognose rechtfertigt.

## Referenzen

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
