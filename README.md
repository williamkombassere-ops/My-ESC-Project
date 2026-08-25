# My-ESC-Project 🚀

Contrôleur de vitesse électronique (ESC) open-source pour moteur brushless triphasé, conçu sur mesure avec KiCad et piloté par un microcontrôleur STM32.

---

## 📌 Aperçu du projet

Ce projet consiste en la conception complète (schématique, routage PCB et logique de commande) d'un ESC (Electronic Speed Controller) adapté aux moteurs synchrones triphasés (BLDC). Il est dimensionné pour supporter des courants forts et implémente une commutation adaptée au pilotage de moteurs de forte puissance.

---

## ⚙️ Spécifications techniques

* **Microcontrôleur :** STM32
* **Type de moteur :** Moteur brushless triphasé (BLDC)
* **Contrôle de vitesse :** Régulation par PWM (rapport cyclique variable)
* **Commutation :** Commutation 120° via STM32 + Drivers de MOSFET IR2101
* **Étage de puissance :** 6 MOSFETs N-Channel
* **Conception PCB :** Pistes de **1.5 mm** optimisées pour le passage de courants forts
* **Outil de conception :** KiCad 9.0

---

## 📂 Structure du dépôt

```text
My-ESC-Project/
├── Images/                               # Captures et schémas visuels du projet
├── Electronic Speed Controller.kicad_sch # Schématique électronique (KiCad)
├── Electronic Speed Controller.kicad_pcb # Routage du circuit imprimé (KiCad)
├── Electronic Speed Controller.kicad_pro # Fichier projet KiCad
└── README.md                             # Documentation du projet
