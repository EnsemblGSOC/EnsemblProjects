# Work Outline
The data provided in Ensembl (http://www.ensembl.org) provides extensive information about biological features mapped to the genome. The features are also available in other public databases, with different points of reference (eg https://www.ncbi.nlm.nih.gov/refseq/ or https://www.uniprot.org/uniprot/). Depending on the question asked, users might start from different data sets, hence it is important to show the correspondence between the different resources available. This is why we link our data to external resources via a variety of methods, see  https://academic.oup.com/database/article-pdf/doi/10.1093/database/bax020/19231914/bax020.pdf for more detail on the methods. While all the links are stored in the same way, they are not all generated in the same manner and can represent different concepts. For example, we can have identical features in another database, identified by sequence alignment, or added information about a feature, like phenotypes for a gene. We would like to review the data available and how it is stored, to present a clear description of the data and its provenance.

# Project goals
The project will involve the successful student providing an exhaustive list of the data we can link to along with the relevant information for each data source. They will then devise a relational schema designed to store all the data, ensuring the information identified in the first step is captured. The student will be responsible for outlining the tasks involved in this process and implementing said tasks.

# Specifications
## The database layer
The data is currently stored in the so-called xref schema as can be seen here: http://www.ensembl.org/info/docs/api/core/core_schema.html. While this can be used as a starting point, the proposed new schema should be designed around the data to be stored rather than be limited by the current implementation.

## The external data
There are a large number of external data sources that are currently being linked to. It is not within the scope of this project to be exhaustive, but the proposal should cover all types of sources. In particular, it should accurately represent the following three types of sources:
•	Sequence alignment data, eg https://www.ncbi.nlm.nih.gov/refseq/
•	Gene naming consortia, eg https://www.genenames.org/
•	Extra annotation data, eg https://www.omim.org/
