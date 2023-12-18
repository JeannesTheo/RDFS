## Sommaire avec les contraintes

### Caractéristiques des personnes

Toutes les personnes ont un nom, et au moins un prénom. \
Les poids sont entre 0 et 250 kilos. \
Le sexe d'un patient est forcément Homme, Femme ou Autre.

Les patients 1, 2 et 3 ne respectent pas les contraintes, alors que le patient 4 est valide.

### Numéros de sécurité sociale

Tous les patients ont exactement un seul numéro de sécurité sociale, qui est une chaine de caractères composée
d'exactement 13 chiffres.

Le patient 1 respecte ces restrictions alors que les patients 2,3 et 4 comportent des violations.

### Informations sur les problèmes médicaux

Les problèmes médicaux doivent avoir une date de diagnostic qui est un littéral, et désigne au moins un problème de
santé. Cette
maladie doit être représentée à l'aide d'une ressource définie dans NCIT. Le problème médical ne peut pas avoir une date
supérieure à 2023.

Les deux premiers problèmes médicaux dans les données ne respectent pas les contraintes, alors que la dernière est
valide.

### Un médecin ne peut pas être son propre patient.

Les suivis médicaux doivent avoir un champ 'Statut du patient' qui peut être rempli en anglais ou en français. Il doit
être rempli au moins une fois et ne pas avoir deux commentaires dans la même langue.
Un indicateur de la santé du patient doit également être présent sous forme de booléen.

Les rapports médicaux doivent être écrits par une personne avec un numéro de docteur. Il doit y avoir exactement 2 noms
de familles dans les gens concernés par le rapport, un pour le patient et un pour le médecin.

Follow-up1 est correct, tandis que les autres ne respectent pas les contraintes. Le Case Report 1 est valide, alors que
le Case report 2 viole les contraintes établit par SHACL.