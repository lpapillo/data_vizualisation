# Data Visualisation
Mini-projet réalisé dans le cadre d'**IGR204 - Visualization** (Telecom Paris), par Ramzi Khalifa, Alexandre Le Bris, Pierrick Leroy, Léa Papillon et Yann Rodriguez.


L'objectif du projet est de concevoir et d'implémenter trois visualisations d'un jeu de données retraçant le nombre d'attribution de prénoms de bébé, par année et par département, entre 1900 et 2019.
Chacune des visualisation devait permettre de répondre un ensemble de questions : 
- **Visualisation 1 :** Comment évoluent les prénoms au cours du temps ? Existe-t-il des prénoms qui sont restés populaires, ou impopulaires ? Certains sont-ils soudainement / brièvement devenus populaires ou impopulaires ?
- **Visualisation 2 :** Y a-t-il un effet régional sur les prénoms ? Certains prénoms sont-ils davantage populaires dans certaines régions ? Les noms populaires sont-ils généralement populaires dans tout le pays ?
- **Visualisation 3 (bonus) :** Y a-t-il des effets de genre dans les données ? La popularité des noms donnés aux deux sexes évolue-t-elle de manière cohérente ?

La première visualisation est un graphe intéractif, affichant les courbes d'évolution du nombre d'attribution par prénom et par année (à l'échelle nationale), entre 1900 et 2019. Des boutons permettent de sélectionner une plage de dates, de filtrer sur la forme du nom (première lettre, dernière lettre...), sa popularité, son origine... Tous ces critères permettent d'identifier les prénoms qui correspondent aux questions posées pour la visualisation 1. On observe par exemple que les prénoms féminins Emma et Louise sont de plus en plus populaires (après avoir été moins utilisé pendant un moment), de même que Gabriel et Nathan pour les garçons. Inversement, certains prénoms ont été très propulaires et ne sont plus très utilisés (Isabelle, Michel, Marcelle, Paule...), etc. Tous le prénoms sont globalement moins attribués avec le temps, car il y a une plus grande diversité de prénoms.

La deuxième visualisation est une carte de France qui indique le nombre de bébés qui portent un même nom, par région. Comme pour la première visualisation, des filtres permettent de sélectionner les critères qui répondent aux questions posées. La carte met clairement en avant un effet régional, car les prénoms ne sont pas répartis de manière homogène sur tout le territoire.

La troisième visualisation est moins interactive et dans un esprit ludique, prend le parti du dynamisme. Le temps est encodé sur l'axe des ordonnées et l'axe des abscisses présente un attribut dérivé, le pourcentage de mixité d'un prénom. Plus le prénom est à gauche, plus il est fréquemment donné à des femmes, plus il est à droite, plus il est masculin, le tout évoluant en fonction du temps.
Le fond du canva est rempli de courbes en gris clair qui représentent les 500 prénoms les plus donnés en france au siècle dernier. On peut déjà remarquer que la très grande majorité des prénoms sont 100% masculins ou 100% féminin la plupart du temps, ce qui est observable grace à la transparence de ces courbes et leur superposition aux extrémités. Sur cet arrière plan on vient représenter des "prénoms intéressants" sélectionnés par un algorithme paramétrable dans la cellule précédant la viz. Les courbes montent de bas en haut à mesure que les années avancent. La popularité de chaque prénom est encodée en utilisant la largeur de la ligne via une échelle logarithmique. Afin de jouer pleinement la carte du jeu, une part d'aléatoire est introduite dans l'algorithme et les prénoms représentés, relancer plusieurs fois la viz donne rarement le même résultat !


Autres fichiers:
- design : nos réflexions pour le design en amont de l'étape de codage
- visualization_3_exempleEtatFinal : au cas où l'animation ne tourne pas (réalisé sous colab) sur un autre système, voici un état final (statique)
