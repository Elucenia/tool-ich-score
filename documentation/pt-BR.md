<!-- ELUCENIA technical documentation · ich-score · pt-BR · no clinical/professional/rights approval -->

# ICH Score

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/ich-score)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Escala de coma de Glasgow

`gcs`

- `0` — 13 a 15
- `1` — 5 a 12
- `2` — 3 a 4

### Volume do hematoma ≥ 30 mL (fórmula ABC/2)

`vol`

### Inundação ventricular

`ivh`

### Origem infratentorial

`infra`

### Idade ≥ 80 anos

`idade`

## Edição do método

ICH/Hemphill 2001:5 fatores, total 0–6; volume ABC/2; sem decisão terapêutica automática

## Fórmula documentada

Glasgow 3 a 4 = 2 · 5 a 12 = 1 · 13 a 15 = 0; volume ≥ 30 mL = 1; inundação ventricular = 1; origem infratentorial = 1; idade ≥ 80 anos = 1. Total: 0 a 6.

Volume pela fórmula ABC/2: A = maior diâmetro do hematoma no corte de maior área; B = diâmetro perpendicular a A; C = número de cortes com hematoma × espessura do corte (em cm). Resultado em mL.

## Limites e população

Estimativa de gravidade na apresentação de hemorragia intracerebral, associada à mortalidade em 30 dias na coorte original. Idade e volume são componentes do escore. O resumo não demonstra que uma pontuação isolada justifique decisão terapêutica ou prognóstico individual definitivo.

## Referências

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Mortalidade em 30 dias: 0%


### 2

Mortalidade em 30 dias: 26%


### 3

Mortalidade em 30 dias: 97%

