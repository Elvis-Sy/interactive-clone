# 📦 Informations du projet – Site ID Interactive Clone

Ce document décrit les **modules installés** et leur **utilité** dans le projet. Il sert de référence rapide pour les membres de l’équipe qui participent au développement du clone du site [id-interactive.fr](https://www.id-interactive.fr).

---

## 🛠️ Dépendances principales

| Module                 | Description |
|------------------------|-------------|
| **React**              | Librairie JS principale pour construire l’interface utilisateur. Utilisée avec Vite pour un démarrage rapide et un rendu ultra-rapide. |
| **Vite**               | Outil de build ultra-rapide. Il sert à lancer l’application localement (`npm run dev`) et à la builder pour la production. |

---

## 🎨 Styling – UI

| Module          | Utilité |
|------------------|--------|
| **tailwindcss**  | Framework CSS utilitaire. Permet de construire rapidement une interface responsive sans écrire de CSS classique. |

---

## 🧭 Routage

| Module              | Utilité |
|---------------------|--------|
| **react-router-dom** | Gère la navigation entre les différentes pages (Home, Réalisations, Contact, etc.). Utilise `<Routes>`, `<Route>`, `<Link>`, etc. |

---

## 🎥 Animation & interactions

| Module            | Utilité |
|-------------------|---------|
| **framer-motion** | Librairie d’animation simple et puissante. Utilisée pour les animations d’entrée/sortie de composants, transitions de pages, hover effects, etc. |
| **gsap**          | Librairie d’animation avancée (GreenSock). Utilisée avec `ScrollTrigger` pour créer des effets complexes liés au scroll (parallax, pinning, reveals). |
| **split-type**    | Découpe du texte en lettres, mots ou lignes (HTML). Utilisé avec GSAP pour animer du texte lettre par lettre ou ligne par ligne. |

---

## 💡 Utilisation recommandée

| Cas d’usage                             | Librairie |
|-----------------------------------------|-----------|
| Apparition douce de sections            | `framer-motion` (`initial`, `animate`, `exit`) |
| Animation au scroll (fade in, parallax) | `gsap` + `ScrollTrigger` |
| Effets de texte dynamiques              | `split-type` + `gsap.from(...)` |
| Navigation entre pages                  | `react-router-dom` |
| Interface responsive                    | `tailwindcss` |

---

## 📂 Organisation recommandée

src/
├── animations/ **Fonctions GSAP (scrollTriggers, reveals...)**
├── assets/ **Images, icônes, etc.**
├── components/ **Composants réutilisables**
├── pages/ **Pages principales (home, contact...)**
├── routes/ **Configuration des routes**
├── App.jsx
└── main.jsx
└── index.css **Pour les styles globaux et themes**

---

## ⚠️ Conseils

- Utilisez **GSAP** uniquement pour les animations scroll complexes.
- Pour les animations simples (hover, fade, slide in), utilisez **framer-motion**.
- Évitez d’animer les mêmes éléments avec les deux librairies en même temps.
- Travaillez en `rem` / `em` / `%` plutôt qu’en `px` pour un meilleur comportement responsive.

---

## 📚 Documentation utile

- Tailwind : https://tailwindcss.com/docs
- React Router : https://reactrouter.com/
- Framer Motion : https://www.framer.com/motion/
- GSAP : https://gsap.com/docs/v3/
- SplitType : https://github.com/lukePeavey/SplitType

---

> 🔁 Ce document peut être mis à jour à chaque ajout ou suppression de dépendance.
