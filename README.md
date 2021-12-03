# Advanced Packet Tracer 

## Etape 1 - 

Réalisation d'un schéma correspondant à l’ensemble des éléments composant le quest, loopbacks compris.

Dans le schéma devra apparaître :

- Les équipements utilisés.
- Les adresses IP (adresses réseaux, adresses des interfaces, masques de sous-réseau et adresses broadcast s’il y a lieu).
- Le nom des interfaces utilisées.
- Les protocoles de routage utilisés.

## Etape 2 - 

- Nommez vos routeurs R1, R2, R3, R4 et R5.
- Nommez vos switchs SW1 et SW2.
- Changez le motd de chaque routeur par « Welcome to router RX », X étant le numéro du routeur.
- Ajoutez le mot de passe « cisco » pour le mode enable de vos routeurs.

## Etape 3 -

#### OSPFv3 – Area 0 – AS 20: FE01:20: :

- Connectez le PC5 au routeur R4.
- Configurez la loopback Lo4 sur le routeur R4 - elle comprendra 1000 hôtes.
- Configurez le protocole de routage OSPFv3 avec la zone 0.

## Etape 4 -

#### OSPFv3 – Area 0 – AS 10: FE01:20: :

- Connectez le routeurs R1 au switch SW1.
- Connectez les switches SW1 et SW2 à l’aide d’un seul câble Ethernet.

#### VLAN 10 Comptabilité

- Connectez le PC2 au switch SW1.
- Connectez le PC3 au switch SW2.
- Configurez-le VLAN 10, nommé « Comptabilité », sur les deux switches.

#### VLAN 20 Finance

- Connectez le PC1 au switch SW1.
- Connectez le PC4 au switch SW2.
- Configurez-le VLAN 20, nommé « Finance », sur les deux switches.
- Configurez le protocole de routage OSPFv3 avec la zone 0.

## Etape 5 -

#### VTP

- Configurez le switch SW1 en mode serveur avec le mot de passe « Etna ».
- Configurez le switch SW2 en mode client.

## Etape 6 -

#### EIGRP – AS 10 : 172.25.0.0

- Connectez le routeur R1 au routeur R2.
- Connectez le routeur R1 au routeur R5.
- Connectez le routeur R2 au routeur R5.
- Configurez la loopback Lo1 sur le routeur R1 - elle comprendra 50 hôtes.
- Configurez la loopback Lo2 sur le routeur R2 - elle comprendra 500 hôtes.
- Configurez le protocole de routage EIGRP.

## Etape 7 -

#### EIGRP – AS 10 : 172.25.0.0

- Configurez les interfaces des routeurs R2 et R5 en mode « passive interface ».

## Etape 8 -

#### OSPF (IPv4) – AS 20 : 172.16.0.0

- Connectez le routeur R3 au routeur R4.
- Configurez la loopback Lo3 sur le routeur R3 - elle comprendra 4 hôtes.

## Etape 9 -

#### OSPF (IPv4) – Authentification

- Configurez l’authentification en MD5 entre les routeurs R3 et R4 avec le mot de passe « etna_cisco ».

## Etape 10 -

#### BGP : 192.168.10.0

- Connectez les routeurs R2 et R3.
- Configurez le protocole de routage BGP entre les deux routeurs :
- Le protocole de routage EIGRP est dans le système autonome 10.
- Le protocole de routage OSPF est dans le système autonome 20.
- Configurez la redistribution entre les différents protocoles de routage.

## Etape 11 -

#### EIGRP – AS 10 : 172.25.0.0

- Connectez le serveur S1 au routeur R5.
- Configurez « Syslog » sur le serveur S1 pour qu’il enregistre les logs de tous les routeurs.
- Configurez le protocole OSPF pour que vos routeurs, loopbacks, PCs et votre serveur puissent communiquer entre eux.

## Etape 12 -

#### OSPF – AS 20 : 172.16.0.0

- Connectez le serveur S2 au routeur R3.
- Sauvegardez les configurations des routeurs sur le serveur TFTP (S2) en les nommant save_RX (X correspondant au numéro du routeur).

## Etape 13 -

#### Tunnel 6to4 : FE01:2 ::

- Configurez un tunnel 6to4 afin que tous les PCs puissent communiquer entre eux.

Copyright © 2021 Groupe de COURTAUX Franck
