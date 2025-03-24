# Plan de Test - DemoQA Text Box  
**Date** : 24/05/2024  
**Auteur** : IKHEBASSENE 

## 1. Objectifs  
- Valider le formulaire "Text Box" de DemoQA :  
  - Fonctionnalité : Affichage des données après soumission.  
  - Erreurs : Messages pour emails invalides.  

## 2. Outils  
- **Selenium WebDriver** (Python)  
- **Pytest** pour l'exécution et les rapports.  
- **GitHub Issues** pour le suivi des bugs.  

## 3. Cas de Test  
| ID  | Description           | Données de Test         | Résultat Attendu          |  
|-----|-----------------------|-------------------------|---------------------------|  
| TC1 | Saisie valide         | Nom="John", Email="john@test.com" | Données affichées en bas. |  
| TC2 | Email invalide        | Email="john"            | Bordure rouge du champ.   |  

## 4. Environnement  
- OS : Windows 11  
- Navigateurs : Chrome 125+  
- URL : https://demoqa.com/text-box
## 5. Cas de Test Détaillés

| ID  | Description           | Étapes                                                                 | Données de Test         | Résultat Attendu          | Statut     |
|-----|-----------------------|-----------------------------------------------------------------------|-------------------------|---------------------------|------------|
| TC1 | Saisie valide         | 1. Remplir "Full Name"<br>2. Remplir "Email" valide<br>3. Cliquer "Submit" | Nom="John Doe"<br>Email="john@test.com" | Données affichées en bas. | ✅ Validé  |
| TC2 | Email invalide        | 1. Remplir "Email" avec "john"<br>2. Cliquer "Submit"                     | Email="john"            | Bordure rouge du champ.   | ✅ Validé  |
| TC3 | Champ "Full Name" vide| 1. Laisser "Full Name" vide<br>2. Cliquer "Submit"                        | Nom=""                  | Le formulaire bloque l'envoi. | 🔄 À tester |
## 6. Métriques
- **Couverture des tests** : 85% (3/4 fonctionnalités testées).  
- **Taux de défauts** : 1 défaut critique (TC3 non validé).  
- **Temps d'exécution** : 2 minutes (tests automatisés).  
