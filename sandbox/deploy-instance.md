# Deploy Instance

## Intention prédagogique

En attendant que l'infrastructure soit disponible, vous débutez le travail d'analyse et de conception pour la suite du projet. Cela vous poussera à approfondir votre connaissance des différents composants nécessaire et d'identifier la bonne stratégie de déploiement.

## Pré-requis

Avoir réalisé la conception (labo précédent).

Les composants suivants vous serons livrés, vous n'avez donc pas besoin de les créer:

## Aspects géographiques

| Composants | Valeur       | Descriptif |
| ---------- | ------------ | ---------- |
| Region     | eu-central-1 | Frankfurt  |
| AZ         | 1a           |            |

## VPC

| Key        | Value                 |   |
| ---------- | --------------------- | - |
| ID         | vpc-0a22d771f16ae549d |   |
| CIDR Block | 10.0.0.0/16           |   |
| Name       | vpc-i346              |   |

## NAT

| Key         | Value               |   |
| ----------- | ------------------- | - |
| Instance ID | i-09d3919ca6d27ab6b |   |

* Region
* VPC
* IGW
* SubnetPublic
* SSH-SRV
* NAT

{% hint style="info" %}
Ne codez pas en "dure" les valeurs des paramètres, vos scripts doivent pouvoir déployer des infrastructures dont les noms, les identifiants changent.
{% endhint %}

## Objectifs opérationnels

Identifier les commandes ainsi que les paramètres nécessaires pour déployer <mark style="color:red;">et supprimer</mark>:

* [ ] Un sous-réseau privé
* [ ] Une instance EC2

{% hint style="warning" %}
Lorsqu'il est mentionné "XX" dans les valeurs, il s'agit du numéro de votre devopsteam.
{% endhint %}

## Subnet

Vous devez réussir à déployer un sous-réseau privé en respectant les contraintes suivantes:

| Key                    | Value                |
| ---------------------- | -------------------- |
| Subnet Name            | Subnet-DevopsteamXX  |
| Availability Zone      | eu-central-1a        |
| IPv4 subnet CIDR Block | 10.0.XX.0/28         |
| Tag name               | Subnet-DevopstreamXX |



| Key               | Value                                     |
| ----------------- | ----------------------------------------- |
| Route table Name  | RteTable-DevopsteamXX                     |
| Route - Local     | <ul><li>Destination: CIDR VPC</li></ul>   |
| Route - DMZ       | <ul><li>Destination:  0.0.0.0/0</li></ul> |
| Subnet Assocation | Your Subnet                               |

* [ ] Route Table
  * [ ] associée à votre sous-réseau
  * [ ] 2 routes
    * [ ] 1 route qui gère le flux interne (tout est autorisé en entrée et sortie)
    * [ ] 1 route qui gère le flux sortant (tout est autorisé vers la NAT)
    * [ ] 1 route qui gère le flux entrant (uniquement le RDP et le SSH en provenance de la DMZ)

## Instance Ec2

Vous devez réussir à déployer des instances Ec2 en respectant les contraintes suivantes:

* [ ] KeyPairs
  * [ ] name : key-devopsteamX
* [ ] Security Group
  * [ ] name : sg-devopsteamX
  * [ ] Pour l'instance Linux
    * [ ] Une règle entrante : SSH uniquement depuis la dmz
    * [ ] Une règle sortante : tous les flux
* [ ] Ec2
  * [ ] Type d'instance Linux :&#x20;



## Livrables

Sur votre dépôt, il s'agit d'ouvrir une feature par thème (Subnet et Ec2).

* [ ] Chaque étape du déploiement est isolé dans un script
  * [ ] Exemple : createSubnet.sh / deleteSubnet
* [ ] Chaque script débute par une ligne de commentaire qui décrit comment utiliser le script. Un exemple est le plus adapté.
* [ ] Reprenez les pratiques du labo s3:
  * [ ] Multiligne
  * [ ] Utilisation d'un profil (le même que pour labo s3)



