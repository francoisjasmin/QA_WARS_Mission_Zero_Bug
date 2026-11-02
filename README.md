# 🎮 QA WARS — Mission Zéro Bug

**Version 1.0 — Jeu pédagogique interactif en français**  
**Public :** étudiants en développement logiciel (niveau intermédiaire)  
**Durée indicative :** environ 35 à 45 minutes, selon le rythme de lecture et les reprises  
**Source pédagogique :** *Stratégies de tests*, support de cours de 26 diapositives fourni par l’enseignant.

## 1. Démarrage rapide

1. Décompressez le fichier ZIP dans un dossier de votre choix.
2. Conservez **index.html**, **style.css** et **script.js** dans **le même dossier**.
3. Double-cliquez sur **index.html** pour l’ouvrir dans Chrome ou Edge.
4. Cliquez sur **« DÉMARRER LA MISSION »**.
5. Complétez les six missions dans l’ordre. À la fin, utilisez **« IMPRIMER / ENREGISTRER EN PDF »** pour obtenir votre bilan.

**Aucune installation, connexion, API, bibliothèque externe, compte ou serveur n’est nécessaire.** Le jeu n’émet aucun son. Des illustrations SVG sont intégrées directement au JavaScript : aucun fichier image externe n’est nécessaire.

## 2. Histoire

En 2042, NEXUS SOFTWARE s’apprête à déployer une application critique. L’équipe QA doit organiser les vérifications, débusquer les anomalies et évaluer si le logiciel peut être livré. Le joueur devient un agent QA devant faire des choix responsables.

## 3. Missions et apprentissages

| Mission | Défis | Activités principales | Compétences |
|---|---:|---|---|
| 1 — Le plan de bataille QA | 13 | 9 cartes à classer + 4 questions | Périmètre, moyens, environnements, méthode, données, rôles, criticité et planification |
| 2 — La pyramide de défense | 10 | 6 scénarios à classer + 4 questions | Unitaires, intégration/API, E2E, TDD, BDD, régression, accessibilité |
| 3 — Le laboratoire Gherkin | 5 | 3 scénarios à assembler + 2 questions | Préconditions, valeurs limites, Étant donné / Lorsque / Alors, critères d’acceptation et DoD |
| 4 — Bug Hunters | 6 | 4 achats à tester + 2 rapports de bogues | Observation, diagnostic, sévérité, résultats attendu/obtenu, reproduction |
| 5 — L’IA sous surveillance | 6 | 1 construction de prompt + 5 audits C#/xUnit | Qualité des assertions, ambiguïtés, règles inventées, confidentialité |
| 6 — GO / NO-GO | 7 | 4 décisions de risque + 3 décisions CI/CD | Priorisation par les risques, critères de sortie, sécurité et livraison |
| **TOTAL** | **47** | | |

Les simulations de boutique, de code C#/xUnit et de pipeline CI/CD sont **pédagogiques** : elles reproduisent des résultats prédéfinis pour entraîner le raisonnement. Le jeu **ne compile pas** de C# et **n’exécute pas** un pipeline de production réel.

## 4. Interactions

- **Cartes :** glisser-déposer une carte dans la zone de destination. Alternative : cliquer la carte, puis cliquer sa catégorie (utile au clavier ou sur petit écran).
- **Choix :** cliquer sur une réponse pour la valider.
- **Gherkin :** sélectionner les propositions pour les trois clauses, puis valider.
- **Boutique :** exécuter le scénario et comparer le comportement observé au comportement attendu.
- **Rapports QA :** compléter les quatre champs de reproduction et de qualification du défaut.
- **IA :** sélectionner cinq consignes fiables puis examiner les extraits C# proposés.
- **GO / NO-GO :** simuler la pipeline, choisir la décision **et** sa justification.

## 5. Pointage et rétroaction

- **47 défis ; 4 700 XP maximum.**
- Bonne réponse au **1er essai : 100 XP** ; au **2e : 70 XP** ; au **3e : 40 XP**.
- Après **3 erreurs**, la correction est révélée et le jeu avance : **0 XP** pour ce défi.
- Une erreur coûte **1 bouclier** et **5 points d’intégrité**.
- Une réussite rend **2 points d’intégrité** (maximum 100 %).
- **5 bonnes réponses consécutives** restaurent un bouclier (maximum 3).
- Les boucliers sont renouvelés entre les missions. Atteindre 0 bouclier ne bloque pas définitivement la partie.
- Le rapport final indique les scores par mission, les badges, la maîtrise et des conseils de révision.

**Rang obtenu :** 90 % et plus = Légende QA ; 75 à 89 % = Commandant QA ; 60 à 74 % = Expert QA ; moins de 60 % = Agent QA en progression.

## 6. Exporter le résultat en PDF

Après la mission finale, cliquez sur **« IMPRIMER / ENREGISTRER EN PDF »**. Dans Chrome ou Edge, choisissez la destination **« Enregistrer au format PDF »**. Le bilan s’imprime sur fond clair, sans le menu du jeu.

## 7. Notes pour l’enseignant

- Le contenu des questions s’appuie sur le support de cours *Stratégies de tests* fourni.
- La **mission 4** introduit volontairement des comportements défectueux dans la boutique fictive. Ces anomalies sont des cas de test, pas des bogues du jeu.
- La **mission 6** demande un arbitrage GO / NO-GO basé sur les critères et risques documentés. Les scénarios proposent une réponse attendue dans le cadre du jeu, sans prétendre fournir une règle universelle de mise en production.
- Le **temps** est affiché comme indicateur de session, **sans limite** imposée.
- **Aucune sauvegarde automatique :** fermer/recharger l’onglet remet le jeu au début. Pour recueillir une preuve de réalisation, demandez l’export PDF final.
- Les sections `strategy`, `pyramids`, `gherkinScenarios`, `simulatedCases`, `bugReports`, `aiReviews`, `risks` et `releases` dans `script.js` contiennent les contenus pédagogiques modifiables.
- Si vous ajoutez/supprimez des questions, ajustez aussi les totaux dans `COUNTS` et les scénarios correspondants.
- La palette et les animations se trouvent dans `style.css`. Le jeu respecte le réglage système « réduire les animations ».

## 8. Fichiers du projet

- `index.html` : structure HTML et chargement des ressources locales.
- `style.css` : thème cyberpunk, grilles, animations, interface adaptative, impression.
- `script.js` : 47 défis, scénarios, règles, illustrations SVG, score, navigation et résultat.
- `LISEZ-MOI.md` : ce mini-guide (document facultatif pour l’exécution).

**Licence pédagogique :** exemple créé pour ce cours, librement modifiable par l’enseignant.
