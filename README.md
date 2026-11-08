# NodX-Lab

Mon homelab pour apprendre les réseaux, Linux et la cybersécurité en manipulant du matériel, en testant des configurations et en cherchant pourquoi ça ne fonctionne pas.

Les notes de cours et les notions à retenir sont dans [learning-journey](https://github.com/itsnodx/learning-journey). Ici, je garde les essais pratiques.

## Mon matériel

| Équipement | Utilisation |
|---|---|
| MacBook Pro M4 | Administration et captures |
| Dell — Ubuntu Server 24.04 LTS | Tests réseau, SSH et services |
| Beelink Ryzen 7 (32 Go) | Proxmox prévu |
| TP-Link TL-SG1016DE | Réseau local et premiers tests |
| Cisco 2960-X | Commutation, VLAN |
| Cisco 3750-X | Commutation et routage |
| pfSense, routeurs Cisco, Raspberry Pi | Évolutions prévues, pas encore en service |

## Réseau prévu

```text
Internet / réseau domestique
             |
          pfSense (prévu)
             |
       Cisco 3750-X
         /       \
   Cisco 2960-X   TP-Link
                      |
                 Dell / autres hôtes
```

Ce schéma est une **cible**, pas la configuration actuelle du lab. L'installation se fait progressivement.

## Labs

Les comptes rendus seront ajoutés dans `labs/` au fil des essais réalisés. Je ne crée pas de dossiers vides pour les expériences à venir.

Exemple d'organisation lorsqu'un lab sera prêt :

```text
labs/
└── lab-01-ping-arp-wireshark/
    ├── README.md
    ├── captures/  (si nécessaire)
    └── configs/   (si nécessaire)
```

Pas de modèle obligatoire. Pour chaque lab, quelques lignes suffisent si elles répondent à ces questions :

1. **Qu'est-ce que j'ai essayé ?** Matériel, objectif et commandes importantes.
2. **Qu'est-ce que j'ai observé ?** Résultat, capture ou panne rencontrée.
3. **Qu'est-ce que j'ai compris ou corrigé ?** Et ce que je veux tester ensuite.

Une capture utile vaut mieux qu'une longue page remplie pour la forme. Je complète les notes si le lab devient plus complexe.

## Précautions

Je vérifie les captures et les configurations avant publication : pas de mot de passe, clé privée ni information personnelle. Les fichiers `.pcap` et `.pcapng` sont ignorés par défaut.
