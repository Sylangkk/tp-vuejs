# Superheroes Web Application

Ce projet est une application web permettant aux utilisateurs d'explorer une collection de superhéros, de consulter des informations détaillées sur eux, et de trouver des superhéros en fonction de superpouvoirs spécifiques. L'application est construite avec **HTML**, **Vue.js**, **Axios**, et **Bootstrap** pour offrir une expérience utilisateur réactive et dynamique.

---

## 📝 Fonctionnalités

### 1. **Page d'accueil (index.html)**
- Affiche une liste de superhéros récupérés via une API externe.
- Fournit une barre de recherche pour filtrer les superhéros par nom.
- Inclut un bouton permettant de consulter les détails de chaque superhéros.

### 2. **Page de détails des superhéros (detail.html)**
- Affiche des informations détaillées sur un superhéros, y compris :
  - Biographie (Nom complet, Lieu de naissance).
  - Statistiques de puissance (Intelligence, Force, Vitesse, etc.).
  - Une grande image du superhéros.
- Les données sont récupérées dynamiquement en fonction de l'ID du superhéros passé en paramètre dans l'URL.

### 3. **SuperPower Matcher (superpower_matcher.html)**
- Permet aux utilisateurs de sélectionner les superpouvoirs souhaités (ex : Intelligence, Force, Vitesse).
- Trouve et affiche les superhéros dont les statistiques répondent aux critères sélectionnés.
- Fournit une interface interactive et claire pour filtrer en fonction des superpouvoirs.

---

## 🛠️ Détails techniques

### Frameworks et bibliothèques utilisés
1. **Vue.js 3** : Pour la gestion réactive et dynamique des données.
2. **Axios** : Pour effectuer des requêtes HTTP et récupérer les données des superhéros depuis une API externe.
3. **Bootstrap 5** : Pour le style et le design responsive.

### API
L'application récupère les données des superhéros via l'[API Superhero](https://github.com/rtomczak/superhero-api) hébergée sur **jsDelivr**.

### Dépendances
- **Vue.js** : Chargé depuis le CDN officiel (`https://unpkg.com/vue@3`).
- **Axios** : Chargé depuis le CDN officiel (`https://unpkg.com/axios@latest`).
- **Bootstrap** : Chargé depuis le CDN officiel (`https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css`).

---

## 🚀 Comment exécuter le projet ?

1. **Clonez ou téléchargez le dépôt.**

2. **Ouvrez `index.html` dans un navigateur web moderne.**

3. **Assurez-vous d'avoir une connexion internet active** pour :
   - Récupérer les données des superhéros depuis l'API externe.
   - Charger Vue.js, Axios et Bootstrap depuis leurs CDN.

4. Utilisez les liens de navigation pour accéder aux pages **index (Home)** et **SuperPower Matcher**.

---

## 🛠️ Fonctionnement

### Page d'accueil
- Récupère tous les superhéros depuis l'API.
- Affiche leurs noms, IDs et une petite image.
- Permet de filtrer par nom grâce à la barre de recherche.
- Redirige vers la page de vue détaillée via un bouton.

### Page de détails des superhéros
- Récupère les détails d’un superhéros grâce à l’ID passé dans l’URL (ex : `detail.html?id=1`).
- Affiche dynamiquement la biographie, l’image et les statistiques de puissance.

### SuperPower Matcher
- Permet de sélectionner les superpouvoirs grâce à des cases à cocher.
- Filtre et affiche les superhéros dont les statistiques répondent aux critères sélectionnés (ex : force > 50).

---

## 📂 Structure du projet

```plaintext
/src
├── index.html        # Le fichier principal de l'application
├── detail.html      # Page de détails des superhéros
├── superpower_matcher.html  # Page de super héro à partir de superpouvoirs
```