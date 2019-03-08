# Pan-genome gene content analysis

## Brief Explanation

For many species, including plants, researchers are now producing not one but several genome assemblies, which are then combined to define what is called a pan-genome. Building on the Compara framework, the student will test different whole-genome alignment strategies and nucleotide gene phylogenies to produce a presence-absence (PAV) matrix.

Input data for this project includes:
- Two or more genome assemblies in FASTA format
- GFF files with genes/features annotated on those genomes

## Expected results

- A workflow to extract a gene PAV matrix from a set of genomes from the same/closely related species and produce a flat file over the REST API
- A script to produce a simple, high-resolution plot of the PAV matrix

## Required knowledge

1. Python/Java/Perl/R
2. Unix HPC environments. We use [eHive](https://github.com/Ensembl/ensembl-hive) but students can choose others if required.
3. Data analysis, bioinformatics. Currently we consider using:
	* [lastZ](https://github.com/lastz/lastZ) and [minimap2](https://github.com/lh3/minimap2)
	* [cactus](https://github.com/ComparativeGenomicsToolkit/cactus)

## Difficulty

Medium

## Mentors

[Matthieu Muffato](https://www.ebi.ac.uk/about/people/matthieu-muffato), [Steve Trevanion](https://www.ebi.ac.uk/about/people/stephen-trevanion), [Bruno Contreras-Moreira](https://www.ebi.ac.uk/about/people/bruno-contreras-moreira)
