1 - ✅ Récupérer le projet vu dans PluralSight : https://github.com/Daniel-Krzyczkowski/Globomantics-Games et le mettre dans son GitHub
2 - ✅ Récupérer son projet en local
3 - ✅ Sur la branche main, supprimer les fichiers et répertoires suivants (mais les garder à disposition)
    .github/workflows/codeql
    .github/workflows/codeql-analysis.yml
    .github/workflows/snyk-license-scanning.yml
    .github/workflows/pre-merge-build-validation.yml
4 - ✅ Dans le fichier de workflow, supprimer l'étape de CD (Déploiement Continue)
4bis - Réécrire l'historique Git pour ne faire apparaitre que ses propres commits
5 - ✅ Créer les branches manquantes définies dans notre workflow d'équipe (develop & recette)
6 - ✅ Pousser les modifications locales dans le dépôt GitHub
7 - ✅ Activation Secret Scanning
8 - ✅ Activation Dependabot
9 - ✅ Sur la branche develop en local, mettre en place les régles d'exécution des branches, puis pousser sur le dépôt GitHub
10 - ✅ Pull Request develop vers recette, synchro branche locale recette
11 - Pull Request recette vers main, synchro branche locale main
12 - Activation CodeQL (et si besoin, reprendre les workflows supprimés plus tôt dans la branche locale develop)
13 - Création d'un job de vérification joué en premier dans le pipeline, et dont CodeQL aura besoin pour se lancer
14 - Répercuter les changements sur les autres branches via PR, voir les comportements, remarques et suggestions
15 - ✅ Protéger les branches recette & main
16 - Dans le workflow, faire dépendre les étapes du CI au résultat de CodeQL
17 - Répercuter les changements sur les autres branches via PR, voir les comportements, remarques et suggestions
18 - Ajouter un job dans le pipeline après le CI pour construire des releases en fonction d'un tag défini (SemVer, 0.1.0 pour le premier)
        branche develop construit un draft de release
        branche recette construit une prerelease
        branche main construit une release définitive
19 - Répercuter les changements sur les autres branches via PR, voir les comportements, remarques et suggestions