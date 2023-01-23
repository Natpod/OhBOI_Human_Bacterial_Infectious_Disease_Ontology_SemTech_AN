## Data retrieval and files

Folder corresponding to programmatic access for Data retrieval and Data reformatting pre KG generation and CQ addressing with heterogeneous data sources over OhBOI.

A series of manual postprocessings were made post data retrieval adding URIs to make the data comply with W3C and RDF specifications for KG generation.

| File   |      Description      |  Used in |
|----------|:-------------:|------:|
| `Data_Retrieval_and_Reformatting_PubChem_ChEMBL_Chebi.ipynb` |  Script with programatic access to PubChem, ChEMBL and CHEBI compound information from RESTful API interfaces and reformatting | Data retrieval and reformatting for `substances_chemical_entities.csv` |
| `queriesSPARQL.sparql` | Series of queries performing data acquisition over PathoPhenoDB, Uniprot and NCBO Bioportal SPARQL endpoints | Data retrieval and reformatting for `pathogen_diseasee_phenotypes.csv`, `pathogen_omics.csv`, `country_prevalence_in_time.csv` |
| `Reformatting.ipynb` | Data mergings and reformattings for heterogeneous relational data generation | Data reformatting |
| `pubchem_chembl_chebi.csv` | Table retrieved from RESTful programmatic access in `Data_Retrieval_and_Reformatting_PubChem_ChEMBL_Chebi.ipynb` | Data for `substances_chemical_entities.csv` |