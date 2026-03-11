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
| US-08 | En tant qu'utilisateur, je veux que mes données persistent entre les sessions afin de ne pas perdre mon historique de procrastination | **C** (Could) | ✅ Livré |
| US-09 | En tant qu'utilisateur, je veux des graphiques visuels (chart.js) montrant l'évolution de ma procrastination dans le temps | **C** (Could) | ✅ Livré |
| US-10 | En tant qu'utilisateur, je veux recevoir une notification desktop quand je procrastine trop afin d'être rappelé à l'ordre | **W** (Won't) | ✅ Livré |

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

### ✅ Fonctionnalités démo-ables :

1. **Compteur interactif** : 6 boutons cliquables (YouTube, Twitter/X, Reddit, Instagram, TikTok, Facebook)
2. **Affichage en temps réel** : Le compteur total se met à jour instantanément
3. **Statistiques détaillées** : Tableau récapitulatif par site avec nombre de visites
4. **Calcul du temps perdu** : Estimation basée sur 5 minutes moyenne par visite
5. **Système d'achievements** : 
   - "Première fois" (1 procrastination)
   - "Rookie" (10 procrastinations)
   - "Habitué" (25 procrastinations)
   - "Accro" (50 procrastinations)
   - "Maître Procrastinateur" (100 procrastinations)
   - "YouTube Addict" (20 visites YouTube)
   - "Papillon Social" (visiter tous les sites)
6. **Bouton reset** : Remise à zéro complète avec confirmation
7. **Interface responsive** : Fonctionne sur desktop, tablette et mobile

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

## Ce qui a été reporté et pourquoi

### ❌ Reporté (Won't Have) :

- Rien, le problème trop fort.

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

### ✅ Prompts qui ont bien marché :

```
"Crée-moi un compteur HTML/CSS/JS avec 6 boutons pour tracker 
les visites sur YouTube, Twitter, Reddit, Instagram, TikTok, Facebook. 
Design moderne avec gradient violet. Tout dans un seul fichier."
```

```
"Ajoute un système d'achievements qui se débloquent à certains seuils 
(1, 10, 25, 50, 100 procrastinations). Affiche-les avec des emojis 
et graye-les tant qu'ils ne sont pas débloqués."
```

```
"Calcule le temps total perdu en supposant 5 minutes par visite. 
Affiche-le en minutes au-dessus des stats."
```

### ❌ Ce qui n'a pas marché du premier coup :

- L'IA proposait initialement des fichiers séparés (HTML/CSS/JS) → on a dû demander explicitement "tout dans un fichier"
- Le calcul du temps était en heures décimales (3.5h) → on a demandé un affichage en heures + minutes
- Les achievements n'étaient pas automatiquement cochés → on a dû préciser le système de vérification au clic

### 🤖 Ce que l'IA n'a pas su faire :

- Proposer des achievements vraiment drôles/sarcastiques
- Suggérer des améliorations UX pertinentes (c'est notre job de PO/designers)

---

## Rétrospective rapide

### ✅ Ce qui a bien marché :

- **Communication fluide** : Le PO validait chaque US avant le merge
- **Commits clairs** : Convention `feat:`, `fix:`, `docs:` respectée à 100%
- **Scope réaliste** : On a priorisé correctement, les 3 Must Have livrés en 1h30
- **IA efficace** : Gain de temps énorme sur le code boilerplate et le CSS

### 🔄 Ce qu'on ferait différemment :

- **Découper plus tôt** : On aurait dû splitter US-05 (achievements) en 2 US (système de base + achievements avancés)
- **Tester sur mobile plus tôt** : On a découvert un bug de responsive en fin de séance
- **Prévoir du buffer** : Les 30 dernières minutes étaient rushées, on aurait dû garder 45 min de marge

### 🚀 Ce qu'on garderait pour le prochain projet :

- Le système de MoSCoW : super efficace pour prioriser
- L'utilisation de l'IA pour le code répétitif (boutons, stats, CSS)
- La règle "1 commit par US livrée" : clarté totale dans l'historique Git
- Le README mis à jour en continu : on n'a pas eu à le rusher à la fin

---

## Statistiques du projet

- **Temps total** : ~2h30
- **Commits** : 33
- **Lignes de code** : ~1950 lignes (HTML + CSS + JS)
- **User Stories livrées** : 10/10
- **Taux de complétion MVP** : 100% (3/3 Must Have)

---

## Liens utiles

- **Repository GitHub** : [ShouldBeWorking](https://github.com/JulieMontoux/ShouldBeWorking)
- **Issues/Backlog** : [Lien vers les GitHub Issues](https://github.com/JulieMontoux/ShouldBeWorking/issues?q=is%3Aissue)

---

## Crédits

Projet réalisé dans le cadre du cours **TRME909 – Méthodes Agiles & Management d'équipe** - EISI M2.

**Fait avec ❤️ et beaucoup de procrastination** (ironiquement).
