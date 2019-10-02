L'une des grandes joies de la vie professionnelle, ce sont ces surprises qui savent vopus attendre alors que vous avez du retard suite à divers incidents sur votre ligne de métro.
Aujourd'hui, c'est un sachet de chouquettes délicieusement offertes par une collègue.
J'en ai déjà pioché quelques unes, et me vient à l'esprit que les bouchées avalées se ressentiront sur ma ligne. 
Et dans le fol espoir d'estimer ma prise de poids, j'en viens à me demander quel est le poids moyen d'une chouquette de cette enseigne parisienne ?

Le meilleur moyen d'avoir la réponse serait de peser toutes les chouquettes du magasin et d'ensuite calculer le poids moyen. 
Ce que je ne vais pas faire pour lutter contre le gaspillage alimentaire, et un peu par limitation budgétaire également.
Je n'aurai donc pas accès au poids moyen exact, mais je peux essayer de l'estimer en récupérant des chouquettes. 
C'est exactement ce à quoi servent les statistiques : estimer une grandeur à partir d'un échantillon de la population qui nous intéresse (ici, les chouquette de cette pâtisserie).

Tout de suite, ce qu'on a très envie de faire, c'est estimer la moyenne de la population (toutes les chouquettes de cette maison) par la moyenne de mon échantillon (les chouquettes qui restent dans le sachet).
Mais est-ce une bonne idée ? Pour répondre à cette question, je vous propose de créer une population de chouquettes fictives, de poids moyen 12g, et de prendre des échantillons aléatoirement
pour voir comment se comporte leur moyenne.

Commençons par imaginer une population de 5 chouquettes, de poids : 12g, 13g, 12g, 11g,10g , 14g. Si je prends des échantillons de 2 chouquettes,
je peux avoir par exemple : une chouquette de 13g et une chouqette de 10g, soit une moyenne de 11,5 g. Quelques combinaisons sont répertoriées dans le tableau suivant :

| Chouquette 1 | Chouquette 2 | Moyenne |
|--------------|--------------|---------|
| 13 | 10 | 11.5 |
| 12 | 11 | 11.5 |
| 12 | 13 | 12.5 |
| 12 | 14 | 13 |
| 10 | 11 | 10.5 |

Avec ce petit exemple, il semble que généralement l'estimation ne tombe pas très loin de la vraie valeur.Mais est-ce que je n'ai pas juste pris les exemples qui allaient bien ?
Ou alors j'aurais eu de la chance ? Je vous propose de créer une population plus grande, disons 500 000 chouquettes, et de faire de nombreux échantillonnages pour voir
comment les moyennes des échantillons se comportent.

![distribution pop](figures/population_distribution.png?raw=true)

Voila donc la distribution des poids de ma population de 500 000 chouquettes. En abscisse on voit le poids et en ordonné la proportion de chouquettes qui pèsent autant.
Toutes les chouquettes ne font pas précisément 12g parce que les pâtissiers ne font pas toujours les mêmes gestes.


Comme il reste pour le moment 20 chouquettes dans le sachet, je vous propose de tirer plusieurs échantillons (disons 50 000) de 20 chouquettes et de voir comment se comportent les moyennes.

![distribution moyenne 20](figures/means_20.png?raw=true)

Cette distribution ci est la distribution des moyennes de mes échantillons. C'est à dire qu'en abscisse, j'ai le poids moyen mesuré, et en ordonné j'ai la proportion d'échantillons qui présentent ce poids.
Les moyennes sont généralement assez proches de la vraie moyenne de la population. Mais parfois l'échantillon s'en éloigne un peu.
On peut donc dire que j'ai de bonnes chances d'avoir une bonne estimation de la moyenne.

Ou plutôt j'avais... Des collègues viennent de passer et de piocher à leur tour dans le sachet. Il reste donc 2 chouquettes. Est-ce que j'en ai assez pour estimer précisément le poids moyen ?
Je vous propose de recommencer plusieurs échantillonnages (toujours 50 000) mais de 2 chouquettes.

![distribution moyenne 2](figures/means_2.png?raw=true)

Voici donc la distribution des moyennes de mes nouveaux échantillons.
La plupart des échantillons sont encore assez proches de la vraie moyenne de la population. Mais la courbe est beaucoup plus "aplatie", ce qui veut dire que les échantillons
s'éloignent aussi beaucoup plus souvent et beaucoup plus de cette valeur. On peut donc dire que j'ai moins de chances d'avoir une bonne estimation de la moyenne, 
et il est même assez probable que je tombe un peu loin.


Alors bien sûr, la notion de précision est subjective, peut-être que vous trouviez déjà qu'avec 20 chouquettes, j'avais tendance à tomber trop loin. 
Et dans ce cas, vous auriez en fait préféré que j'en échantillonne plus, puisque manifestement plus l'échantillon est grand et plus on tombe prés de la vraie valeur.
Et ce n'est pas une impression, la moyenne a cette propriété que plus l'échantillon est grand, plus elle va converger vers la valeur qui nous intéresse : celle de la population. 
C'est une des raisons pour lesquelles la moyenne est très utilisée.

Bref, qu'en est-il du poids de ces chouquettes ? Eh bien, je ne sais pas. Parce qu'il n'en reste plus.
Ce qui veut dire que nous avons appris 3 choses importantes :
 - les statistiques servent à estimer des valeurs quand nous n'avons pas accès à notre population d'intérêt
 - la moyenne d'un échantillon est un bon estimateur qui va être de plus en plus précis à mesure que la taille de l'échantillon augmente (la "bonne" taille d'échantillon est donc celle qui correspond à une précision suffisante)
 - un paquet de chouquette dure moins longtemps que ce qu'il faut pour écrire ce genre d'article de blog.