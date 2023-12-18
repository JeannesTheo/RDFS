Pour valider que les médecins et les personnes sont considérées comme des personnes :
```sparql
select * where {
    ?x a s:Person
}
```
Trouver les frères et sœurs dans le graphe :
```sparql
select * where {
    ?x s:sibling ?y
}
```
Trouver les gens qui sont liés de facon indirect :
```sparql
select * where {
    ?x s:notDirectlyRelated ?y
}
```
Trouver tous les ascendants du patient 6 :
```sparql
select * where {
    :Patient6 s:hasAscendant ?x
}
```
Tous les problèmes médicaux qui sont traités avec autre chose que des médicaments :
```sparql
select * where {
    ?x a s:AlternativesTreatmentCaseReport
}
```



