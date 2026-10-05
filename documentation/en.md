<!-- ELUCENIA technical documentation · ich-score · en · no clinical/professional/rights approval -->

# ICH Score

[conditions, sources and permissions](https://elucenia.org/en/tools/ich-score)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Glasgow Coma Scale

`gcs`

- `0` — 13 to 15
- `1` — 5 to 12
- `2` — 3 to 4

### Hematoma volume ≥ 30 mL (ABC/2 formula)

`vol`

### Intraventricular hemorrhage

`ivh`

### Infratentorial origin

`infra`

### Age ≥ 80 years

`idade`

## Method edition

ICH/Hemphill 2001: 5 factors, total 0–6; ABC/2 volume; no automatic treatment decision

## Documented formula

Glasgow 3 to 4 = 2 · 5 to 12 = 1 · 13 to 15 = 0; volume ≥ 30 mL = 1; intraventricular extension = 1; infratentorial origin = 1; age ≥ 80 years = 1. Total: 0 to 6.

Volume by ABC/2: A = longest haematoma diameter on the largest-area slice; B = diameter perpendicular to A; C = number of slices with haematoma × slice thickness (cm). Result in mL.

## Limits and population

An estimate of severity at intracerebral hemorrhage presentation, associated with 30-day mortality in the original cohort. Age and volume are components of the score. The abstract does not demonstrate that a score alone justifies a therapeutic decision or definitive individual prognosis.

## References

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
