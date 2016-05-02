<<<<<<< HEAD
Gene set tests are often used in differential expression analyses to explore the behaviour of a group of related genes. This is useful for identifying large-scale co-regulation of genes belonging to the same biological process or molecular pathway. 

One of the most flexible and powerful gene set tests is the ROAST method in the limma R package. ROAST uses residual space rotation as a sort of continuous version of sample permutation. Like permutation tests, it protects against false positives caused by correlations between genes in the set. Unlike permutation tests, it can be used with complex experimental design and with small numbers of replicates. It is the only gene set test method that is able to analyse complex "gene expression signatures" that incorporate information about both up and down regulated genes simultaneously.

ROAST works well for individual expression signatures, but has limitations when applied to large collections of gene sets, such as the Broad Institute's Molecular Signature Database with over 8000 gene sets. In particular, the p-value resolution is limited by the number of rotations that are done for each set. This makes it impossible to obtain very small p-values and hence to distinguish the top ranking pathways from a large collection. As with permutation tests, the p-values for each set may vary from run to run.

This talk presents Fry, a very fast approximation to the complete ROAST method. Fry approximates the limiting p-value that would be obtained from performing a very large number of rotations with ROAST. Fry preserves most of the advantages of ROAST, but also provides high resolution exact p-values very quickly. In particular, it is able to distinguish the most significant sets in large collections and to yield statistically significant results after adjustment for multiple testing. This makes it an ideal tool for large-scale pathway analysis.
`fry()` and `roast()` `limma::lmEffects()`
=======
# fry-web-app
>>>>>>> 2e49a80fa9a6881bd207f9115f447fb1c077d95a
