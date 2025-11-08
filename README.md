# 🐔 Zelda Noob - Partie 7 : PNJ avec Intelligence Artificielle

> Un tutoriel RPG Godot 4 par **Lysdora Craft** - Apprends à créer des personnages non-joueurs autonomes !

![Godot 4.4](https://img.shields.io/badge/Godot-4.4+-blue?logo=godotengine)
![License MIT](https://img.shields.io/badge/license-MIT-green)
![YouTube](https://img.shields.io/badge/YouTube-Lysdora%20Craft-red?logo=youtube)

---

## 📺 Vidéo du tutoriel

🎬 **[Regarder la Partie 7 sur YouTube](https://www.youtube.com/watch?v=CXW521WiT9k)**

---

## 🎯 Ce que tu vas apprendre dans cette partie

Dans cet épisode, on crée un **poulet qui se balade tout seul** dans le jeu ! C'est notre premier PNJ (Personnage Non-Joueur) avec une vraie IA simple mais efficace.

### ✨ Les nouvelles fonctionnalités

#### 🐓 **Mouvement autonome du poulet**
- Le poulet se déplace automatiquement de gauche à droite
- Il change de direction toutes les 2 secondes grâce à un `Timer`
- Il s'arrête parfois pour faire une pause (20% de chance) - réaliste !
- Quand il touche un mur, il fait demi-tour intelligemment

#### 🎲 **Système de choix aléatoires**
- Utilisation de `randi()` pour générer des nombres au hasard
- La fonction `pick_random()` pour choisir une direction aléatoirement
- Création d'une IA simple mais vivante !

#### 🎬 **Animation et feedback visuel**
- Animations "walk" (marche) et "idle" (repos)
- Le sprite se retourne (`flip_h`) selon la direction
- Animation de collecte avec **Tween** :
  - Le poulet saute vers le haut
  - Il fait une rotation complète (360°)
  - Il retombe au sol
  - Il disparaît en fondu

#### 🪶 **Système de drop d'objets**
- Quand tu ramasses le poulet, il drop une **plume**
- Utilisation de `preload()` pour charger la scène de la plume
- Instanciation dynamique avec `instantiate()`
- Ajout dans le jeu avec `add_child()`

#### 📡 **Système de signaux**
- Émission d'un signal `poulet_collecte` quand le poulet est ramassé
- Utilisation de `queue_free()` pour supprimer proprement le poulet

---

