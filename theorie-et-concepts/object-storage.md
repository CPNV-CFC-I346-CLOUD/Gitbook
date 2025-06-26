# Object Storage

## Introduction

Ce document est un résumé des recherches effectuées par les étudiants. Il condense en trois paragraphe les termes et explications découlant de leur travail de découverte du concept d'"Object Storage".

## Stockage objet - les principes

L’object storage est une architecture de stockage conçue pour gérer d’énormes volumes de données de manière efficace et flexible. Contrairement au <mark style="color:orange;">stockage par bloc</mark>, où les fichiers sont découpés en blocs gérés par un système de fichiers classique, le stockage objet stocke les données sous forme d’objets indépendants.&#x20;

### Un objet

Chaque objet est identifié par:

* un id unique,&#x20;
* accompagné de metadata (informations descriptives comme la date de création, le type de fichier, etc.) et,
* des data elles-mêmes.&#x20;

Cette approche facilite l’organisation et la recherche des fichiers tout en optimisant l’évolutivité et la durabilité des données.

### Mise à l'échelle

L’un des principaux avantages du stockage objet est <mark style="color:orange;">sa mise à l'échelle horizontale</mark>. Contrairement aux systèmes traditionnels qui ajoutent des ressources à un serveur centralisé (mise à l’échelle verticale), ici, les données sont réparties sur plusieurs serveurs ou nœuds, permettant d’augmenter la capacité de stockage de manière quasi illimitée.&#x20;

### Accès

L’accès aux objets se fait généralement via HTTP et des API REST, ce qui facilite leur utilisation par des applications cloud et favorise une intégration fluide avec divers services.

### Cas d'utilisation

Ce type de stockage est particulièrement utilisé pour créer des buckets S3, une technologie popularisée par Amazon Web Services (AWS), qui permet d’organiser les objets de manière efficace. Il est également idéal pour des usages comme le data lake, un système de stockage massivement scalable conçu pour conserver de grandes quantités de données brutes en format natif.

Contrairement à un stockage linéaire, où les fichiers sont enregistrés de manière séquentielle, l’object storage permet un accès direct et distribué aux données, rendant les recherches et analyses plus rapides et adaptées aux besoins modernes du <mark style="color:orange;">Big Data</mark> et de l’<mark style="color:orange;">intelligence artificielle</mark>.

