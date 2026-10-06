<!-- ELUCENIA technical documentation · ich-score · it · no clinical/professional/rights approval -->

# Punteggio ICH

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/ich-score)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Scala del coma di Glasgow

`gcs`

- `0` — 13 a 15
- `1` — 5 a 12
- `2` — 3 a 4

### Volume dell’ematoma ≥ 30 mL (formula ABC/2)

`vol`

### Emorragia intraventricolare

`ivh`

### Origine infratentoriale

`infra`

### Età ≥ 80 anni

`idade`

## Edizione del metodo

ICH/Hemphill 2001: 5 fattori, totale 0–6; volume ABC/2; nessuna decisione terapeutica automatica

## Formula documentata

Glasgow 3–4 = 2 · 5–12 = 1 · 13–15 = 0; volume ≥ 30 mL = 1; estensione ventricolare = 1; origine infratentoriale = 1; età ≥ 80 anni = 1. Totale: 0–6.

Volume con ABC/2: A = diametro massimo nella sezione di area maggiore; B = diametro perpendicolare ad A; C = numero sezioni con ematoma × spessore (cm). Risultato mL.

## Limiti e popolazione

Stima della gravità alla presentazione di un’emorragia intracerebrale, associata alla mortalità a 30 giorni nella coorte originale. Età e volume sono componenti del punteggio. L’abstract non dimostra che un punteggio da solo giustifichi una decisione terapeutica o una prognosi individuale definitiva.

## Riferimenti

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Mortalità a 30 giorni: 0%


### 2

Mortalità a 30 giorni: 26%


### 3

Mortalità a 30 giorni: 97%

