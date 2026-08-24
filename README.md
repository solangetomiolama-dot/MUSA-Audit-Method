# \# MUSA - Méthode Unifiée d'Audit de Sécurité Applicative

# 

# \[!\[Licence](https://img.shields.io/badge/Licence-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

# 

# 

# \## 📖 Présentation

# 

# \*\*MUSA\*\* (Méthode Unifiée d'Audit de Sécurité Applicative) est une démarche d'audit innovante qui fusionne l'audit de sécurité et l'audit fonctionnel des applications en une seule mission.

# 

# Développée dans le cadre d'un mémoire d'ingénierie à l'École Nationale Supérieure Polytechnique de Yaoundé (ENSPY), MUSA répond à une contrainte spécifique des PME camerounaises : la nécessité de réaliser un audit complet de leurs applications sans supporter le coût de deux missions distinctes.

# 

# \### 🎯 Objectifs

# 

# \- \*\*Fusionner\*\* les audits de sécurité et fonctionnels en une démarche unique

# \- \*\*Mesurer\*\* l'incertitude et la reproductibilité via l'entropie de Shannon

# \- \*\*Structurer\*\* la mission autour de sept outils standardisés et réutilisables

# \- \*\*Garantir\*\* la conformité avec les référentiels internationaux (ISO 27001, OWASP ASVS, NIST SP 800-115, ISO 19011, normes IIA)

# \- \*\*Valider\*\* l'approche sur un cas concret : GIDOCEP (application développée par SOLTEC)

# 

# \---

# 

# \## 🗂️ Structure du dépôt

MUSA-Audit-Method/

├── 01\_MEMOIRE/ # Le document de référence complet

│ └── TOMI\_OLAMA\_MUSA\_Audit\_2026.pdf

│

├── 02\_OUTILS/ # Les outils opérationnels de la méthode

│ ├── L00\_Aide\_Memoire\_GIDOCEP.docx

│ ├── L01\_Fiche\_Technique\_GIDOCEP.docx

│ ├── L02\_TDR\_GIDOCEP.docx

│ ├── L03\_Documents\_Sollicites\_GIDOCEP.docx

│ ├── L04\_Outil\_Aide\_Audit\_GIDOCEP.xlsx

│ ├── L04\_Outil\_Aide\_Audit\_GIDOCEP - Copie.xlsx

│ ├── L05\_Guide\_Entretien\_GIDOCEP.docx

│ └── L06\_Plan\_Audit\_GIDOCEP.docx

│

├── 03\_GUIDE\_ENTRETIEN/ # Guides d'entretien détaillés

│ ├── Guide\_entretien\_Direction.pdf

│ ├── Guide\_entretien\_Developpeurs.pdf

│ └── Guide\_entretien\_Utilisateurs.pdf

│

├── 04\_REFERENTIELS/ # Référentiels normatifs utilisés

│ ├── Points\_de\_controle\_ISO27001.pdf

│ ├── Checklist\_OWASP\_ASVS.pdf

│ ├── Grille\_NIST\_SP800-115.pdf

│ ├── Correspondance\_ISO19011\_ANTIC.pdf

│ └── Normes\_IIA\_applicables.pdf

│

└── 05\_RAPPORT\_GIDOCEP/ # Application concrète sur GIDOCEP

├── rapport\_audit\_GIDOCEP.pdf

├── Guide\_Explication\_Outil\_Audit\_GIDOCEP.pdf



\---



\## 📚 Les sept outils MUSA (L00 à L06)



| Outil | Intitulé | Fonction |

| :---: | :--- | :--- |

| \*\*L00\*\* | Aide-mémoire de mission | Synthèse des cinq phases, architecture documentaire |

| \*\*L01\*\* | Fiche technique de mission | Cadrage : objectif, périmètre, référentiels, équipe |

| \*\*L02\*\* | Termes de Référence (TDR) | Contexte, objectifs, périmètre, risques préliminaires |

| \*\*L03\*\* | Documents à solliciter | Liste des pièces à collecter en phase préparatoire |

| \*\*L04\*\* | Outil Tableur (NEK/PAS) | Collecte des réponses, calcul entropie, maturité CMMi |

| \*\*L05\*\* | Guide d'entretien fusionné | 41 questions couvrant technique et organisationnel |

| \*\*L06\*\* | Plan d'audit | Programme de travail, calendrier, équipe |



> 💡 \*\*L'Outil Tableur (L04) est le cœur de la méthode.\*\* Il calcule automatiquement :

> - La réponse fusionnée \*\*O/N/PAS\*\* (Conforme / Non Conforme / Zone Grise)

> - L'\*\*entropie de Shannon (H)\*\* par domaine

> - Le niveau de \*\*maturité CMMi\*\* (1 à 5)

> - La \*\*criticité\*\* et l'\*\*échéance\*\* de traitement



\---



\## 🔬 Étude de cas : GIDOCEP



La méthode a été appliquée à \*\*GIDOCEP\*\*, une application développée par \*\*SOLTEC\*\* pour les établissements publics camerounais.



\### Résultats clés de l'audit



| Métrique | Valeur | Interprétation |

| :--- | :--- | :--- |

| Taux de conformité global | 9,5 % | Très faible |

| Entropie globale (H) | \*\*1,267 bits\*\* | \*\*Zone grise critique\*\* |

| Maturité globale CMMi | \*\*Niveau 1 (Initial)\*\* | Absence de processus formalisés |



> 📄 Le rapport d'audit complet est disponible dans `05\_RAPPORT\_GIDOCEP/`.



\---



\## 📖 Référentiels mobilisés



| Référentiel | Domaine | Utilisation |

| :--- | :--- | :--- |

| \*\*ISO/IEC 27001:2022\*\* | Management de la sécurité | 93 contrôles |

| \*\*OWASP ASVS v4.0.3\*\* | Sécurité applicative | 14 catégories, 3 niveaux |

| \*\*NIST SP 800-115\*\* | Tests de sécurité | 3 phases |

| \*\*ISO 19011:2018\*\* | Audit | 7 principes, 5 phases |

| \*\*Normes IIA (IPPF) 2024\*\* | Gouvernance | Indépendance, planification, suivi |



\---



\## 🚀 Comment utiliser ce dépôt



\- \*\*Auditeurs\*\* : lisez le mémoire, étudiez le cas pratique, inspirez-vous des outils

\- \*\*Chercheurs/Étudiants\*\* : explorez la méthode, analysez l'entropie, reproduisez

\- \*\*PME\*\* : comprenez l'enjeu, inspirez-vous du plan d'actions, évaluez votre maturité



\---



\## 👤 Auteure



\*\*TOMI OLAMA Gabrielle Solange\*\*  

Étudiante en Cybersécurité et Investigation Numérique  

ENSPY - Promotion 2025-2026



\---



\## 🤝 Encadrement



| Rôle | Nom | Institution |

| :--- | :--- | :--- |

| Superviseur académique | Dr. TIOGNING DJIOGUE Lauraine | Université de Yaoundé I |

| Encadreur professionnel | Ing. MBOULE Patrick | SOLTEC (RSSI) |

| Superviseur général | Ing. MINKA MI NGUIDJOI Thierry Emmanuel | CONSUPE / ENSPY |



\---



\## 📝 Licence



Ce travail est sous licence \*\*CC BY-NC-SA 4.0\*\*.



\- Partage : copiez, distribuez

\- Adaptation : modifiez, transformez

\- Attribution : créditez l'auteure

\- **Pas d'usage commercial**

\- Partage dans les mêmes conditions



Pour plus d'informations : https://creativecommons.org/licenses/by-nc-sa/4.0/



\---



\## 🔗 Liens utiles



\- \[Dépôt du cours INF3226 - Audit des SI](https://github.com/Maletyon/INF3226/tree/chapitres)

\- \[Site de l'ANTIC](https://www.antic.cm)



\---



**Ce dépôt a été créé dans le cadre d'un mémoire de fin d'études à l'ENSPY. Il est destiné à la recherche, à l'enseignement et à la pratique professionnelle de l'audit des systèmes d'information.**





