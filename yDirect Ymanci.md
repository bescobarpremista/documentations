# yDirect Ymanci

La calculatrice yDirect est une calculatrice ayant pour but de facilement permettre à l’utilisateur d’avoir une estimation d’une opération de rachat de crédit.

Dans le cas ou le résultat de la simulation lui plait, il peut choisir d’être contacté en renseignant certaines informations de contact.

## Données en entrées - partie simulation


| Nom                                      | Format  | Utilité                                                                               | Statut                                            |
| ---------------------------------------- | ------- | ------------------------------------------------------------------------------------- | ------------------------------------------------- |
| Segment                                  | STRING  | Propriétaire - Locataire - Hébergé gratuitement                                       | **Obligatoire**                                   |
| Revenu                                   | INT     | Revenu mensuel net du foyer.                                                          | **Obligatoire**                                   |
| Trésorerie                               | INT     | Montant de trésorerie voulu. 0 par défaut.                                            | Optionnel                                         |
| Loyer                                    | INT     | Loyer de la personne. Le champs n’est que présent si le segment choisi est locataire. | **Obligatoire si segment est locataire**          |
| Charges                                  | INT     | Charges de la personne.                                                               | Optionnel                                         |
| Nombre crédit immobilier                 | INT     | Nombre de crédit immobilier. 0 par défaut.                                            | Optionnel                                         |
| Montant mensualité immobilier            | INT     | Montant de la mensualité des crédit immobilier.                                       | **Obligatoire si nombre crédit immobilier > 0**   |
| Montant immobilier restant a remboursé   | INT     | Montant totale des crédits immobiliers.                                               | **Obligatoire si nombre crédit immobilier > 0**   |
| Renégociation crédit immobilier          | BOOLÉEN | Si la personne veut inclure ses crédits immobiliers dans le calcul.                   | **Obligatoire si nombre crédit immobilier > 0**   |
| Nombre crédit consommation               | INT     | Nombre de crédit consommation. 0 par défaut.                                          | Optionnel                                         |
| Montant mensualité consommation          | INT     | Montant de la mensualité des crédits consommation.                                    | **Obligatoire si nombre crédit consommation > 0** |
| Montant consommation restant a remboursé | INT     | Montant totale des crédits consommation.                                              | **Obligatoire si nombre crédit consommation > 0** |


## Données en entrées - partie contact


| Nom              | Format              | Utilité                                         | Statut          |
| ---------------- | ------------------- | ----------------------------------------------- | --------------- |
| Civilité         | STRING              | Récupérer la civilité de la personne.           | **Obligatoire** |
| Nom              | STRING              | Nom de la personne.                             | **Obligatoire** |
| Prénom           | STRING              | Prénom de la personne.                          | **Obligatoire** |
| Date naissance   | STRING - JJ/MM/AAAA | Date de naissance de la personne.               | **Obligatoire** |
| Mail             | STRING              | Mail de la personne.                            | **Obligatoire** |
| Téléphone        | STRING              | Téléphone de la personne.                       | **Obligatoire** |
| Fichage bancaire | BOOLÉEN             | Si la personne est fiché à la banque de France. | **Obligatoire** |


## Données de retour

Le retour de la calculette se fait aprés remplissage des informations dans la partie simulation. Il est restitué les données de simulation avec une durée et la mensualité qui lui convient. La durée est entre 5 ans et soit 15, soit 25 soit 35 ans dépendant des données en entrées.

Les données de retours sont affichées pour mieux donner une idée de l’impact de l’opération pour le client avec toujours la plus petites mensualités possible et donc la plus longue durée d'emprunt.

Il y a en données restitué :

- La nouvelle mensualité
- La baisse de cout entre l’ancienne et la nouvelle mensualité
- La nouvelle durée d’emprunt ( possible de la changé pour explorer les différentes possibilités)
- Un graphique de la situation avant le rachat avec en affichage:
  - Le reste à vivre
  - Le loyer + les charges
  - La mensualité des crédits consommations
  - La mensualité des crédits immobiliers
- Un graphique de la situation aprés l’opération:
  - Le reste à vivre
  - Le loyer + les charges
  - La nouvelle mensualité
  - La mensualité immobilière si la renégociation n’est pas voulu

 

## Quelques captures

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772700954.png)

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772700995.png)

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772701015.png)

 