# Stratégie de versioning — InduSense
## Code
Toute modification passe par une PR. La PR doit avoir une CI verte : ruff, black, pytest, build.
## Données
Les datasets volumineux sont suivis avec DVC. Git conserve les pointeurs, pas les fichiers lourds.
## Modèle
Les artefacts modèle sont accompagnés de model_metadata.json. Promotion : Candidate -> Staging -> Production ## Secrets
Aucun secret dans Git. Secrets locaux dans .env, secrets CI dans GitHub Actions secrets.