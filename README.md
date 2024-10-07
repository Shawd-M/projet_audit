# Groupe de joseph_d 1036947

# Audit de Sécurité - FramaFTP

## Objectifs

### 1. Repérage
- **Description** : Cartographier les services exposés sur les serveurs cibles.

### 2. Identification de Vulnérabilités
- **Description** : Rechercher et identifier les vulnérabilités sur les serveurs, d'abord en boîte noire (sans accès utilisateur), puis en boîte grise (avec compte utilisateur).

### 3. Exploitation de Vulnérabilités
- **Description** : Exploiter les vulnérabilités identifiées pour vérifier leur impact réel sur la sécurité.

### 4. Prévention
- **Description** : Identifier et signaler les mauvaises pratiques et comportements pouvant mener à des risques de sécurité.

### 5. Recommandations
- **Description** : Proposer des solutions et recommandations pour corriger les vulnérabilités découvertes et améliorer la sécurité de l'infrastructure.

## Consignes

Le leader du libre **FramaFTP** propose un service de stockage gratuit et accessible à tous. En tant que consultant en sécurité, il vous est demandé de réaliser un **audit de sécurité** sur leur infrastructure.

- **Mode d'audit** : Test d'intrusion en "boîte noire", commençant par la machine exposée aux clients à l'adresse suivante : `172.16.239.10:student:null`.
- **Objectif principal** : Réaliser un rapport détaillant les vulnérabilités découvertes et fournir des recommandations pour corriger ces failles.

## Rapports attendus

- **Rapport d'intrusion** : Résumer les vulnérabilités découvertes, leur gravité, et proposer des solutions.
- **Réunion de restitution** : Support de présentation pour expliquer les résultats de l'audit et les recommandations.

## Règles et Limitations

Seuls les outils suivants sont autorisés pour l'audit :

- Scanner de ports : `nmap`
- Proxy HTTP : `Burp Proxy`
- Clients natifs de serveurs (ex. : clients MySQL, MSSQL, SSH, FTP, etc.)
- Outils de cracking de mots de passe : `John The Ripper`, `patator.py` (avec dictionnaires de bruteforce)

**Interdictions :**

- Aucun outil d'exploitation automatique n'est autorisé (ex. : `Nessus`, `Nexpose`, `Acunetix`, `SQLMap`, etc.).
- Les scripts `nmap` et options comme `-sC`, `--script=*` ou `-A` sont strictement interdits.

## Note

Obtenir un accès root ne signifie pas forcément que vous avez tout exploré. Il est crucial d'essayer d'exploiter toutes les failles possibles pour fournir un audit complet.
