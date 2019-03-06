# Repeat annotation

## Brief Explanation

Vertebrate genomes contain repetitive stretches of DNA. This might mean the same element repeated in tandem in a particular region or an element is repeated at numerous locations over the genome (or both). Repeat elements often greatly expand the sequence of a genome without adding to the functional repertoire.

The annotation of repeat families is interesting from an evolutionary standpoint, but also important from a computational standpoint. Repeats have a tendency to slow, confuse or completely break software. In addition they naturally make the search space for functional elements much bigger than it should be, as it is very unusual to find function elements such as genes within repeats.

As part of the genome annotation pipeline Ensembl runs popular repeat finding tools including RepeatMasker, Dust and TRF to find potential repeats. This strategy works well for species where the repeats have a well characterised repeat library to help with finding repeats in the genome sequence.

For species with unique repeats, or where there is no suitable repeat library, this strategy does not work well. In such cases we use RepeatModeler for ab initio repeat finding, in order to generate a repeat library. One major issue with this strategy is that RepeatModeler sometimes identifies gene families as repeats. Some gene families, for example single exon genes, are particularly susceptible to this problem. The purpose of this project would be to examine and implement new methods of repeat finding and filtering to improve the quality of repeat annotation in Ensembl

## Expected results
 - Generate a set of high quality repeat libraries for all vertebrates with an available genome sequence
 - Produce repeat-masked copies of these genomes submitted post analysis back to the public archives
 - Update the Ensembl annotation code-base and pipelines to take advantage of improvements to the repeat annotation process
 - Potential to create a standalone, containerised, continuously deployed pipeline for repeat annotation. This could run on genome sequences as soon as they arrive in the public archives and submit a completed repeat analysis back to the archives

## Required knowledge
 - Object-oriented coding
 - Familiarity with some of the following: genomics, repeat annotation, bioinformatics software, GIT, containers, deployment strategies, CWL

## Difficulty
 - Medium-hard

## Mentors
Osagie Izuogu, Fergal Martin
