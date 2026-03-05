# Baromètre taux crédit immobilier

Le baromètre des taux de crédit immobilier fait partie du plugin "Premista Rate Barometer".

Il est possible de l’afficher avec le short code:

```markdown
[prb_immo] 
#Affiche le baromètre avec ses 3 blocs

[prb_immo showbarometer=false] 
L'option showbarometer permet d'afficher (true) ou non (false) le premier bloc. Default: true

[prb_immo showchart=false] 
L'option showchart permet d'afficher (true) ou non (false) le second bloc d'historique des taux. Default: true

[prb_immo  showcta=false] 
L'option showcta permet d'afficher (true) ou non (false) le troisième bloc des CTA. Default: true

[prb_immo hidecta=false] 
L'option hidecta permet de cacher(true) ou non (false) le bouton "je fais une demande" quand le scroll est sur le formulaire. Default: true
```

Les trois blocs vont être abordé à la suite.

## Premier bloc - Baromètre

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772721741.png)

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772721837.png)

Le premier bloc permet de voir le taux suivant la durée d’emprunt et la région métropole et DROM-COM

Les durées vont de 10 à 25 ans.

Les taux sont récupérer depuis Gandalf.

## Second bloc - Historique des taux

Le second bloc permet de voir l’évolution des taux de rachat de crédit sur une durée sélectionnable sur les boutons à droite.

Les données sont aujourd’hui stocké en JSON dans les fichiers de plugins.  

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772722311.png)

Le second bloc permet de voir l’évolution des taux de crédit immobilier sur une durée sélectionnable sur les boutons à droite ainsi que la zone.

Les données sont aujourd’hui stocké en JSON dans les fichiers de plugins.

## Troisième bloc - CTA

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772722693.png)

Le troisième bloc est un bloc CTA. 

- Estimer ma mensualité redirige vers la [calculette mensualité](https://ymanci.fr/credit-immobilier/outils/calculer-mensualites/)
- Faire une demande redirige vers le [formulaire immobilier](https://ymanci.fr/credit-immobilier/outils/demande-de-credit-immobilier/)

## Affichage des taux sous tableau

Il est possible d’afficher les taux sous simple tableau.

`[prc_rac_immo]`

Il est possible de modifier le caption du tableau comme suit:

`[prc_rac_table caption=’Nouvelle caption']`

La caption de base est « Tableau des taux de rachat de crédit - mis à jour le JJ Mois Année». Toutes caption sera suivi de « mis à jour le JJ Mois Année »

![](asset://localhost/%2FUsers%2Fbenjiesco%2FDocuments%2Fdocumentation%2Fdocs%2Fassets%2Fscreenshot-1772723283.png)

 