# Serveurs sous Debian 10 : DNS, Web, FTP et DHCP

Installation d'une machine virtuelle Debian 10 sous **VMware** et configuration de quatre services réseau. 

## Environnement

| Élément | Valeur |
|---|---|
| Système | Debian 10 (installation graphique) |
| Virtualisation | VMware |
| Mémoire / disque | 2 Go de RAM, disque de 30 Go |
| Réseau | 2 interfaces : NAT (accès Internet) et Host-only (communication entre machines virtuelles) |

## Services configurés

| Service | Paquet | Rôle |
|---|---|---|
| DNS | BIND9 | Zone locale `rone.sn`, enregistrements A et CNAME |
| Web | Apache2 | Hôte virtuel et page d'accueil personnalisée |
| FTP | vsftpd | Accès local uniquement (pas d'anonyme), utilisateurs enfermés dans leur dossier, chiffrement SSL/TLS |
| DHCP | isc-dhcp-server | Attribution d'adresses IP sur les interfaces `ens33` et `ens34` |

## Contenu du rapport

1. Création de la machine virtuelle et installation de Debian
2. Configuration de base : mise à jour des paquets, configuration réseau
3. Serveur DNS (BIND9)
4. Serveur web (Apache2)
5. Serveur FTP (vsftpd)
6. Serveur DHCP (isc-dhcp-server)

Rapport complet avec captures d'écran : [rapport-debian10.docx](rapport-debian10.docx)

## Compétences mises en œuvre

Administration Linux (Debian), ligne de commande, configuration réseau (NAT, Host-only), DNS, hôtes virtuels Apache, sécurisation FTP (SSL/TLS), DHCP, virtualisation VMware.


## Auteur

**LOUNIS Tassadit**
