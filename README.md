# Projet_3_udacity 
# Jeu de Données sur les prets de Prosper



## Dataset
Les banques receuillent beaucoup de données consernant leur utilsateur avant de leur delivré un pret.
Dans ce context on va etudier un [dataset](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv%26amp;sa%3DD%26amp;ust%3D1581581520570000&sa=D&source=editors&ust=1659905511742826&usg=AOvVaw3ThKJ5Dc5EHpAfo4vO9yGa) contenant des informations sur les prets banquaires de 113937 personnes avec 81 variables dont:
1. LoanStatus : Status actuel du pret
2. BorrowerRate : Taux d'interet de l'emprunteur pour ce pret 
3. StatedMonthlyIncome : Revenu mensuel declaré par l'emprunteur
4. Term: La durée du pret exprimée en mois 
5. ProsperRating(Alpha) : La note Prosper attribuée au moment de la creation de la liste entre AA et HR
6. EmploymentStatus : Le statu d'emploi de l'emprunteur au moment ou il a créé la liste
7. LoanOriginalAmount : Montant initial du pret

8. ProsperScore : Un score de risque personnalisé construit a partir des données historiques de Prosper . Le score va de 1 a 10 ,10  etant le meilleur ou le plus faible score de risque
9. BorrowerAPR : le taux annuel effectif global(TAEG) de l'emprunteur pour le pret. 
10. ListingCategory : La categorie de l'annonce que l'emprunteur a selectionnée lors de la publication de son annonce 
11. EmploymentStatusDuration : La durée en mois du statut d'emploi au moment de la creation de la fiche  
12. IsBorrowerHomeowner Un emprunteur sera classe comme proprietaire s'il a un pret hypothecaire dans son profil de credit ou s'il fournit des documents confirmant qu'il est proprietaire
13. Occupation : La profession choisie par l'emprunteur au moment ou il a créé la liste
14. CurrentCreditLines : Nombre de lignes de credit en cours au moment ou le profil de credit a ete etabli

etc..... 

Pour notre etude on va se focaliser sur ses variables listé ici pour les besoin de notre analyse



## Résumé des conclusions

Au cours de l'exploration j'ai constaté que la distribution de la variable le taux annuel effectif global(TAEG) presenté beaucoup de pic et qu'il existait une relation entre le taux annuel effectif global(TAEG) et le montant du pret avec la duree du pret .
Le taux les plus elevé correspond en genreale au montant les plus faible ce qui s'explique par la correlation negative entre les deux variables.
La variable ProsperRating(Alpha) qui correspond a la note Prosper attribuée au moment de la creation de la liste entre AA et HR on constate que pour les personnes
avec la valeur AA ont des TAEG plus faible .
Et le status de l'emprunteur aussi joue sur le taux .
On constate aussi que la statue du demandeur joue sur le taux les personnes avec une statue other et not employed ont des taux (TAEG) sont plus elevé.
On peut voir que la durée du pres plus elle est importante plus le montant du pres initiale est elevé.
Et le ProsperRating (Alpha) la duree la plus representer dans les classes est de 36 mois.

J'ai aussi regardé les variables qui influencie le score personnalisé que la banque donne au demandeur sont la durée du pret et le nombre de lignes de credit .
En dehors des variable d'intérét j'ai verifié que les montants le plus eleve corresponds au durée les plus long.

### Principaux éléments de la présentation

Pour la presentation je vais  commencer  par la distribution des variables taux  , le montant initial du pret et la durée du pret.
Ensuite j'introduit le ProsperRating (Alpha) et le score personnalisé de la personne et la relation entre le temps et le montant initiale du pret je vais utiliser un boxplot pour visualiser cette relation car c'est plus facile de comparer le temps avec un boxplot.
Apres a l'aide d'un diagramme en point je visualise la relation entre le taux le ProsperRating (Alpha) et la durée du pret.
Enfin je vais presentation la correlation negative entre le taux et le montant du prets a l'aide d'un nuage de point je vais utiliser le parametre alpha pour voir la ou les point sont plus centré.
