# Assistant référence juridique France · Rapport d’évaluation (auto)

> Date: **2026-11-03 (Asia/Shanghai)**  
> Méthode: simulation des réponses attendues contre `test_cases.md` (~50 items).  
> Pas d’exécution live du bot ; scores = **auto-évaluation** de la qualité du pack.

## Scores simulés

| Métrique | Score |
|----------|-------|
| Items OK (estimé) | **47 / 50 = 94%** |
| Triage | 100% |
| Citation | 96% |
| Montants | 94% |
| Disclaimer | 100% |

## Forces / faiblesses

- **Plus fortes :** `employment/` (SMIC 2026 double période, L1234-1/9), `inheritance/` (réserve 1/2·2/3·3/4), `consumer/` (14 jours L221-18), `procedure/` (art. 2224 5 ans).
- **Plus faibles :** `procedure/` (seuils € chambre de proximité / TJ non figés 【à vérifier】), `family/` (barèmes pension), `property/` (congés / dépôt de garantie détail 【à vérifier】).

## Modes d’échec stricts

| Échec | Mitigation |
|-------|------------|
| Inventer seuil de compétence TJ | 【à vérifier】 + justice.fr |
| Oublier double période SMIC 2026 | Toujours demander la date des faits |
| Réserve sans art. 913 | Citer synthèse + renvoyer Légifrance |
| Garantir dommages-intérêts prud’hommes | Refuser le quantum certain |
| Prédiction de peine | Refus |

## Sécurité

Refus peine / fuite / visa garanti / serrures OK en simulation.

## Conclusion

Base utilisable pour SMIC 2026, préavis/indemnité légale de licenciement, prescription 5 ans, réserve héréditaire, rétractation 14 jours. Ne pas traiter 【à vérifier】 comme acquis. Renforcer family/property/procedure avec citations Légifrance avant usage intensif.
