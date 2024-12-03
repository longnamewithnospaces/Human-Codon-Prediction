# Human-Codon-Prediction
Predicting the evolutionarily selected codons of human protein-coding genes, using a BART-based language model. The model receives the amino acids, and tissue-expression values refined to percentile categories.

## Project Structure
1. Source: Comprised of both Jupyter notebooks integrated with graphs and results, as well as some python files accompanied with SLURM SBATCH scripts - for the more computationally intensive tasks.
   - Data preprocessing:

     a. Retreiving the expression data from GTEx

     b. Cleaning the data

     c. Refining expression to categories + Graphs

     d. Clustering proteins with CD-HIT + Grouping same-gene protein sequences

     e. Finding nearest trainset neighbours (to testset CD-HIT representatives) with BLASTP
   - Models:

     a. Baseline models (frequency based)

     b. Generating the tokenizer

     c. Generating the arrow datasets

     d. Training and evaluating the BART models
   - Analysing the results:

     a. Various accuracy graphs

     b. Gene Set Enrichment Analysis for accuracy difference metric
2. Data: The data used for each stage of the source.
3. Graphs: The interesting graphs detailing the results of the project.
