# Guide de Contribution - Contributing Guide

Merci de votre intérêt pour contribuer à l'Ultimate Multi-Module Indicator v6! 🎉

Thank you for your interest in contributing to the Ultimate Multi-Module Indicator v6! 🎉

## 🌍 Langues / Languages

Ce projet accepte les contributions en français et en anglais.
This project accepts contributions in French and English.

---

## 📋 Table des Matières / Table of Contents

1. [Comment Contribuer](#comment-contribuer)
2. [Types de Contributions](#types-de-contributions)
3. [Processus de Contribution](#processus-de-contribution)
4. [Standards de Code](#standards-de-code)
5. [Documentation](#documentation)
6. [Questions et Support](#questions-et-support)

---

## 🤝 Comment Contribuer / How to Contribute

### Avant de Commencer / Before Starting

1. **Lisez la documentation existante**
   - [README.md](README.md)
   - [DOCUMENTATION.md](DOCUMENTATION.md)
   - [FAQ.md](FAQ.md)

2. **Vérifiez les issues existantes**
   - Recherchez si votre suggestion/bug a déjà été signalé
   - Évitez les doublons

3. **Testez votre contribution**
   - Sur compte démo TradingView
   - Sur plusieurs actifs et timeframes
   - Vérifiez qu'il n'y a pas d'erreurs

---

## 🎯 Types de Contributions / Types of Contributions

### ✅ Contributions Acceptées / Accepted Contributions

#### 1. Corrections de Bugs / Bug Fixes
- Erreurs dans le code Pine Script
- Problèmes d'affichage
- Bugs dans les calculs
- Erreurs de documentation

#### 2. Améliorations de Code / Code Improvements
- Optimisation des performances
- Refactoring pour meilleure lisibilité
- Ajout de commentaires utiles
- Amélioration de la structure

#### 3. Nouvelles Fonctionnalités / New Features
- Nouveaux indicateurs techniques
- Patterns de chandeliers
- Nouveaux types d'alertes
- Améliorations du tableau de bord
- Nouveaux modules d'analyse

#### 4. Documentation / Documentation
- Corrections de typos
- Amélioration des explications
- Traductions
- Nouveaux exemples
- Nouveaux guides

#### 5. Configurations / Configurations
- Nouvelles configurations optimisées
- Templates pour nouveaux actifs
- Stratégies testées et validées

#### 6. Tests / Testing
- Tests sur différents marchés
- Backtesting et résultats
- Cas d'usage documentés

### ❌ Contributions Non Acceptées / Not Accepted Contributions

- Code malveillant ou dangereux
- Modifications qui cassent la compatibilité
- Changements non documentés
- Code non testé
- Spam ou contenu inapproprié

---

## 🔄 Processus de Contribution / Contribution Process

### 1. Fork et Clone

```bash
# Fork le repository sur GitHub
# Clonez votre fork
git clone https://github.com/VOTRE-USERNAME/Pinev6AI.git
cd Pinev6AI

# Ajoutez le repository original comme remote
git remote add upstream https://github.com/davidnault0/Pinev6AI.git
```

### 2. Créez une Branche / Create a Branch

```bash
# Créez une branche descriptive
git checkout -b feature/nom-de-votre-feature
# ou
git checkout -b fix/nom-du-bug
# ou
git checkout -b docs/amelioration-doc
```

**Nommage des branches / Branch naming:**
- `feature/` - Nouvelles fonctionnalités
- `fix/` - Corrections de bugs
- `docs/` - Documentation
- `refactor/` - Refactoring
- `test/` - Tests

### 3. Effectuez vos Modifications / Make Your Changes

- Modifiez le code
- Testez vos modifications
- Documentez vos changements
- Suivez les standards de code

### 4. Committez / Commit

```bash
# Ajoutez vos fichiers
git add .

# Committez avec un message descriptif
git commit -m "Type: Description courte

Description détaillée si nécessaire
- Point 1
- Point 2

Refs #numero-issue (si applicable)"
```

**Format des messages de commit / Commit message format:**
- `Feature: Ajout de l'indicateur Stochastic`
- `Fix: Correction du calcul RSI en période 7`
- `Docs: Mise à jour du guide d'installation`
- `Refactor: Amélioration de la fonction f_ma`
- `Test: Ajout d'exemples pour le Forex`

### 5. Poussez et Créez une Pull Request / Push and Create Pull Request

```bash
# Poussez votre branche
git push origin votre-branche

# Allez sur GitHub et créez une Pull Request
```

**Template de Pull Request:**

```markdown
## Type de Changement
- [ ] Bug fix
- [ ] Nouvelle fonctionnalité
- [ ] Documentation
- [ ] Refactoring
- [ ] Configuration

## Description
Décrivez vos changements en détail...

## Motivation
Pourquoi cette modification est-elle nécessaire?

## Tests Effectués
- [ ] Testé sur compte démo
- [ ] Testé sur [actifs]: ...
- [ ] Testé sur [timeframes]: ...
- [ ] Aucune erreur dans l'éditeur Pine

## Screenshots (si applicable)
[Ajoutez des captures d'écran si pertinent]

## Checklist
- [ ] Mon code suit les standards du projet
- [ ] J'ai commenté les parties complexes
- [ ] J'ai mis à jour la documentation
- [ ] J'ai testé mes changements
- [ ] Les changements ne cassent rien
```

### 6. Review et Feedback

- Un maintainer reviewera votre PR
- Répondez aux commentaires
- Effectuez les modifications demandées
- Une fois approuvé, votre PR sera mergée

---

## 📝 Standards de Code / Code Standards

### Pine Script

#### Style
```pinescript
// Utilisez des noms de variables descriptifs
float movingAverage20 = ta.ema(close, 20)  // ✅ Bon
float ma = ta.ema(close, 20)                // ❌ Moins clair

// Commentez les sections importantes
// ============================================================================
// SECTION: DESCRIPTION
// ============================================================================

// Utilisez des espaces pour la lisibilité
if condition
    value = 1
else
    value = 0

// Indentez avec 4 espaces
```

#### Conventions de Nommage
- **Variables**: camelCase (`movingAverage`, `rsiValue`)
- **Constantes**: UPPER_SNAKE_CASE (`MAX_BARS`, `DEFAULT_PERIOD`)
- **Fonctions**: préfixe `f_` puis camelCase (`f_calculateMA`, `f_getTrend`)
- **Paramètres d'entrée**: camelCase avec suffixe descriptif (`maPeriod1`, `colorBullish`)

#### Commentaires
```pinescript
// Commentaire simple pour ligne unique

// Commentaire sur plusieurs lignes pour
// expliquer un concept plus complexe

// --- Section de paramètres ---
// Commentaire de sous-section
```

### Documentation

#### Markdown
- Utilisez les headers appropriés (`#`, `##`, `###`)
- Ajoutez des exemples de code
- Incluez des emoji pour rendre plus visuel 🎯
- Liens vers autres documents quand pertinent

#### Langue
- Documentation principale: Français et Anglais
- Code et commentaires: Français de préférence
- Variables: Anglais pour compatibilité

---

## 📚 Documentation / Documentation

### Fichiers à Mettre à Jour / Files to Update

Selon votre contribution, mettez à jour:

1. **README.md** - Si fonctionnalité majeure
2. **DOCUMENTATION.md** - Si nouvelle feature ou paramètre
3. **GUIDE_RAPIDE.md** - Si impact sur l'utilisation basique
4. **EXEMPLES.md** - Si nouveau cas d'usage
5. **CONFIGURATIONS.md** - Si nouvelle configuration
6. **FAQ.md** - Si réponse à question fréquente
7. **CHANGELOG.md** - TOUJOURS pour tout changement

### Format de la Documentation

```markdown
## Titre de la Section

### Sous-section

Description claire et concise.

#### Exemple
\`\`\`pinescript
// Code d'exemple
float example = ta.ema(close, 20)
\`\`\`

**Note importante:** Texte d'avertissement
**Astuce:** Conseil utile
```

---

## 🧪 Tests / Testing

### Tests Requis / Required Testing

Avant de soumettre:

1. **Pas d'erreurs dans l'éditeur Pine**
   - Code compile sans erreur
   - Aucun warning critique

2. **Test Visuel**
   - Indicateur s'affiche correctement
   - Couleurs et labels visibles
   - Tableau de bord lisible

3. **Test Fonctionnel**
   - Tous les signaux fonctionnent
   - Paramètres ajustables
   - Alertes déclenchables

4. **Test Multi-Actifs**
   - Testez sur au moins 2-3 actifs différents
   - Actifs de volatilités différentes

5. **Test Multi-Timeframes**
   - Testez sur au moins 2-3 timeframes
   - Du court terme au long terme

### Rapporter les Résultats / Report Results

Incluez dans votre PR:
```markdown
## Tests Effectués

### Actifs Testés
- BTC/USD (crypto)
- EUR/USD (forex)
- AAPL (action)

### Timeframes Testés
- 15M, 1H, 4H, 1D

### Résultats
- ✅ Aucune erreur
- ✅ Affichage correct
- ✅ Signaux générés
- ⚠️ Problème mineur sur [détails]
```

---

## 💡 Suggestions de Contributions / Contribution Ideas

### Débutants / Beginners
- Corrections de typos dans la documentation
- Ajout d'exemples supplémentaires
- Traduction de parties de doc
- Tests et rapports de bugs
- Amélioration des commentaires dans le code

### Intermédiaires / Intermediate
- Nouvelles configurations optimisées
- Nouveaux exemples de stratégies
- Améliorations de la documentation
- Optimisation de code existant
- Ajout de nouveaux types d'alertes

### Avancés / Advanced
- Nouveaux indicateurs techniques
- Patterns de chandeliers
- Modules d'analyse avancés
- Système de backtesting
- Optimisation des performances
- Refactoring majeur

---

## ❓ Questions et Support / Questions and Support

### Avant de Demander / Before Asking

1. Lisez la [FAQ](FAQ.md)
2. Cherchez dans les issues existantes
3. Consultez la [Documentation](DOCUMENTATION.md)

### Où Demander / Where to Ask

- **Questions générales**: Ouvrez une issue avec label `question`
- **Bugs**: Ouvrez une issue avec label `bug`
- **Features**: Ouvrez une issue avec label `enhancement`
- **Discussion**: Utilisez les Discussions GitHub

### Template d'Issue pour Bug

```markdown
## Description du Bug
[Description claire et concise]

## Étapes pour Reproduire
1. ...
2. ...
3. ...

## Comportement Attendu
[Ce qui devrait se passer]

## Comportement Actuel
[Ce qui se passe réellement]

## Environnement
- Actif: [ex: BTC/USD]
- Timeframe: [ex: 1H]
- Configuration: [paramètres utilisés]

## Screenshots
[Si applicable]
```

---

## 🏆 Reconnaissance / Recognition

Les contributeurs seront reconnus dans:
- Le fichier [CHANGELOG.md](CHANGELOG.md)
- Les notes de version
- La section "Contributeurs" du README

---

## 📜 Code de Conduite / Code of Conduct

### Nos Engagements / Our Pledge

Nous nous engageons à:
- Créer un environnement accueillant et inclusif
- Respecter tous les contributeurs
- Accepter les critiques constructives
- Se concentrer sur ce qui est le mieux pour la communauté

### Comportements Attendus / Expected Behavior

✅ Soyez respectueux et courtois
✅ Acceptez les feedbacks constructifs
✅ Concentrez-vous sur les faits, pas les personnes
✅ Aidez les nouveaux contributeurs

❌ Pas de harcèlement ou comportement offensant
❌ Pas de spam ou auto-promotion excessive
❌ Pas de trolling ou commentaires destructifs

---

## 📄 License

En contribuant, vous acceptez que vos contributions soient sous la même [License MIT](LICENSE) que le projet.

---

## 🙏 Merci / Thank You

Merci de contribuer à rendre cet indicateur meilleur pour toute la communauté!
Thank you for contributing to make this indicator better for the whole community!

Des questions? N'hésitez pas à ouvrir une issue!
Questions? Don't hesitate to open an issue!

---

**Bon coding! / Happy coding!** 🚀
