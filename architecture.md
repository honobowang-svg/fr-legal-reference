# Assistant de référence juridique France · Architecture (triage interne)

> Workspace: `/workspace/global-law-agents/fr/`  
> Référence juridique publique gratuite (pas un conseil).  
> Un seul Bot à routage interne — **pas** onze bots.  
> Révision: 2026-11-03 (Asia/Shanghai)

---

## 1. Objectifs

1. Miroir US/JP/KR/UK/DE : master + 11 branches × 5 fichiers.
2. Triage faits + catégorie ; noms de codes en français même si la réponse est CN/EN.
3. Pénal = droits/procédure ; séjour = référence seule (pas de garantie de titre).
4. Pas d’invention ; écarts **`【à vérifier】`**.
5. Double période SMIC 2026 (avant / après 1er juin) toujours distinguée.

---

## 2. Couches d’exécution

| Couche | Fichier(s) | Rôle |
|--------|------------|------|
| Instructions | `bot_master_prompt.md` | Persona, triage, refus, disclaimer |
| Playbooks | `*/system_prompt.md` | Périmètre, refus, flux |
| Savoir | `*/knowledge_base.md` | Textes / portails |
| Calculateurs | `*/calculators.md` | SMIC, indemnité, réserve |
| Délais | `*/deadlines.md` | Prescription / procédure |
| Modèles | `*/templates.md` | Checklists / lettres |
| QA (optionnel) | `test_cases.md`, `eval_report.md` | Hors knowledge utilisateur |

---

## 3. Séquence de triage

```
Question
  → Faits / lieu / période (ex. SMIC avant/après 1.6.2026) si besoin
  → une des 11 catégories
  → Pack de branche (5 fichiers)
  → Réponse citée (code + article + date) + avertissement
```

---

## 4. Politique de couverture

| Niveau | Contenu |
|--------|---------|
| Priorité | SMIC 2026, L1234-1/9, art. 2224, réserve art. 913, L221-18 14 jours |
| Référence | Autres branches avec portails officiels + 【à vérifier】 |
| Hors scope | Prédiction de peine, soustraction, garantie de visa, montants de contentieux inventés |

---

## 5. Garde-fous

- Pas de prédiction de peine / soustraction / destruction de preuves.
- Pas de garantie de titre de séjour.
- Pas de faux numéros d’articles.
- Disclaimer à chaque réponse.
- Expulsion de fait (serrures) : refuser ; voies judiciaires.

---

## 6. Maintenance

Mettre à jour citations + dates ; recalculer tableaux SMIC à chaque revalorisation ; vérifier seuils de compétence TJ / proximité sur justice.fr ; ajouter un cas de non-régression dans `test_cases.md`.
