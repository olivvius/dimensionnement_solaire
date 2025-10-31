# Dimensionnement Solaire

Cet outil est une application web conçue pour aider les utilisateurs à dimensionner une installation solaire autonome. En partant de la consommation électrique journalière, l'application calcule les besoins en panneaux solaires, en capacité de batterie, et fournit des indications essentielles pour le câblage et les protections du système.

## Fonctionnalités

- **Calcul de la consommation** : Estimez votre besoin énergétique journalier en listant vos appareils électriques.
- **Dimensionnement des panneaux** : Détermine la puissance photovoltaïque nécessaire et le nombre de panneaux requis.
- **Dimensionnement des batteries** : Calcule la capacité du parc de batteries en Wh et en Ah, en fonction de l'autonomie souhaitée.
- **Calcul des protections** : Suggère les calibres pour les fusibles et disjoncteurs.
- **Calcul des sections de câbles** : Propose les sections de câbles adaptées en fonction des distances et des courants.

## Guide d'utilisation

L'application est divisée en plusieurs sections pour vous guider pas à pas. Voici comment remplir les champs principaux.

### 1. Bilan de Consommation

Cette première section sert à calculer votre besoin total en énergie pour une journée.

- **Ajouter un appareil** : Utilisez le menu déroulant pour sélectionner un appareil commun dans la liste. Ses valeurs de puissance et de durée se rempliront automatiquement. Vous pouvez les ajuster.
- **Puissance (W)** : Indique la puissance instantanée de l'appareil lorsqu'il fonctionne. Cette information se trouve généralement sur l'étiquette de l'appareil ou son chargeur.  Si non, vous pouvez utiliser un wattmètre.
- **Durée / jour (h)** : Estimez combien d'heures par jour cet appareil sera utilisé.

L'**Énergie journalière totale (Wh)** est la somme de l'énergie consommée par tous vos appareils. C'est la base de tous les autres calculs.

### 2. Paramètres du Système

Ici, vous définissez les caractéristiques de votre future installation.

- **Jours d'autonomie souhaités** : Le nombre de jours pendant lesquels votre système doit pouvoir fonctionner sans soleil (grâce aux batteries). Une valeur de 2 ou 3 est courante.
- **Puissance d'un panneau (Wc)** : Indiquez la puissance crête d'un seul panneau solaire que vous envisagez d'acheter (ex: 400 Wc).
- **Tension du parc batteries (V)** : C'est la tension de votre système de stockage. Les choix courants sont 12V, 24V ou 48V. Un système en 24V ou 48V est généralement plus efficace pour des besoins importants.
- **Tension des panneaux (V)** : La tension nominale de vos panneaux. Elle doit être compatible avec votre régulateur de charge et la configuration de votre parc batteries.
- **Puissance max entrée solaire onduleur (W)** : La puissance maximale que votre onduleur (ou régulateur de charge) peut recevoir depuis les panneaux solaires. Cette donnée se trouve dans la fiche technique de l'onduleur.
- **Puissance max sortie batterie (W)** : La puissance maximale que vos batteries peuvent délivrer en continu. Cette valeur est cruciale et se trouve dans la documentation de la batterie.
- **Distance panneaux -> onduleur (m)** : La longueur de câble (aller simple) entre vos panneaux solaires et votre onduleur/régulateur.
- **Distance batteries -> onduleur (m)** : La longueur de câble (aller simple) entre votre parc de batteries et votre onduleur.

### 3. Comprendre les Résultats

Les sections "Résultats Calculés" et "Caractéristiques du Circuit" vous donnent les grandeurs dimensionnées pour votre projet.

- **Puissance PV nécessaire** : La puissance crête minimale que votre champ solaire doit pouvoir produire pour couvrir vos besoins journaliers.
- **Capacité batterie (Ah)** : La capacité de stockage nécessaire, exprimée en Ampères-heures pour la tension que vous avez choisie.
- **Demande de puissance de pointe** : La puissance totale si tous vos appareils fonctionnaient en même temps. Assurez-vous que cette valeur est inférieure à la "Puissance max sortie batterie".
- **Fusible / Disjoncteur** : Calibres des protections électriques à installer pour sécuriser votre installation.
- **Section câble** : Diamètre du câble en mm² recommandé pour limiter les pertes d'énergie et éviter la surchauffe.

