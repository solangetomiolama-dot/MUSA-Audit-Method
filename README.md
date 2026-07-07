MUSA : Méthode Unifiée d'Audit de Sécurité Applicative

Auteure: Solange TOMI OLAMA GABRIELLE  
Mémoire: Standardisation de l'Audit de Sécurité d'une Application basée sur la démarche de l'ANTIC : Cas de GIDOCEP  
Année: 2025-2026  
Structure d'accueil: SOLTEC (Solutions Techniques)

- Présentation

MUSA(Méthode Unifiée d'Audit de Sécurité Applicative) est une démarche standardisée d'audit de sécurité applicative conçue pour le contexte camerounais.

Problématique adressée:

La démarche d'audit de l'ANTIC présente trois lacunes majeures :
1. Manque de reproductibilité: deux auditeurs peuvent obtenir des résultats différents
2. Séparation artificielle entre audit de sécurité et audit fonctionnel
3. Absence de mesure objective de la qualité de l'audit

Solution : MUSA

MUSA répond à ces lacunes par quatre piliers :

| Pilier | Contenu |
|--------|---------|
| **Standards de contenu** | ISO 27001, OWASP ASVS, NIST SP 800-115 |
| **Standards de conduite** | ISO 19011:2018, normes IIA (IPPF) |
| **Innovation mesurable** | Entropie de Shannon \(H\) pour quantifier l'accord inter-auditeurs |
| **Artefacts réutilisables** | 6 fichiers Excel (PT01 à PT06), modèles de rapport en 7 sections |

 Structure du Dépôt
MUSA-Audit-Method/
│
├── README.md # Présentation du projet
├── LICENSE # Licence CC BY-NC-SA
├── .gitignore # Fichiers exclus du versionnement
│
├── Memoire/ # Mémoire complet
│ ├── Memoire-MUSA-TOMI-SOLANGE.pdf
│ └── Memoire-MUSA-TOMI-SOLANGE.docx
│
└── Artefacts-MUSA/ # Les 6 fichiers Excel opérationnels
├── PT01-Phase1-Initiation.xlsx
├── PT02-Phase2a-Audit-Organisationnel.xlsx
├── PT03-Phase2b-Audit-Technique.xlsx
├── PT04-Phase2c-Risques-Maturite.xlsx
├── PT05-Phase3-Rapport.xlsx
└── PT06-Phase5-Suivi.xlsx


Note :Tous les modèles de documents (charte, déclaration d'indépendance, PV, rapport, plan d'actions), guides d'entretien et grilles de référence sont déjà inclus dans les annexes du mémoire.


Description des Artefacts MUSA
- PT01-Phase1-Initiation.xlsx: Phase 1 /Faisabilité, équipe, indépendance, périmètre, criticité, documents, PV lancement 
PT02-Phase2a-Audit-Organisationnel.xlsx:Phase 2a/ Entretiens (3 profils), inspection physique, ISO 27001, entropie PT03-Phase2b-Audit-Technique.xlsx: Phase 2b/ OWASP ASVS, NIST, SAST/DAST, configuration, logique métier 
PT04-Phase2c-Risques-Maturite.xlsx: Phase 2c/ Matrice P×I, CVSS, maturité (6 domaines), entropie globale 
PT05-Phase3-Rapport.xlsx: Phase 3/ Constats consolidés, 5 métriques, plan d'actions, contradictoire 
PT06-Phase5-Suivi.xlsx: Phase 5/ Suivi post-audit, retests, escalade 3 niveaux, archivage


Outils recommandés pour l'audit technique

- Scan réseau: Nmap , Masscan 
- Scan vulnérabilités: Nuclei / OpenVAS, Nikto 
- Test dynamique (DAST): OWASP ZAP, Burp Suite 
- Analyse statique (SAST): SonarQube, Semgrep 
- Injection SQL: SQLMap, Test manuel 


Résultats de l'audit GIDOCEP (cas d'étude)

L'audit de GIDOCEP a permis d'identifier 6 vulnérabilités confirmées** :

| ID | Vulnérabilité | R | Priorité |
|----|---------------|---|----------|
| DAST-001 | Injection SQL sur l'endpoint de recherche | 16 | 🔴 Critique |
| DAST-002 | XSS stockée via le champ libellé | 9 | 🟠 Élevé |
| DAST-003 | IDOR sur l'identifiant d'établissement | 9 | 🟠 Élevé |
| PHY-001 | Mots de passe sur post-it / postes non verrouillés | 9 | 🟠 Élevé |
| DAST-004 | En-têtes HTTP de sécurité absents | 4 | 🟡 Modéré |
| DAST-005 | Divulgation de la bannière serveur | 2 | 🟢 Faible |

Métriques globales :
- Taux de conformité : 34%
- Score de maturité : 29,2% (Niveau 1 - Initial)
- Entropie globale : \(H = 0,317\) → Accord fort, bonne reproductibilité 

Comment utiliser MUSA:

1. Phase 1 : Téléchargez `PT01-Phase1-Initiation.xlsx`, définissez le périmètre
2. Phase 2 : Utilisez les guides d'entretien (Annexes F, G, H du mémoire)
3. Phase 3-5 : Consolidez les constats dans `PT05-Rapport.xlsx`, planifiez le suivi avec `PT06-Suivi.xlsx`

Licence

Ce travail est sous licence Creative Commons CC BY-NC-SA.

Vous êtes autorisé à :
- Partager, copier, distribuer le matériel
- Adapter, modifier, transformer le matériel

Sous les conditions :
- ✅ Attribution : créditer l'auteure
- ❌ Pas d'utilisation commerciale
- ✅ Partage dans les mêmes conditions

Auteure

Solange Gabrielle TOMI OLAMA  
Ingénieur de Conception en Humanités Numériques  
ENSPY - École Nationale Supérieure Polytechnique de Yaoundé  

📧 solangetomiolama@gmail.com 
🔗 [https://github.com/solangetomiolama-dot](https://github.com/solangetomiolama-dot)



Dernière mise à jour : Juillet 2026
