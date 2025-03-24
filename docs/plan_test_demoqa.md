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
