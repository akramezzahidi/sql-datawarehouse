# Conventions de Nommage des Couches de Données

## Principes Généraux

- **Convention** : snake_case (minuscules avec underscores)
- **Langue** : Anglais uniquement
- **Éviter** : Les mots réservés SQL

## Conventions par Couche

### Bronze & Silver

- **Format** : `<sourcesystem>_<entity>`
- **Règle** : Conserver les noms originaux des tables sources
- **Exemple** : `crm_customer_info`

### Gold

- **Format** : `<category>_<entity>`
- **Règle** : Noms métier alignés avec le business
- **Catégories** : 
  - `dim` (dimensions)
  - `fact` (faits)
- **Exemples** :
  - `dim_customers` (table de dimension clients)
  - `fact_sales` (table de faits des ventes)
