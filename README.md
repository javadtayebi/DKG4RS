# DKG4RS

## DKG4RS: Drug Knowledge Graph for Recommender Systems.

Introduced and employed in:
> https://github.com/javadtayebi/EKGDR

### Features

|||DKG4RS|
| :-------------------: | :------------ | ----------: |
| Disease-Drug Interaction | #Diseases        |      1,229 |
|                       | #Drugs        |      1,509 |
|                       | #Interactions |     6,657 |
|    Knowledge Graph    | #Entities     |      32,672 |
|                       | #Relations    |          28 |
|                       | #Triplets     |   1,441,310 |

- `disease_drug_interactions.txt`
	- disease-drug interactions file
	- Extracted from [repoDB](https://unmtid-shinyapps.net/shiny/repodb/).
	- Each row is a disease with its approved positive (observed/known) interactions with drugs

- `kg_final.txt`
	- Knowledge Graph (KG) triplets file
	- Extracted from [DrugBank(v5.1.9)](https://go.drugbank.com/), [MetaADEDB](http://lmmd.ecust.edu.cn/metaadedb/) (drug side effects), and [PubChem](https://pubchem.ncbi.nlm.nih.gov/) (PubChem substructure fingerprint for drugs).
	- Each row is a triplet in the form of *(head entity, relation, tail entity)*.

- `disease_list.txt`
	- diseases dictionary file
	- Each row is a triplet in the form of *(original ID | name | ID in DKG4RS)*.

- `drug_list.txt`
	- drugs dictionary file
	- Each row is a triplet in the form of *(original ID | name | ID in DKG4RS)*.

- `entity_list.txt`
	- KG entities dictionary file
	- Each row is a triplet in the form of *(original ID | name | ID in DKG4RS)*.

- `relation_list.txt`
	- relations dictionary file
	- Each row is a pair in the form of *(original ID (name) | ID in DKG4RS)*.
