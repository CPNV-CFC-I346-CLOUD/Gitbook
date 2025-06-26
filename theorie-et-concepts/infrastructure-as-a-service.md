# Infrastructure as a Service

## Intention pédagogique

Appréhender le vocabulaire spécifique aux infrastructure "as a Service" et faire des liens avec les infrastructures connues.

## Les différents composants clés d'une infrastructure "as a Service"

### Pour les composants en lien avec la mise en place du réseau:

| Besoin                                       | Produit AWS                                                                                                     |
| -------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| Isoler son infrastructure (private)          | [VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) \*                              |
| Situer son infrastructure                    | [Region and AZ](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/) \*                          |
| Connecter son infrastructure au web          | [Internet Gateway (IGW)](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.htm) \*          |
| Offrir un accès sortant à son infrastructure | [Network Address Translation (NAT)](https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html) \* |
| Assigner une adresse ip à son infrastructure | [Public IP (EIP)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-addresses-eip.html) \*         |
| Définir des sous-réseaux                     | [Subnet](https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html) \*                            |
| Réguler le traffic entre les réseaux         | [Route table](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Route_Tables.html) \*                        |

### Pour les composants en lien avec de la puissance de calcul:

| Besoin                                    | Produit AWS                                                                                                                       |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Gérer des machines virtuelles             | <p><a href="https://aws.amazon.com/ec2/">EC2</a> *<br><a href="https://aws.amazon.com/ec2/instance-types/">Instance types</a></p> |
| Disposer d'espace de stockage pour les vm | [EBS](https://aws.amazon.com/ebs/)                                                                                                |
| Gérer la sécurité (parefeu)               | [Security group (SG)](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html) \*                               |
| Utiliser des images préconfigurées de vm  | [AMI](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html)                                                              |
| Réaliser des sauvegardes des volumes      | [SNAPSHOT](https://docs.aws.amazon.com/ebs/latest/userguide/ebs-snapshots.html)                                                   |
| Obtenir des clés d'accès pour les vm.     | [KEY PAIRS](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html)                                               |



{% embed url="https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html" %}

## Démonstration

Une démonstration via la console AWS sera réalisée en classe pour amener chacun des éléments présentés ci-dessus.

