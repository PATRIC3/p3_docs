:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/system_documentation/database.rst

Database
=========

Data Types
----------

(See Data Section for list and description of data types supported)

Database Schema
----------------

The primary data store for PATRIC is a Solr database. The Solr configuration allows "cores" to be defined in schema xml files. These core definitions, combined with the data indexes are deployed on a Solr host, allowing queries for those cores to be handled. Multiple machines can utilize the same set of cores and indexes to address availability and to scale to allow more concurrent queries to be handled. Below is a list of the cores and the main fields available for each core. Refer to https://github.com/PATRIC3/patric_solr for the most updated configurations and schemas.

**Solr Cores:**

- antibiotics
- enzyme_class_ref
- feature_sequence
- gene_ontology_ref
- genome
- genome_amr
- genome_feature
- genome_sequence
- id_ref
- misc_niaid_sgc
- model_complex_role
- model_compound
- model_reaction
- model_template_biomass
- model_template_reaction
- pathway
- pathway_ref
- ppi
- protein_family_ref
- sp_gene
- sp_gene_evidence
- sp_gene_ref
- structured_assertion
- subsystem
- subsystem_ref
- taxonomy
- transcriptomics_experiment
- transcriptomics_gene
- transcriptomics_sample


Data Dictionary
---------------
**[NEEDED]**
