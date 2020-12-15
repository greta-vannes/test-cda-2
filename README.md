# Triangle du miam

## Introduction

Des scientifiques du MIT viennent de trouver une loi très étrange qui permet de prédire les repas de ses étudiants plusieurs jours à l'avance et ainsi améliorer la gestion de ses stocks.

À chaque retour de vacances les étudiants font la liste des repas de la semaine en ayant le choix entre 🍣 (sushi) 🍕 (pizza) ou 🥦 (repas diététique)

Exemple de liste de la semaine (deux repas par jour pendant sept jours) :

🍣🍣🍕🍣🍕🥦🍕🥦🍣🍣🍕🍕🥦🍣 

En étudiant cette liste, des scientifiques se sont rendu compte qu'ils peuvent prédire les quatre vingt onze repas suivants de manière précise avec la théorie du Triangle du miam 👀...

## Spécifications

Chaque combinaison de deux repas permet de faire une prédiction comme ceci :
              

Combinaison  🍣 🍣   🍣 🍕   🍣 🥦   🍕 🥦
Prédiction    🍣      🥦      🍕     🍣

Les prédictions se font par lignes successives de taille Combinaisons précédentes - 1, ce qui donne naissance au fameux Triangle du miam.

En reprenant l'exemple précédent :

🍣 🍣 🍕 🍣 🍕 🥦 🍕 🥦 🍣 🍣 🍕 🍕 🥦 🍣
 🍣 🥦 🥦 🥦 🍣 🍣 🍣 🍕 🍣 🥦 🍕 🍣 🍕
  🍕 🥦 🥦 🍕 🍣 🍣 🥦 🥦 🍕 🍣 🥦 🥦
   🍣 🥦 🍣 🥦 🍣 🍕 🥦 🍣 🥦 🍕 🥦
    🍕 🍕 🍕 🍕 🥦 🍣 🍕 🍕 🍣 🍣
     🍕 🍕 🍕 🍣 🍕 🥦 🍕 🥦 🍣
      🍕 🍕 🥦 🥦 🍣 🍣 🍣 🍕
       🍕 🍣 🥦 🍕 🍣 🍣 🥦
        🥦 🍕 🍣 🥦 🍣 🍕
         🍣 🥦 🍕 🍕 🥦
          🍕 🍣 🍕 🍣
           🥦 🥦 🥦
            🥦 🥦
             🥦

Je suis donc en mesure de connaître les repas d'un étudiant à J+18, par exemple, en calculant les jours comme ceci (midi et soir):

 1 1  2 2  3 3  4 4   5 5  6 6  7 7
🍣 🍣 🍕 🍣 🍕 🥦 🍕 🥦 🍣 🍣 🍕 🍕 🥦 🍣
  8 8  9 9  1010 1111 1212  1313 14
 🍣 🥦 🥦 🥦 🍣 🍣 🍣 🍕 🍣 🥦 🍕 🍣 🍕
  14 1515 1616  1717 1818 ...
  🍕 🥦 🥦 🍕 🍣 🍣 🥦 🥦 🍕 🍣 🥦 🥦

À J+18, cet étudiant mangera 🥦 le midi et 🍕 le soir !

### But du jeu

À partir de ces informations, vous devez réaliser un petit programme qui vous retourne les repas de n'importe quel jour en fonction de la liste des repas de la semaine de départ.

![Exemple](./miam-1.png)



