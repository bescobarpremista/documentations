# Baromètre taux rachat de crédit

Le baromètre des taux de rachat de crédit fait partie du plugin "Premista Rate Barometer".

Il est possible de l’afficher avec le short code:

```markdown
[prb_rac] 
#Affiche le baromètre avec ses 3 blocs

[prb_rac showbarometer=false] 
L'option showbarometer permet d'afficher (true) ou non (false) le premier bloc. Default: true

[prb_rac showchart=false] 
L'option showchart permet d'afficher (true) ou non (false) le second bloc d'historique des taux. Default: true

[prb_rac showcta=false] 
L'option showcta permet d'afficher (true) ou non (false) le troisième bloc des CTA. Default: true

[prb_rac hidecta=false] 
L'option hidecta permet de cacher(true) ou non (false) le bouton "je fais une demande" quand le scroll est sur le formulaire. Default: true
```

Les trois blocs vont être abordé à la suite.

## Premier bloc - Baromètre

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772716303.png)

Le premier bloc permet de voir le taux suivant la durée d’emprunt et le statut de la personne.

Les durées pour le **locataire** vont de 3 à 15 ans.

Les durées pour le **propriétaires** vont de 5 à 35 ans. A partir de 20 ans on fait des bons de 5 ans.

Les taux sont récupérer depuis Gandalf.

## Second bloc - Historique des taux

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772716672.png)

Le second bloc permet de voir l’évolution des taux de rachat de crédit sur une durée sélectionnable sur les boutons à droite.

Les données sont aujourd’hui stocké en JSON dans les fichiers de plugins.

## Troisième bloc - CTA

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772717023.png)

Le troisième bloc est un bloc CTA. 

- Estimer ma mensualité redirige vers la [yDirect.](https://ymanci.fr/regroupement-credits/outils/simulation-allegement-mensualite/)
- Faire une demande redirige vers le [Cleverform](https://ymanci.fr/regroupement-credits/outils/demande-rachat-de-credit-en-ligne-rapide/)

## Affichage des taux sous tableau

Il est possible d’afficher les taux sous simple tableau.

Pour les taux locataire:

`[prc_rac_table type='tenant']`

Pour les taux propriétaires:

`[prc_rac_table type=‘owner']`

Il est possible de modifier le caption du tableau comme suit:

`[prc_rac_table type=‘tenant’ caption=’Nouvelle caption']`

La caption de base est « Tableau des taux de rachat de crédit - mis à jour le JJ Mois Année»

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772723185.png)

 