<!-- ELUCENIA technical documentation · ich-score · fr · no clinical/professional/rights approval -->

# Score ICH

[conditions, sources et autorisations](https://elucenia.org/fr/outils/ich-score)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Échelle de coma de Glasgow

`gcs`

- `0` — 13 à 15
- `1` — 5 à 12
- `2` — 3 à 4

### Volume de l’hématome ≥ 30 mL (formule ABC/2)

`vol`

### Hémorragie intraventriculaire

`ivh`

### Origine infratentorielle

`infra`

### Âge ≥ 80 ans

`idade`

## Édition de la méthode

ICH/Hemphill 2001 : 5 facteurs, total 0–6 ; volume ABC/2 ; pas de décision thérapeutique automatique

## Formule documentée

Glasgow 3 à 4 = 2 · 5 à 12 = 1 · 13 à 15 = 0 ; volume ≥ 30 mL = 1 ; extension ventriculaire = 1 ; origine infratentorielle = 1 ; âge ≥ 80 ans = 1. Total : 0 à 6.

Volume par ABC/2 : A = plus grand diamètre sur la coupe de plus grande surface ; B = diamètre perpendiculaire à A ; C = nombre de coupes avec hématome × épaisseur (cm). Résultat mL.

## Limites et population

Estimation de la sévérité à la présentation d’une hémorragie intracérébrale, associée à la mortalité à 30 jours dans la cohorte originale. L’âge et le volume sont des composants du score. Le résumé ne démontre pas qu’un score seul justifie une décision thérapeutique ou un pronostic individuel définitif.

## Références

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Mortalité à 30 jours : 0%


### 2

Mortalité à 30 jours : 26%


### 3

Mortalité à 30 jours : 97%

