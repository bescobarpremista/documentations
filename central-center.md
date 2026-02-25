# Insertion Leads sur Central center
## À la création

Il faut passer par l'url

```
https://financial.centralfinances.fr/Services/Service_Financial.php
```
ou pour test:
```
https://test.centralfinances.fr/Services/Service_Financial.php
```

Les données doivent être envoyé dans le body sous format texte de telle manière que le contenue ressemble à:

```
dossier_financial={"data":"data"}
```

Les données pouvant être présentes sont:

| Nom du champ | Format | Utilité | Statut |
| :--- | :--- | :--- | :--- |
| **civ_vous** | STRING | Civlité. Monsieur = Mr, Madame = Mme | *Optionnel* |
| **nom_vous** | STRING | Nom de la lead | **Obligatoire** |
| **prenom_vous** | STRING | Prénom de la lead | *Optionnel* |
| **date_naissance** | STRING | Date de naissance de la lead | **Obligatoire** |
| **situations** | INT | Situation familiale: 1 = Célbataire, 2 = Marié, 3 = Pacsés, 4 = Veuf, 5 = concubins, 6 = separe, 7 = divorcé | *Optionnel* |
| **jour_vous** | STRING | Jour de naissance de la lead | *Optionnel* |
| **mois_vous** | STRING | Mois de naissance de la lead | *Optionnel* |
| **annee_vous** | STRING | Année de naissance de la lead | *Optionnel* |
| **tel1** | STRING | Numéro de téléphone de la lead | **Obligatoire** |
| **mail** | STRING | Adresse mail de la lead | **Obligatoire** |
| **cp** | STRING | Code postal de la lead | *Optionnel* |
| **ville** | STRING | Ville de la lead | *Optionnel* |
| **adresse** | STRING | Adresse de la lead | *Optionnel* |
| **fonciers** | INT | Taxe foncier | *Optionnel* |
| **aide_logement** | INT | Aide au logement reçu | *Optionnel* |
| **pensions** | INT | Pension (versée ou reçue) | *Optionnel* |
| **profession** | STRING | Profession de la lead| *Optionnel* |
| **profession_vous** | STRING | Profession de la lead, si aucune 'n/a' | *Optionnel* |
| **revenu_vous** | INT | Revenu de la lead | **Obligatoire** |
| **logement** | STRING | Type de logement - doit être 'proprietaire', 'locataire' ou 'hebergement' | *Optionnel* |
| **proprietaire** | BOOLEEN | true lead propriétaire | **Obligatoire** |
| **locataire** | BOOLEEN | true si lead locataire | **Obligatoire** |
| **hebergement_gratuit** | BOOLEEN | true si lead hébergée gratuitement | **Obligatoire** |
| **loyer** | INT | Loyer de la lead, default: 1 | **Obligatoire** |
| **autres_charges** | INT | Autres charges de la lead | *Optionnel* |
| **charges** | INT | Charges de la lead | *Optionnel* |
| **nb_conso** | INT | Nombre de prêts conso | *Optionnel* |
| **nb_immo** | INT | Nombre de prêts immo | *Optionnel* |
| **type_credit** | ARRAY | Si prêt conso présent on ajoute 'Prêt personnel' (en premier), si prêt immo présent on ajoute 'Prêt Immobilier' | *Optionnel* |
| **mensualite** | ARRAY | Tableau des mensualités, conso en premier et immo en second | *Optionnel* |
| **crd** | ARRAY | Tableau des CRD, les crd conso en premier et immo en second | *Optionnel*|
| **montant_souhaite** | INT | Montant de trésorerie souhaité | *Optionnel* |
| **securecode** | STRING | Code de sécurité anti spam | **Obligatoire** |
| **src** | STRING | SRC de la lead | **Obligatoire** |
| ed | STRING | Identifiants de campagne | *Optionnel* |
| gclid | STRING | Google Click ID | *Optionnel* |
| **bdf** | STRING | Si la lead est fichée à la Banque de France: 'oui' ou 'non' | *Optionnel* |
| **cnf** | STRING | Domaine pour central center | **Obligatoire** |
| **formulaire** | STRING | Nom du formulaire | *Optionnel* |
| **url** | STRING | Lien de la lead | *Optionnel* |
| **acc_finalite** | BOOLEEN | --- | *Optionnel* |
| **acc_noemailing** | BOOLEEN | --- | *Optionnel* |
| **prospect_sms** | BOOLEEN | TRUE si accepte recevoir SMS | *Optionnel* |
| **emailing** | BOOLEEN | TRUE si accepte recevoir MAIL | *Optionnel* |
| **assurance_optin** | BOOLEEN | TRUE si accepte recevoir offre assurance | *Optionnel* |
| **financement_optin** | BOOLEEN | TRUE si accepte recevoir offre financement | *Optionnel* |
| **acc_partenaires** | BOOLEEN | TRUE si accepte recevoir offre partenaires | *Optionnel* |
| **remarque_commerciale** | STRING | Informations supplémentaires qui apparaîtront dans le champ remarque commerciale | *Optionnel* |

Pour le cnf, nous utilisons: 'centralfinances.fr'.

Pour le secure code nous le créons comme suit:

```php
md5(date("Y-m-d") . "ANTISPAM")
```
