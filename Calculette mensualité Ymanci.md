# Calculette mensualité Ymanci

La calculette mensualité Ymanci à pour but de p[ermettre aux utilisateur de simuler facilement un crédit immobilier en changeant rapidement et simplement les paramètres du crédit.

## Données en entrées


| Nom              | Format | Utilité                  | Statut          |
| ---------------- | ------ | ------------------------ | --------------- |
| Montant emprunté | INT    | Montant du prêt          | **OBLIGATOIRE** |
| Durée            | INT    | Durée du prêt voulu      | **OBLIGATOIRE** |
| Taux d'intérêt   | FLOAT  | Taux d'intérêt du prêt   | **OBLIGATOIRE** |
| Taux d'assurance | FLOAT  | Taux d’assurance du prêt | **OBLIGATOIRE** |


## Données en sorties


| Nom                          | Format | Utilité                                                             |
| ---------------------------- | ------ | ------------------------------------------------------------------- |
| Mensualité                   | INT    | Mensualité suite à la simulation                                    |
| Prix assurance               | INT    | Prix de l’assurance suite à la simulation                           |
| Montant total à rembourser   | INT    | Montant total (montant + intérêt + assurance) suite à la simulation |
| Montant intérêts             | INT    | Montant des intérêts                                                |
| Montant assurances           | INT    | Montant du cout de l'assurance                                      |
| Mensualités (hors assurance) | INT    | Mensualité sans l'assurance                                         |
| Mensualités assurance        | INT    | Mensualité du prix de l'assurance                                   |
| Coût du crédit               | INT    | Cout                                                                |
| Coût assurance               | INT    |                                                                |
| Taux débiteur                | FLOAT  |                                                                |


Les données en sorties sur l’informations du prêt sont aussi donnée pour des durée différentes :  

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772715782.png)

## Quelques captures

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772715818.png)

 