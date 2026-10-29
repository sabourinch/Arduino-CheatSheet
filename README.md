# Aide-mémoire Arduino · Arduino Cheat Sheet

Aide-mémoire interactif pour les cartes Arduino à microcontrôleur **AVR 8 bits** (ATmega328P et ATmega2560), en français et en anglais.

**➜ [Ouvrir l'aide-mémoire](https://sabourinch.github.io/Arduino-CheatSheet/)**

*English version below.*

---

## Contenu

- **Plus de 60 fiches** classées en 12 catégories : structure, E/S numériques et analogiques, temps, liaison série, maths, types, contrôle, bits, interruptions, timers et bibliothèques. Chaque fiche a une courte explication et un exemple de code coloré, copiable en un clic.
- **Configurateur d'interruptions par les registres** :
  - interruptions externes INTx avec choix du front (EICRA/EICRB, EIMSK, EIFR) ;
  - interruptions sur changement d'état PCINT, sur une ou plusieurs broches (PCICR, PCMSKn, PCIFR) ;
  - affichage bit par bit des registres et code prêt à l'emploi.
- **Configurateur de timers** :
  - modes Normal, CTC, Fast PWM et PWM à phase correcte ;
  - choix automatique ou manuel du prescaler, avec la fréquence réelle et l'erreur ;
  - registres TCCRnA, TCCRnB et TIMSKn détaillés, et code généré.
- **Brochage des cartes** : broches PWM, analogiques, d'interruption, I²C et SPI, et LED intégrée.
- **Calculateurs** : conversion `analogRead` → tension, `map()` avec l'arrondi entier de la carte, et résistance pour une LED (valeur E12 et code couleur).

### Fonctions pratiques

- Recherche instantanée : la touche `/` place le curseur dans le champ, `Échap` l'efface. La recherche trouve les fiches en français comme en anglais.
- Filtres par catégorie.
- Bascule **FR / EN**. Elle traduit aussi les commentaires du code, et la langue choisie est mémorisée.
- Thème clair ou sombre selon le réglage du système.
- Affichage adapté au téléphone.

## Cartes prises en charge

| Carte | Microcontrôleur | Horloge |
|---|---|---|
| Uno R3 | ATmega328P | 16 MHz |
| Nano | ATmega328P | 16 MHz |
| Pro Mini | ATmega328P | 16 MHz (5 V) ou 8 MHz (3,3 V) |
| Mega 2560 | ATmega2560 | 16 MHz |

Les cartes 32 bits (Uno R4, Due, Zero, ESP32…) ne sont pas couvertes : leurs registres et leurs limites sont différents.

## Utilisation hors ligne

Le site tient en un seul fichier, `index.html`, sans dépendance à installer. Téléchargez-le et ouvrez-le dans un navigateur. Seules les polices (Google Fonts) demandent une connexion ; sans elles, la page utilise les polices du système.

## Avertissement

Les valeurs et le code sont donnés à titre indicatif. Vérifiez toujours la fiche technique de votre carte et du microcontrôleur avant de câbler ou de modifier des registres. En particulier, reconfigurer le Timer 0 fausse `millis()` et `delay()`.

---

## English

An interactive cheat sheet for **8-bit AVR** Arduino boards (ATmega328P and ATmega2560), available in French and English.

**➜ [Open the cheat sheet](https://sabourinch.github.io/Arduino-CheatSheet/)**

- **60+ reference cards** across 12 categories, each with a short explanation and a copyable, highlighted code example.
- **Register-level interrupt configurator**: INTx with edge selection, and PCINT on one or more pins. It shows the register bits and generates the code.
- **Timer configurator**: Normal, CTC, Fast PWM and phase correct PWM. It picks the prescaler automatically or lets you choose one, shows the actual frequency and error, and generates the code.
- **Board pinouts** and **calculators** (ADC voltage, `map()`, LED resistor).
- Instant search (`/` to focus), category filters, **FR / EN** toggle, light and dark themes, mobile-friendly layout.
- A single `index.html` file with nothing to install: it also works offline.

Supported boards: Uno R3, Nano, Pro Mini, Mega 2560. 32-bit boards are not covered.
