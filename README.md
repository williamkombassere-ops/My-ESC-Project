% Description du projet ESC Brushless (My-ESC-Project)

% --- Faits : Spécifications techniques ---
microcontroleur('STM32').
type_moteur('Brushless triphasé (BLDC)').
controle_vitesse('Régulation par PWM (rapport cyclique variable)').
commutation('120° via STM32 + Drivers IR2101').
etage_puissance('6 MOSFETs N-Channel').
largeur_pistes('1.5mm pour courant fort').
outil_conception('KiCad 9.0').

% --- Faits : Structure du dépôt ---
fichier_projet('Electronic Speed Controller.kicad_sch', 'Saisie schématique').
fichier_projet('Electronic Speed Controller.kicad_pcb', 'Routage du circuit imprimé').
fichier_projet('Electronic Speed Controller.kicad_pro', 'Fichier projet KiCad').
dossier('Images', 'Captures et schémas visuels').

% --- Règles : Requêtes d'information sur le projet ---

% Permet de lister toutes les spécifications du système
specification(Composant) :-
    microcontroleur(Composant);
    type_moteur(Composant);
    controle_vitesse(Composant);
    commutation(Composant);
    etage_puissance(Composant);
    largeur_pistes(Composant);
    outil_conception(Composant).

% Permet de vérifier si un fichier appartient au projet KiCad
est_element_kicad(Fichier) :-
    fichier_projet(Fichier, _).
