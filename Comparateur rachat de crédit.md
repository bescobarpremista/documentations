# Comparateur rachat de crédit

Cet outil est intégré en iFrame et n’est pas gérer par nous.

## Données en entrées


| Nom                                      | Format | Utilité                                                     | Statut                                            |
| ---------------------------------------- | ------ | ----------------------------------------------------------- | ------------------------------------------------- |
| Type de projet                           | STRING | Choix entre: Travaux - auto - Trésorerie - Achat Immobilier | **Obligatoire**                                   |
| Montant du projet                        | INT    | Montant du projet                                           | **Obligatoire**                                   |
| Nombre emprunteur                        | STRING | Seul ou a deux                                              | **Obligatoire**                                   |
| Nombre d'enfants                         | INT    | Nombre d'enfant                                             | **Obligatoire**                                   |
| Segment                                  | STRING | Locataire ou propriétaire                                   | **Obligatoire**                                   |
| Loyer                                    | INT    | Loyer si locataore                                          | **Obligatoire si locataire**                      |
| Age emprunteur                           | INT    |                                                        | **Obligatoire**                                   |
| Age co emprunteur                        | INT    |                                                        | **Obligatoire si co emprunteur**                  |
| Revenu emprunteur                        | INT    |                                                        | **Obligatoire**                                   |
| Nombre mois                              | INT    | Nombre de mois de salaire                                   | **Obligatoire**                                   |
| Revenu co emprunteur                     | INT    |                                                        | **Obligatoire si co emprunteur**                  |
| Nombre mois co emprunteur                | INT    | Nombre de mois de salaire                                   | **Obligatoire si co emprunteur**                  |
| Autre revenu                             | INT    |                                                        | Optionnel                                         |
| Nombre mois autre revenu                 | INT    | Nombre de mois pour les autres revenu                       | **Obligatoire si autre revenu**                   |
| Somme mensualité crédit immobilier       | INT    |                                                        | Optionnel                                         |
| Montant à rembourser crédit immobilier   | INT    |                                                        | **Obligatoire si mensualité crédit immobilier**   |
| Somme mensualité crédit consommation     | INT    |                                                        | Optionnel                                         |
| Montant à rembourser crédit consommation | INT    |                                                        | **Obligatoire si mensualité crédit consommation** |


## Données en sortie

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1773046261.png)

Comme vu sur le screen, le retour contient trois offres avec ces données:


| Nom                            | Format   | Utilité |
| ------------------------------ | -------- | ------- |
| Montant du nouveau projet      | INT      |    |
| Montant crédit en cours        | INT      |    |
| Montant emprunté               | INT      |    |
| Durée nouveau financement      | INT      |    |
| Nouvelle mensualité            | INT      |    |
| Mensualités en cours           | INT      |    |
| Mensualités totales            | INT      |    |
| Revenu                         | INT      |    |
| Reste a vivre après finacement | INT      |    |
| Endettement après financement  | POURCENT |    |


 