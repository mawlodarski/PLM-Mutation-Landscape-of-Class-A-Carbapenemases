plm_mutation_workflow.drawio (2).png

# PLM-Mutation-Landscape-of-Class-A-Carbapenemases
Using protein language model embeddings and systematic in silico mutagenesis, this project maps the mutation landscape of class A carbapenemases to identify residues under functional constraint that distinguish carbapenemase enzymes from closely related β-lactamases.


# 1 Sequence retrieval

CARD v4.0.1
Filtered card.json to only class A carbapenemases (KPC, SME, IMI) and non-carbapenemases (TEM, CTX-M, SHV, VEB)

# 2 Data filtering
998 sequences total:

Carbapenemase (KPC, SME, IMI)
0    737
1    261

Family
CTX-M    266
KPC      230
SHV      216
TEM      216
VEB       39
IMI       26
SME        5

# 3 Embedding generation
esm2_t33_650M_UR50D (1280D)
PyTorch version: 2.10.0

need to try smaller model + shallow FCN classifier
