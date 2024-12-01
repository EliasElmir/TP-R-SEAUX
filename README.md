# TP-R-SEAUX


Projet Reseaux B2 INFORMATIQUE 


Réalisation de chacun : 

- Elias : Gestion des demandes de prix + DPGF + Calcule PoE & MBPS + Shema Logique et physique 
- Matteo : Préparation et animation de la soutenance
- Mahdi : Rédaction du mémoire technique
- Louna : /
- Cyriaque : /


MEMOIRE : 

**[1. Introduction]{.underline}**

Ce mémoire s\'inscrit dans le cadre de la conception d\'un réseau
complet pour un bâtiment multi-étages, répondant à un appel d\'offres
fictif. L\'objectif est de fournir une infrastructure réseau fiable,
évolutive et respectueuse de l\'environnement, alignée avec les besoins
exprimés dans le Cahier des Clauses Techniques Particulières (CCTP).

L\'approche repose sur une analyse rigoureuse des besoins, une
planification minutieuse des équipements, et une simulation
fonctionnelle permettant de valider la faisabilité technique. Ce projet
met l\'accent sur la modularité et la performance tout en respectant les
contraintes financières.

**[2. Analyse des Besoins]{.underline}**

**Les besoins principaux exprimés dans le CCTP incluent :**

-   Connectivité réseau complète (filaire et Wi-Fi) avec segmentation
    par VLAN pour chaque étage.

-   Plan d'adressage IP clair et extensible pour chaque étage et
    service.

-   Gestion PoE pour les équipements actifs (points d'accès Wi-Fi,
    caméras, etc.).

-   Bande passante adaptée au nombre d'utilisateurs pour éviter les
    goulots d\'étranglement.

-   Sécurisation et isolation des flux internes et externes via des
    VLAN.

-   Intégration d'équipements compatibles avec les standards modernes
    comme Wi-Fi 6E.

Le projet vise également à répondre à des critères environnementaux en
privilégiant des équipements à faible consommation énergétique et en
anticipant les besoins futurs par une planification d\'expansion.

**[3. Proposition Technique]{.underline}**

La solution proposée repose sur une architecture réseau robuste et
évolutive, intégrant les éléments suivants :

-   **Schéma logique** : VLAN, interconnexions et gestion du routage.

-   **Schéma physique** : Positionnement des équipements dans les
    étages.

-   **Configuration des équipements** : Modèles sélectionnés pour leur
    efficacité et leur compatibilité avec les besoins exprimés.

**3.1 Justification du Choix de Fortinet et du Schéma Mesh**

Le choix de Fortinet comme entreprise repose sur sa réputation et son
expertise dans le domaine des solutions réseau sécurisées et
performantes. Fortinet est reconnu pour offrir des équipements fiables,
adaptés aux environnements professionnels exigeants, notamment en
matière de sécurité, de gestion centralisée et de compatibilité avec des
normes modernes comme le Wi-Fi 6E.

Le schéma Mesh a été sélectionné pour sa capacité à offrir une
couverture réseau homogène et optimale dans un bâtiment multi-étages.
Cette architecture permet une connectivité fluide et une gestion
simplifiée, tout en assurant une redondance et une flexibilité en cas de
défaillance d'un nœud du réseau.

**[4. Schémas Logique et Physique]{.underline}**

Les schémas logique et physique, en format PDF, détailleront :

-   La structure des VLAN pour chaque étage et service.

-   Le positionnement des équipements (bornes Wi-Fi, switches, caméras)
    dans le bâtiment.

-   La connectivité inter-étages avec un focus sur la redondance.

**[5. Maquette Packet Tracer]{.underline}**

La maquette réalisée dans Packet Tracer simule le réseau Mesh proposé
avec les configurations suivantes :

-   VLAN distincts pour les réseaux invités et internes.

-   Configuration des commutateurs et des points d'accès Wi-Fi pour
    correspondre aux spécifications de Fortinet.

-   Validation de la connectivité entre les différents équipements du
    réseau.

**[6. Coûts et Équipements]{.underline}**

**La section ci-dessous détaille le processus d'évaluation et
d'optimisation des coûts associés aux équipements sélectionnés pour le
projet, conformément aux exigences du CCTP.**

**Pour réaliser cette évaluation, plusieurs étapes ont été suivies :**

1.  **Analyse des besoins par étage : Les quatre premiers étages ont été
    analysés pour déterminer le nombre d'équipements requis, notamment
    les dispositifs nécessitant une alimentation PoE. Par la suite, les
    besoins en ports et en puissance (en Watts) et MBPS ont été calculés
    pour chaque étage.**

2.  **Choix des équipements Fortinet : En consultant les gammes
    d'équipements Fortinet, une optimisation a été effectuée pour
    limiter les coûts. Les switches ont été sélectionnés en fonction des
    besoins spécifiques de chaque étage, avec un choix stratégique entre
    des switches à 48, 24 et 8 ports. Cela a permis de réduire les
    surcapacités inutiles dans certains étages.**

3.  **Application de la marge d'extension (+30%) : Conformément aux
    consignes, 30 % de capacité supplémentaire ont été ajoutés aux ports
    et à la puissance PoE pour anticiper les besoins futurs et assurer
    une évolutivité.**

4.  **Deux gammes d'équipements sélectionnées : Deux catégories de
    switches ont été retenues dans la gamme Fortinet :**

    -   **Switches standards : Offrant un bon rapport qualité/prix,
        adaptés aux besoins basiques.**

    -   **Switches performants (Séries 400 et 500) : Destinés aux zones
        nécessitant des performances élevées, notamment pour le cœur de
        réseau.**

5.  **Optimisation du cœur de réseau : Après des recherches sur les
    architectures réseau adaptées aux bâtiments multi-étages et aux
    schémas Mesh, trois switches cœur de réseau ont été retenus. Cette
    configuration garantit une robustesse accrue et une redondance
    efficace, permettant la continuité du service même en cas de
    défaillance d'un équipement.**

**Deux paniers ont été constitués pour répondre à des contraintes
budgétaires différentes :**

-   **Panier économique : Intègre principalement des switches standards
    pour réduire les coûts.**

-   **Panier premium : Inclut des switches haut de gamme pour des
    performances optimales.**

**Ces choix techniques assurent une optimisation à la fois financière et
opérationnelle, tout en respectant les contraintes exprimées dans le
CCTP.**

-   

**[7. Justifications du choix des modèles]{.underline}**

[1. FS-524D-FPOE (24 ports) et FS-548D-FPOE (48 ports)]{.underline}

Ports PoE intégrés : Ces switches sont idéaux pour alimenter directement
des équipements réseau tels que les points d\'accès WiFi, caméras de
surveillance, ou téléphones IP sur chaque étage. En éliminant le besoin
d\'alimentations séparées, ils simplifient considérablement
l\'installation et réduisent les coûts dans un bâtiment de grande
taille.

Performance adaptée : Les capacités de commutation robustes et les
uplinks 10 Gbps garantissent une gestion efficace des volumes de données
générés sur les 12 étages, même dans un environnement à forte densité
d\'appareils connectés.

Évolutivité : Grâce à leurs nombreux ports, ces modèles permettent
d\'ajouter facilement de nouveaux périphériques au réseau sans
nécessiter une mise à niveau matérielle, offrant ainsi une flexibilité
pour les futures extensions.

[2. FS-108F-FPOE (8 ports)]{.underline}

Design compact : Parfait pour des environnements nécessitant une
connectivité plus limitée, tels que les salles de serveurs ou les
extensions réseau dans des zones spécifiques où la densité d\'appareils
est faible.

Intégration homogène : Bien qu\'il soit de taille réduite, il reste
entièrement géré via FortiLink, garantissant une administration
cohérente et centralisée du réseau. Cela permet une gestion simplifiée
tout en maintenant une uniformité dans l'écosystème Fortinet.

[3. FortiSwitch 1048E : Le cœur du réseau]{.underline}

[a. Capacité et performance]{.underline}

48 ports 10 GbE et 6 uplinks 100 GbE : Ces ports haute vitesse assurent
une connectivité fluide entre les switches d\'accès (FS-524D, FS-548D)
déployés sur les 12 étages et le backbone du réseau. Ils offrent une
capacité suffisante pour gérer les volumes de trafic générés par des
centaines d'appareils connectés.

Connectivité backbone rapide et fiable : Les uplinks 100 GbE permettent
une communication ultra-rapide avec le cœur réseau ou les serveurs
centraux, garantissant une bande passante suffisante pour les
applications critiques.

Capacité de commutation massive : Avec une bande passante atteignant
1,44 Tbps, ce switch est conçu pour gérer de lourdes charges de données
sans compromettre les performances, un atout indispensable pour un
bâtiment de grande envergure.

[b. Fonctionnalités avancées]{.underline}

QoS (Quality of Service) : Cette fonctionnalité priorise les flux
critiques, tels que les communications VoIP, les applications
professionnelles, ou les transferts de données prioritaires, optimisant
ainsi les performances globales du réseau.

Support VLAN étendu : Permet une segmentation efficace du réseau, par
exemple en attribuant un VLAN distinct à chaque étage ou département,
assurant ainsi une isolation des données et une sécurité accrue.

Sécurité intégrée : Comprend des options avancées comme l'inspection des
sessions, l'authentification 802.1X, et une synchronisation transparente
avec FortiGate pour appliquer des politiques de sécurité uniformes dans
tout le réseau.

[c. Redondance et fiabilité]{.underline}

Alimentation redondante : Essentielle pour un switch de cœur, cette
fonctionnalité garantit le fonctionnement continu du réseau en cas de
défaillance d'une alimentation, minimisant ainsi les risques de panne.

Haute disponibilité : En intégrant des protocoles de redondance tels que
le VRRP (Virtual Router Redundancy Protocol), le réseau reste
opérationnel même en cas de panne matérielle, assurant ainsi une
continuité de service.

[4. Conclusion]{.underline} [:]{.underline} Une architecture réseau
optimale pour un grand bâtiment

Ces modèles offrent une combinaison idéale de puissance, flexibilité, et
sécurité pour répondre aux besoins d'un grand bâtiment à usage
professionnel.

Les switches d'accès (FS-524D, FS-548D, FS-108F) garantissent une
connectivité fiable et évolutive à chaque étage et dans les zones
spécifiques.

Le FortiSwitch 1048E, au cœur du réseau, assure une infrastructure
performante, sécurisée, et redondante capable de gérer de lourdes
charges de données sans latence.\
Cette architecture est parfaitement adaptée à un réseau d'entreprise
moderne nécessitant une gestion centralisée, une sécurité robuste, et
une performance optimale à long terme.

**[8. Conclusion]{.underline}**

**Ce mémoire technique présente une solution réseau complète et
optimisée pour répondre aux besoins spécifiques d'un bâtiment
multi-étages, tels qu'exprimés dans le CCTP. L'approche suivie a permis
de combiner une architecture robuste et évolutive avec des choix
financiers et techniques réfléchis.**

**La conception repose sur le choix stratégique de Fortinet pour ses
équipements fiables et performants, ainsi que sur une architecture Mesh,
idéale pour offrir une couverture homogène, une connectivité fluide et
une redondance accrue. Les besoins en segmentation VLAN, connectivité
filaire et Wi-Fi, ainsi que gestion PoE, ont été soigneusement pris en
compte à chaque étape de la planification.**

**Une attention particulière a été portée à l'optimisation des coûts et
des ressources :**

-   **Deux gammes d'équipements ont été constituées pour s'adapter à des
    contraintes budgétaires variées, avec un panier économique et un
    panier premium, tous deux basés sur les switches standards et
    performants de Fortinet.**

-   **Anticipation des besoins futurs par l'ajout d'une marge
    d'extension de 30 % en ports et en puissance PoE, garantissant une
    capacité évolutive.**

**La sélection de trois switches pour le cœur de réseau assure une
robustesse et une continuité de service en cas de défaillance,
renforçant la fiabilité de l'infrastructure.**

**En conclusion, cette solution réseau combine modularité, performance
et respect des contraintes financières et environnementales, tout en
anticipant les besoins futurs de l'entreprise. Elle représente une
réponse technique et financièrement solide, alignée avec les objectifs
du projet.**



