# Simulateur — Indépendante complémentaire · Praxis Loten

> Outil interactif bilingue **FR/DE** pour kinésithérapeutes envisageant un statut d'**indépendant complémentaire** au cabinet **Praxis Loten** (Eupen, Belgique).

## 🎯 Objectif

Aider les collègues hospitalières ou hospitaliers à visualiser concrètement, **avant toute décision**, ce que représente un complément d'activité libérale au cabinet :

- Combien resterait-il vraiment en net chaque mois ?
- Comment se ventilent les ponctions (INASTI, IPP marginal, communale Eupen) ?
- Où se cache le piège fiscal du cumul salaire + indépendant ?
- Quel impact concret du déconventionnement vs conventionnement ?
- Quelles charges sont réellement déductibles ?

## 🧮 Ce que ça calcule

- **Volume** : séances de 30 min/semaine × semaines actives → séances/an facturables
- **CA brut cabinet** : volume × tarif moyen (M24 31,64 € conv. / 35 € déco)
- **Rétrocession Praxis Loten** : 20 % plafonné à 700 €/mois (au-delà → 100 % gardé)
- **INASTI** : 20,5 % du bénéfice imposable
- **IPP marginal** : tranches 25 % / 40 % / **45 %** / **50 %** selon revenu cumulé
- **Communale Eupen** : 7 % de l'IPP fédéral
- **Net total en poche** : hôpital + cabinet net

## 📚 Sections pédagogiques

1. Ton profil (situation familiale, enfants à charge)
2. Ton activité hôpital actuelle
3. Ton planning cabinet (séances 30 min/sem)
4. Tarification & nomenclature INAMI + tarifs concrets Praxis Loten
5. Rétrocession au cabinet (20 %/700 €)
6. Tes charges déductibles
7. **Fonctionnement fiscal — comprendre où part ton argent** ⭐
   - 7.1 Le principe du cumul
   - 7.2 Les trois ponctions
   - 7.3 Le piège du cumul marginal (détaillé)
   - 7.4 Calendrier fiscal

## 🛠 Stack technique

- **HTML statique single-file** — entièrement autonome, ~200 Ko
- **Tailwind CSS** (CDN Play)
- **Chart.js 4** (CDN)
- **Inter** + **Fraunces** (Google Fonts)
- **Logo Praxis Loten** embarqué en base64
- Aucun build step, aucun framework SPA — déploiement instantané

## 🌍 Déploiement

Déployé sur **Vercel**. Tout push sur `main` déclenche un redéploiement automatique en ~10 secondes.

## 📐 Sources de données

- **INASTI** : barèmes 2026 (20,5 % jusqu'à 75 024,54 €)
- **INAMI** : convention M/25 indexée +2,72 % au 01/01/2026
- **SPF Finances** : tranches IPP 2026 (25 / 40 / 45 / 50 %)
- **Eupen** : taxe communale 7 % (2026)
- **Barème kilométrique pro 2026** : 0,4280 €/km
- **Tarifs Praxis Loten** : [praxisloten.be/fr/honoraires](https://praxisloten.be/fr/honoraires)

## ⚠️ Avertissement

Outil pédagogique à vocation d'aide à la décision. Les chiffres sont des **estimations** basées sur les barèmes en vigueur en mai 2026. Toute décision engageante (choix conventionnement, montage juridique, achat matériel > 5 000 €) doit être validée avec **un·e comptable de son choix**.

---

**Cabinet** : Praxis Loten · Loten 1, 4700 Eupen, Belgique  
**Site** : [praxisloten.be](https://praxisloten.be)  
**Maintenance** : Philippe Banaszak (PBKINE SRL)
