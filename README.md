# Assistant de référence juridique France — Base de connaissances

Base publique **gratuite** de **référence** juridique française pour un Grok Bot unique à triage interne (miroir des packs US/JP/KR/UK/DE).

**Pas un conseil juridique. Pas un avocat.** Les textes et montants changent ; vérifiez toujours [Légifrance](https://www.legifrance.gouv.fr/), [service-public.fr](https://www.service-public.fr/), [justice.fr](https://www.justice.fr/) et consultez un avocat ou l’aide juridictionnelle / une maison de la justice et du droit.

## Contenu

- Droit français **national** ; demander le lieu / tribunal lorsque la compétence, l’aide locale ou un usage territorial compte.
- **11 branches**, chacune avec cinq fichiers : `system_prompt.md`, `knowledge_base.md`, `calculators.md`, `deadlines.md`, `templates.md`.
- Langue par défaut : **français**. Si l’utilisateur écrit en chinois ou en anglais, répondre dans cette langue — **garder les noms de codes et articles en français**.

## Branches

| Dir | Sujet |
|-----|--------|
| `family/` | Famille / divorce / enfants / pension |
| `inheritance/` | Successions / réserve héréditaire |
| `contracts/` | Contrats (formation, exécution) |
| `torts/` | Responsabilité civile (art. 1240 et s.) |
| `property/` | Bail / logement / propriété |
| `employment/` | Travail / SMIC / licenciement |
| `criminal/` | Pénal **droits & procédure seulement** |
| `business/` | Sociétés & propriété intellectuelle |
| `admin/` | Administratif / séjour (**référence seule**) |
| `consumer/` | Consommation & en ligne / rétractation |
| `procedure/` | Procédure civile / tribunal judiciaire |

## Assemblage du Bot

1. Coller / attacher `bot_master_prompt.md` comme Instructions.
2. Attacher les cinq fichiers de chaque branche comme knowledge.
3. Ne pas attacher `test_cases.md` / `eval_report.md` en production sauf QA.

## Règle de vérification

Citer uniquement des sources officielles. Code + article + date d’effet / de consultation. Non vérifié = **`【à vérifier】` / `[TO VERIFY]`**. Ne jamais inventer articles, euros ou arrêts.

## Chiffres vérifiés (consultation 2026-11-03 Asia/Shanghai)

| Sujet | Valeur | Source |
|-------|--------|--------|
| SMIC horaire 1.1–31.5.2026 | **12,02 €** | service-public / INSEE / Urssaf |
| SMIC horaire dès 1.6.2026 | **12,31 €** | idem |
| SMIC mensuel 35 h dès 1.6.2026 | **1 867,02 €** | idem |
| Préavis licenciement ≥2 ans | **2 mois** | C. trav. L1234-1 |
| Préavis 6 mois–<2 ans | **1 mois** | L1234-1 |
| Indemnité légale ouverture | **8 mois** CDI | L1234-9 |
| Prescription de droit commun | **5 ans** | art. 2224 C. civ. |
| Réserve 1 / 2 / 3+ enfants | **1/2 · 2/3 · 3/4** | art. 913 C. civ. (synthèse) |
| Rétractation distance | **14 jours** | C. consom. L221-18 |

## Avertissement (chaque réponse)

**Information de référence uniquement.** **Pas un conseil juridique**, l’assistant **n’est pas avocat** ; consulter un **avocat** ou l’**aide juridictionnelle**.

## Licence / coût

Matériels de référence publics gratuits. Aucune affiliation commerciale. Pas de push de dépôt prévu.

Révision: 2026-11-03 (Asia/Shanghai)
