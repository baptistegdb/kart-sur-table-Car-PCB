# Projet de carte PCB pour le projet 'Kart Sur Table' 

## Description

Ce dépôt contient les fichiers de conception d'une carte PCB pour le projet 'Kart Sur Table'. La carte a été conçue pour remplacer le montage actuel utilisé cette année, qui est composé de nombreux modules assemblés les uns sur les autres. Le but de cette carte est de centraliser toutes les fonctionnalités nécessaires sur une même carte, afin d'optimiser l'espace disponible et de réduire la taille de l'électronique.
Fichiers

   - Rapport du projet.pdf : rapport de projet détaillant la conception de la carte PCB.
   - Peripherals.SchDoc : schématique des périphériques de la carte (IMU, pont en H pour les moteurs, boutons BOOT et EN, LED de contrôle).
   - power.SchDoc : schématique de l'alimentation de la carte (régulation de la tension en 5V et 3V3).
   - Controller.SchDoc : schématique du microcontrôleur de la carte (ESP32-WROOM-32E).
   - PCB1 25-03-2024 16-33-14.WAS : fichier de sauvegarde automatique de la conception de la carte PCB.
   - PCB1.cctpref : fichier de préférences de la conception de la carte PCB.
   - Schlib1.SchLib : bibliothèque de schémas pour la conception de la carte PCB.
   - PcbLib1.PcbLib : bibliothèque de PCB pour la conception de la carte PCB.
   - PCB1.PcbDoc : fichier de conception de la carte PCB.

## Conception de la carte PCB

La carte PCB a été conçue à l'aide du logiciel Altium Designer. Elle est composée de trois parties principales : les périphériques, l'alimentation et le microcontrôleur.
Périphériques

## Les périphériques de la carte sont les suivants :

   - Une IMU (LSM6DS3TR) pour mesurer l'accélération et la vitesse angulaire du kart.
   - Un pont en H (TB6612FNG) pour contrôler les deux moteurs du kart.
   - Deux boutons (BOOT et EN) pour démarrer et arrêter le microcontrôleur.
   - Deux LED (rouge et verte) pour indiquer l'état du microcontrôleur.

## Alimentation

L'alimentation de la carte est assurée par deux régulateurs de tension :

   - Un régulateur LDO (LMR14050) pour réguler la tension d'entrée (7,4V) à 5V.
   - Un régulateur LDO (TPS7A7002DDAR) pour réguler la tension de 5V à 3V3.

La carte est alimentée par une batterie LiPO de 7,4V/3600mAh, qui est connectée à la carte via un connecteur JST.
Microcontrôleur

Le microcontrôleur de la carte est un ESP32-WROOM-32E. Il est connecté aux périphériques et à l'alimentation de la carte via des connecteurs et des broches d'alimentation.


- pour en savoir plus consultez le Rapport du projet :

[Rapport du projet](https://github.com/baptistegdb/kart-sur-table-Car-PCB/blob/main/Rapport%20du%20projet.pdf)
