# PROJET-STM32-TRACKSAFE
# Projet STM32 TrackSafe (ATAROUWA Abdou-Malik / HADJ-SAID Matthieu)

![image](https://github.com/Lik-i-am/Projet-STM32-TrackSafe/assets/173574043/cf14d9cc-38f7-46fb-a669-acc8b29d68b5)

![image](https://github.com/Lik-i-am/Projet-STM32-TrackSafe/assets/173574043/923e7ce3-e607-4075-9e74-10c4018784c4)


## 1. Placer votre TrackSafe sur le colis :

Le TrackSafe doit être fixé solidement sur le colis pour garantir que les capteurs puissent détecter fidèlement les conditions de transport du colis.


## 2. Alimenter votre TrackSafe :

Le TrackSafe nécessite une source d'alimentation pour fonctionner. Cela peut être une batterie rechargeable ou une alimentation externe via un connecteur approprié.


## 3. Détection des chocs avec l'accéléromètre (I2C) :

### Fonctionnement :

  -  Accéléromètre : Utilisation d'un capteur accéléromètre pour détecter les chocs et les vibrations.
  
  -  Communication I2C : L'accéléromètre communique avec le microcontrôleur STM32 via le protocole I2C.
  
  -  Seuil de détection : Lorsque l'accéléromètre détecte une accélération dépassant un certain seuil sur les axes X ou Y, cela est interprété comme un choc.

### Exemple de code :



## 4. Détection de la température (I2C) :

### Fonctionnement :

   - Détecteur de température : Utilisation d'un capteur de température pour surveiller les conditions environnementales.
   
   - Communication I2C : Le capteur de température communique avec le microcontrôleur STM32 via le protocole I2C.
   
   - Seuil de température : Lorsque la température détectée dépasse 30°C, une alarme est déclenchée.

### Exemple de code :


## 5. Alarme et affichage des erreurs (BUZZER PWM + SPI) :

### Fonctionnement :

   - Alarme sonore : Utilisation d'un buzzer pour alerter en cas de choc ou de température élevée.
   
   - Communication SPI : Utilisation du protocole SPI pour la communication avec d'autres périphériques si nécessaire.
   
   - PWM : Le buzzer est contrôlé par un signal PWM pour générer le son d'alarme.

### Exemple de code :



## 6. Consultation de l'historique via le port série (GPIO INTERRUPTION + AFFICHAGE LED + UART) :

### Fonctionnement :

   - Mot de passe : Utilisation d'une séquence de boutons pour entrer le mot de passe (1, 4, 3, 2) via GPIO interruptions.
   
   - Affichage LED : Indication visuelle pour chaque chiffre du mot de passe entré.
   
   - UART : Consultation de l'historique des événements via la communication UART.

### Exemple de code :



## 7. Réglage de l'intensité de l'afficheur avec le potentiomètre (ADC) :

### Fonctionnement :

   - Potentiomètre : Utilisation d'un potentiomètre pour ajuster l'intensité de l'afficheur.
   
   - ADC : Conversion de la position du potentiomètre en signal numérique pour contrôler l'intensité de l'afficheur.

### Exemple de code :


![image](https://github.com/Lik-i-am/Projet-STM32-TrackSafe/assets/173574043/ab7bd885-770a-4256-9b8d-4c88eac1d78b)

![image](https://github.com/Lik-i-am/Projet-STM32-TrackSafe/assets/173574043/410cdbf5-4adf-45fd-b951-aad4bf910c11)

# Conclusion :

Le projet TrackSafe intègre diverses technologies pour surveiller et sécuriser les colis durant le transport. 
Grâce à l'utilisation de capteurs et de modules de communication, TrackSafe offre une solution complète pour la détection des chocs et des variations de température, l'alerte sonore en cas d'anomalie, et la consultation de l'historique via une interface sécurisée.

![image](https://github.com/Lik-i-am/Projet-STM32-TrackSafe/assets/173574043/8d59ce7b-6bb7-4704-803e-ca9168279582)
