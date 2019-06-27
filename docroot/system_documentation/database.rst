:github_url: https://github.com/PATRIC3/p3_docs/blob/master/docroot/system_documentation/database.rst

Database
=========

Data Types
----------

(See Data Section for list and description of data types supported)

Database Schema
----------------

The primary data store for PATRIC is a distributed SolrCloud database. The SolrCloud configuration allows "collections" to be defined using xml schema files. These collection definitions, combined with the data indexes are deployed on one or more SolrCloud hosts. Multiple machines can utilize the same set of collections and/or indexes to address scalability, high availability and higher throughput and query performance by allowing more concurrent queries. 

Below is a list of the collections and the main fields/attributes available in each collection. Refer to https://github.com/PATRIC3/patric_solr_cloud for the most updated configurations and schemas.

**Solr Cores/Collections:**

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
