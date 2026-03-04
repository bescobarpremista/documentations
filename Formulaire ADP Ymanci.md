# Formulaire ADP Ymanci

Le formulaire ADP a besoin du JavaScript. Il est responsive entre desktop et mobile.

Il envoie ses données a Gandalf qui les traites puis les transmet a MyComparateur puis restitue la réponse de MyComparateur et un lien Calizy.

## Données en entrées


| Nom                             | Type                                                                         |
| ------------------------------- | ---------------------------------------------------------------------------- |
| Type de projet                  | Changer d’assurance ou Assurer un nouveau prêt                               |
| Nombre de personne              | 1 ou 2                                                                       |
| Objet du prêt                   | Résidence principale - Investissement locatif - Résidence secondaire - autre |
| Souscription à la banque        | Oui - non                                                                    |
| Mensualité assurance            | Mensualité ou vide                                                           |
| Type de prêt                    | Prêt immobilier classique - Prêt relais - Prêt à taux zéro                   |
| Montant initial du prêt         | INT                                                                          |
| Durée du prêt                   | INT                                                                          |
| Taux du prêt                    | Float                                                                        |
| Année de la première mensualité | Date JJ/MM/AAAA                                                              |
| Banque prêteuse                 | Liste de banque prêteuse voir plus bas                                       |
| Civilité                        | `0 Monsieur - 1 Madame`                                                      |
| Nom                             | String                                                                       |
| Prénom                          | String                                                                       |
| Date naissance                  | Date JJ/MM/AAAA                                                              |
| mail                            | String                                                                       |
| Téléphone                       | String                                                                       |
| Fume                            | OUI - NON                                                                    |
| Profession                      | Liste de métier voir plus bas                                                |
| Commentaire                     | Texte                                                                        |
| RGPD                            | Booléen                                                                      |
| Contact partenaires             | Booléen                                                                      |



| Job                         |
| --------------------------- |
| Salarié Cadre               |
| Salarié Non Cadre           |
| Artisan                     |
| Commerçant                  |
| Fonctionnaire non cadre     |
| Auxiliaire médical          |
| Paramédical                 |
| Dentiste                    |
| Pharmacien                  |
| Médecin Chirurgien          |
| Dirigeant entreprise        |
| Expl. Agricole              |
| Sans profession             |
| Profession libérale         |
| Intermittent                |
| Fonctionnaire cadre         |
| Retraite Cadre              |
| Salarié Non Cadre Tertiaire |



| Banque                    |
| ------------------------- |
| Axa                       |
| Banque Populaire          |
| La banque postale         |
| BNP Paribas               |
| BRED                      |
| Caisse d'épargne          |
| Caisse agricole           |
| Crédit mutuel de bretagne |
| Boursobank                |
| CIC                       |
| Crédit mutuel             |
| Société générale          |
| LCL                       |
| Autres                    |


## Données en sorties


| Nom            | Type de données                                                         |
| -------------- | ----------------------------------------------------------------------- |
| URL RDV        | Lien pour prendre rdv                                                   |
| Liste d'offres | Chaque offre contient :- Assureur- Cout moyen/an- Garanties de l'offre |


 