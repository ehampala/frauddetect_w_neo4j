# Projet 1 : Détection de fraude par l’analyse de graphes sur des transactions financières

**Réalisé par : Axel & Pascal**  
**Encadrant : [Dr DJEKI]**  
**Date : [May 22, 2025]**

---

## 1. Introduction

Dans un contexte où les fraudes financières deviennent de plus en plus complexes et interconnectées, les approches traditionnelles basées sur des règles statistiques atteignent leurs limites. Ce projet vise à exploiter les bases de données orientées graphe, notamment Neo4j, afin d’analyser les transactions financières et d’identifier des comportements suspects.

---

## 2. Modélisation du graphe

### Nœuds :
- `Client`
- `Compte`
- `Transaction`
- `Marchand`

### Relations :
- `(Client)-[:POSSEDE]->(Compte)`
- `(Compte)-[:REALISE]->(Transaction)`
- `(Transaction)-[:VERS]->(Marchand)`

![Schéma de modélisation du graphe](lien_image_ou_capture_schema)

---

## 3. Données utilisées

- Format : *.dump
- Nombre total de clients : …
- Nombre de transactions : …
- Méthode d’importation : `LOAD CSV WITH HEADERS FROM 'file:///transactions.csv'`

Exemple de structure :
