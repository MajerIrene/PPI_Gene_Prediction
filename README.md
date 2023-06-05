# PPI_Gene_Prediction
>Human diseases generally are consequences of perturbations in the molecular network induced by various factors such as genetic mutations, epigenetic changes and pathogens → Gene associated with the same or similar diseases commonly reside in the same neighborhood of these networks and form physical and/or functional modules. 
Since proteins (products of genes) usually work together to achieve a specific function, biomolecular networks, such as the protein-protein interaction (PPI) network and gene co-expression networks, are widely used to predict disease genes by analyzing the relationships between known disease genes and other genes in the networks. 

From Wang et al. (2011) Network-based methods for human disease gene prediction. Briefings in Functional Genomics 10(5):280–293.

## General Information

This is a Python package for disease gene prediction based on an protein-protein interaction network. 
The package takes: 
1. A protein-protein interaction network from an individual species (e.g., human) from the STRING database (see below), using only physical interactions (direct)
2. A set of known disease-related “seed” (or reference) genes
3. Optionally a set of “candidate” disease genes (if not specified, all non-seed genes will be taken as candidates)

The aim is to rank all “candidate” genes according to their vicinity to the seed genes on the network using the random walk with restart approach.
