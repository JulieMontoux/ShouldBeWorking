# ShouldBeWorking 🎯

Un compteur de procrastination qui te rappelle gentiment (ou pas) que tu devrais être en train de bosser.

---

## L'équipe

| Nom | Rôle Scrum |
|-----|-----------|
| Julie | Product Owner |
| Paul | Scrum Master |
| Yassin | Dev Team |
| Mathieu | Dev Team |

---

## La vision produit

**Quel problème résout ce projet ? Pour qui ?**

En tant que **développeur/étudiant/professionnel**, ce projet permet de **prendre conscience du temps réellement perdu en procrastination** et de **gamifier la lutte contre les distractions** grâce à des statistiques détaillées et des achievements sarcastiques.

**Le problème :** On sous-estime massivement le temps qu'on passe sur YouTube, Reddit, Twitter/X, TikTok, Instagram et autres réseaux sociaux quand on devrait travailler.

**La solution :** Un tracker simple et drôle qui comptabilise chaque visite sur ces sites, calcule le temps perdu, et débloque des achievements aussi drôles que déprimants.

---

## Product Backlog

| ID | User Story | MoSCoW | Statut |
|----|-----------|--------|--------|
| US-01 | En tant qu'utilisateur, je veux cliquer sur un bouton pour comptabiliser une visite sur un site de procrastination afin de suivre mes distractions | **M** (Must) | ✅ Livré |
| US-02 | En tant qu'utilisateur, je veux voir le nombre total de procrastinations afin d'avoir une vue d'ensemble de mon comportement | **M** (Must) | ✅ Livré |
| US-03 | En tant qu'utilisateur, je veux voir des statistiques par site afin de savoir quel réseau social me distrait le plus | **M** (Must) | ✅ Livré |
| US-04 | En tant qu'utilisateur, je veux voir le temps total estimé perdu afin de réaliser l'impact réel de ma procrastination | **S** (Should) | ✅ Livré |
| US-05 | En tant qu'utilisateur, je veux débloquer des achievements basés sur mon nombre de procrastinations afin de gamifier l'expérience (même si c'est triste) | **S** (Should) | ✅ Livré |
| US-06 | En tant qu'utilisateur, je veux pouvoir réinitialiser mes statistiques afin de repartir à zéro (et me mentir à moi-même) | **S** (Should) | ✅ Livré |
| US-07 | En tant qu'utilisateur, je veux voir des citations motivationnelles/démotivantes qui changent afin de me rappeler que je devrais bosser | **C** (Could) | ✅ Livré |
| US-08 | En tant qu'utilisateur, je veux que mes données persistent entre les sessions afin de ne pas perdre mon historique de procrastination | **C** (Could) | ⏳ En cours |
| US-09 | En tant qu'utilisateur, je veux des graphiques visuels (chart.js) montrant l'évolution de ma procrastination dans le temps | **C** (Could) | ❌ Reporté |
| US-10 | En tant qu'utilisateur, je veux recevoir une notification desktop quand je procrastine trop afin d'être rappelé à l'ordre | **W** (Won't) | ❌ Reporté |

---

## Definition of Done

Une User Story est considérée comme terminée quand :

- ☑ Le code est fonctionnel et testé manuellement
- ☑ L'interface est responsive et utilisable sur mobile
- ☑ Le design respecte la charte graphique (gradient violet, cards arrondies)
- ☑ Le code est commité sur GitHub par le membre responsable
- ☑ Le README est mis à jour pour refléter l'US livrée

---

## Ce qui a été livré (MVP)

### 🚀 Comment lancer le projet :

```bash
# Cloner le repo
git clone https://github.com/JulieMontoux/ShouldBeWorking.git

# Ouvrir le fichier HTML
# Méthode 1 : Double-clic sur index.html
# Méthode 2 : Live Server dans VSCode
# Méthode 3 : python -m http.server 8000
```

Accéder à l'application : `http://localhost:8000` (si serveur local) ou directement via le fichier HTML.

---

## Nos décisions techniques

### Stack choisie :

- **HTML/CSS/JavaScript vanilla** : Pas de framework pour rester simple et léger
- **Pas de backend** : Application 100% frontend, fonctionne offline (une fois chargée)
- **localStorage** (prévu pour v2) : Persistance côté client sans base de données

### Pourquoi ce choix ?

- ✅ Déploiement ultra-simple (un seul fichier HTML)
- ✅ Pas de dépendances, pas de build
- ✅ Fonctionne partout (desktop, mobile, tablette)
- ✅ Parfait pour un MVP à livrer en 2h30

### Décisions techniques importantes :

1. **Tout dans un fichier** : HTML + CSS + JS inline pour faciliter le déploiement et le partage
2. **Gradient violet/mauve** : Charte graphique cohérente et moderne (#667eea → #764ba2)
3. **Achievements codés en dur** : Array d'objets avec seuils de déclenchement, extensible facilement
4. **Estimation temps = 5 min/visite** : Basé sur des études moyennes de temps passé par session sur les réseaux sociaux

---

## Comment on a utilisé l'IA

## Rétrospective rapide

---

## Statistiques du projet

- **Temps total** : [À compléter après la séance]
- **Commits** : [À compléter après la séance]
- **Lignes de code** : [À compléter après la séance]
- **User Stories livrées** : [À compléter après la séance]
- **Taux de complétion MVP** : [À compléter après la séance]

---

## Liens utiles

- **Démo live** : [À compléter avec le lien GitHub Pages]
- **Repository GitHub** : [À compléter]
- **Issues/Backlog** : [Lien vers les GitHub Issues si utilisées]

---

## Crédits

Projet réalisé dans le cadre du cours **TRME909 – Méthodes Agiles & Management d'équipe** - EISI 2ème année.

**Fait avec ❤️ et beaucoup de procrastination** (ironiquement).