Debian Secure NAS

Introduction

Ce projet présente la mise en place d’un serveur NAS sécurisé sous Debian Bookworm.
L’objectif est de déployer une solution de stockage fiable et accessible via plusieurs protocoles réseau tout en appliquant des mécanismes de sécurité et d’administration adaptés à un environnement Linux.

Le serveur repose sur un RAID5 logiciel géré par mdadm permettant la tolérance à la panne d’un disque.

Le stockage est monté sur /mnt/raid et exposé via plusieurs services :

- SMB / Samba pour Windows et macOS
- NFS pour Linux
- SFTP chrooté pour les transferts sécurisés
- WebDAV en HTTPS pour l’accès web

Le serveur intègre également plusieurs outils d’administration et de sécurité :

- Cockpit pour l’administration web
- rsync + cron pour les sauvegardes automatiques
- Tailscale pour l’accès distant sécurisé
- Fail2Ban pour la protection contre les attaques

Projet réalisé dans le cadre de ma formation à La Plateforme (2026).
