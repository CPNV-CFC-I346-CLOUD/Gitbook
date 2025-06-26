# Backlog AWS

## Réalisation du laboratoire

Pour connaître les tâches à réaliser durant ce laboratoire, veuillez vous référez à ce backlog qui sera présenté et discuté durant les heures de présence en classe.

## Objectifs

Déployer une infastructure comme celle dessinée ci-dessous. La validation de l'infrastructure se fera en démontrant le scenario suivant:

```
//GIVEN (contexte de départ)
* l'infrastructure a été déployée
* je suis connecté sur mes deux instances privées (LIN et WIN)

//WHEN (événement)
* depuis mon sous-réseau privé, je tente d'accéder à internet (ping 8.8.8.8)

//THEN (résultat attendu
* j'observe l'envoi et la réception des paquets du "ping" 
  prouvant la connectivité avec l'extérieur du VPC
```

### Exemple de résultat à obtenir

```bash
ping 8.8.8.8
```

```bash
Pinging 8.8.8.8 with 32 bytes of data:
Reply from 8.8.8.8: bytes=32 time=25ms TTL=103
Reply from 8.8.8.8: bytes=32 time=11ms TTL=103
Reply from 8.8.8.8: bytes=32 time=10ms TTL=103
Reply from 8.8.8.8: bytes=32 time=12ms TTL=103

Ping statistics for 8.8.8.8:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 10ms, Maximum = 25ms, Average = 14ms
```

## Infrastructure à déployer

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

* Pour chacunes des "cartes", une démontration aura lieu en classe

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Capture d'écran du backlog présentant les différentes tâches à réaliser</p></figcaption></figure>

{% embed url="https://github.com/orgs/CPNV-CFC-I346-CLOUD/projects/1" %}

* Une fois par semaine, une sesssio de question-réponse sera proposée, permettant d'affiner la compréhension du travail à réaliser et de valider les étapes intermédiaires.
* Pour connaître les valeurs à utiliser (tag name, nom des ressources) vous pouvez, via l'accès à al console d'AWS qui vous a été livrée, voir le résultat attendu concernant l'équipe "devopsteam99".

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption><p>Exemple pour le "devopsteam99" - > subnets</p></figcaption></figure>

