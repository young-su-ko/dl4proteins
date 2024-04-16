# Papers related to protein language models

## 1. [Genomic language model predicts protein co-regulation and function](https://www.nature.com/articles/s41467-024-46947-9)
<details>
<summary>Summary</summary>

### Abstract
Deciphering the relationship between a gene and its genomic context is fundamental to understanding and engineering biological systems. Machine learning has shown promise in learning latent relationships underlying the sequence-structure-function paradigm from massive protein sequence datasets. However, to date, limited attempts have been made in extending this continuum to include higher order genomic context information. Evolutionary processes dictate the specificity of genomic contexts in which a gene is found across phylogenetic distances, and these emergent genomic patterns can be leveraged to uncover functional relationships between gene products. Here, we train a genomic language model (gLM) on millions of metagenomic scaffolds to learn the latent functional and regulatory relationships between genes. gLM learns contextualized protein embeddings that capture the genomic context as well as the protein sequence itself, and encode biologically meaningful and functionally relevant information (e.g. enzymatic function, taxonomy). Our analysis of the attention patterns demonstrates that gLM is learning co-regulated functional modules (i.e. operons). Our findings illustrate that gLM’s unsupervised deep learning of the metagenomic corpus is an effective and promising approach to encode functional semantics and regulatory syntax of genes in their genomic contexts and uncover complex relationships between genes in a genomic region.

[Github link](https://github.com/y-hwang/gLM)
</details>

## 2. [OntoProtein: Protein Pretraining With Gene Ontology Embedding](https://arxiv.org/abs/2201.11147)
<details>
<summary>Summary</summary>

### Abstract
Self-supervised protein language models have proved their effectiveness in learning the proteins representations. With the increasing computational power, current protein language models pre-trained with millions of diverse sequences can advance the parameter scale from million-level to billion-level and achieve remarkable improvement. However, those prevailing approaches rarely consider incorporating knowledge graphs (KGs), which can provide rich structured knowledge facts for better protein representations. We argue that informative biology knowledge in KGs can enhance protein representation with external knowledge. In this work, we propose OntoProtein, the first general framework that makes use of structure in GO (Gene Ontology) into protein pre-training models. We construct a novel large-scale knowledge graph that consists of GO and its related proteins, and gene annotation texts or protein sequences describe all nodes in the graph. We propose novel contrastive learning with knowledge-aware negative sampling to jointly optimize the knowledge graph and protein embedding during pre-training. Experimental results show that OntoProtein can surpass state-of-the-art methods with pre-trained protein language models in TAPE benchmark and yield better performance compared with baselines in protein-protein interaction and protein function prediction. Code and datasets are available in this https URL.

[Github link](https://github.com/zjunlp/OntoProtein)
</details>

## 3. [ProteinBERT: a universal deep-learning model of protein sequence and function](https://academic.oup.com/bioinformatics/article/38/8/2102/6502274)
<details>
<summary>Summary</summary>

### Abstract
Self-supervised deep language modeling has shown unprecedented success across natural language tasks, and has recently been repurposed to biological sequences. However, existing models and pretraining methods are designed and optimized for text analysis. We introduce ProteinBERT, a deep language model specifically designed for proteins. Our pretraining scheme combines language modeling with a novel task of Gene Ontology (GO) annotation prediction. We introduce novel architectural elements that make the model highly efficient and flexible to long sequences. The architecture of ProteinBERT consists of both local and global representations, allowing end-to-end processing of these types of inputs and outputs. ProteinBERT obtains near state-of-the-art performance, and sometimes exceeds it, on multiple benchmarks covering diverse protein properties (including protein structure, post-translational modifications and biophysical attributes), despite using a far smaller and faster model than competing deep-learning methods. Overall, ProteinBERT provides an efficient framework for rapidly training protein predictors, even with limited labeled data

[Github link](https://github.com/nadavbra/protein_bert)
</details>

## 3. [ProteinBERT: a universal deep-learning model of protein sequence and function](https://academic.oup.com/bioinformatics/article/38/8/2102/6502274)
<details>
<summary>Summary</summary>

### Abstract
Self-supervised deep language modeling has shown unprecedented success across natural language tasks, and has recently been repurposed to biological sequences. However, existing models and pretraining methods are designed and optimized for text analysis. We introduce ProteinBERT, a deep language model specifically designed for proteins. Our pretraining scheme combines language modeling with a novel task of Gene Ontology (GO) annotation prediction. We introduce novel architectural elements that make the model highly efficient and flexible to long sequences. The architecture of ProteinBERT consists of both local and global representations, allowing end-to-end processing of these types of inputs and outputs. ProteinBERT obtains near state-of-the-art performance, and sometimes exceeds it, on multiple benchmarks covering diverse protein properties (including protein structure, post-translational modifications and biophysical attributes), despite using a far smaller and faster model than competing deep-learning methods. Overall, ProteinBERT provides an efficient framework for rapidly training protein predictors, even with limited labeled data

[Github link](https://github.com/nadavbra/protein_bert)
</details>

## 4. [Sequence modeling and design from molecular to genome scale with Evo](https://www.biorxiv.org/content/10.1101/2024.02.27.582234v2)
<details>
<summary>Summary</summary>

### Abstract
The genome is a sequence that completely encodes the DNA, RNA, and proteins that orchestrate the function of a whole organism. Advances in machine learning combined with massive datasets of whole genomes could enable a biological foundation model that accelerates the mechanistic understanding and generative design of complex molecular interactions. We report Evo, a genomic foundation model that enables prediction and generation tasks from the molecular to genome scale. Using an architecture based on advances in deep signal processing, we scale Evo to 7 billion parameters with a context length of 131 kilobases (kb) at single-nucleotide, byte resolution. Trained on 2.7M prokaryotic and phage genomes, Evo can generalize across the three fundamental modalities of the central dogma of molecular biology to perform zero-shot function prediction that is competitive with, or outperforms, leading domain-specific language models. Evo also excels at multi-element generation tasks, which we demonstrate by generating synthetic CRISPR-Cas molecular complexes and entire transposable systems for the first time. Using information learned over whole genomes, Evo can also predict gene essentiality at nucleotide resolution and can generate coding-rich sequences up to 650 kb in length, orders of magnitude longer than previous methods. Advances in multi-modal and multiscale learning with Evo provides a promising path toward improving our understanding and control of biology across multiple levels of complexity.

[Github link](https://github.com/evo-design/evo)
</details>

## 5. [S-PLM: Structure-aware Protein Language Model via Contrastive Learning between Sequence and Structure](https://www.biorxiv.org/content/10.1101/2023.08.06.552203v2)
<details>
<summary>Summary</summary>

### Abstract
Large protein language models (PLMs) present excellent potential to reshape protein research by encoding the amino acid sequences into mathematical and biological meaningful embeddings. However, the lack of crucial 3D structure information in most PLMs restricts the prediction capacity of PLMs in various applications, especially those heavily depending on 3D structures. To address this issue, we introduce S-PLM, a 3D structure-aware PLM utilizing multi-view contrastive learning to align the sequence and 3D structure of a protein in a coordinate space. S-PLM applies Swin-Transformer on AlphaFold-predicted protein structures to embed the structural information and fuses it into sequence-based embedding from ESM2. Additionally, we provide a library of lightweight tuning tools to adapt S-PLM for diverse protein property prediction tasks. Our results demonstrate S-PLM’s superior performance over sequence-only PLMs, achieving competitiveness in protein function prediction compared to state-of-the-art methods employing both sequence and structure inputs.

[Github link](https://github.com/duolinwang/S-PLM/)
</details>

## 6. [Pre-training co-evolutionary protein representation via a pairwise masked language model](https://arxiv.org/pdf/2110.15527.pdf)
<details>
<summary>Summary</summary>

### Abstract
Understanding protein sequences is vital and urgent for biology, healthcare, and medicine. Labeling approaches are expensive yet time-consuming, while the amount of unlabeled data is increasing quite faster than that of the labeled data due to low-cost, high-throughput sequencing methods. In order to extract knowledge from these unlabeled data, representation learning is of significant value for protein-related tasks and has great potential for helping us learn more about protein functions and structures. The key problem in the protein sequence representation learning is to capture the co-evolutionary information reflected by the inter-residue co-variation in the sequences. Instead of leveraging multiple sequence alignment as is usually done, we propose a novel method to capture this information directly by pre-training via a dedicated language model, i.e., Pairwise Masked Language Model (PMLM). In a conventional masked language model, the masked tokens are modeled by conditioning on the unmasked tokens only, but processed independently to each other. However, our proposed PMLM takes the dependency among masked tokens into consideration, i.e., the probability of a token pair is not equal to the product of the probability of the two tokens. By applying this model, the pre-trained encoder is able to generate a better representation for protein sequences. Our result shows that the proposed method can effectively capture the inter-residue correlations and improves the performance of contact prediction by up to 9% compared to the MLM baseline under the same setting. The proposed model also significantly outperforms the MSA baseline by more than 7% on the TAPE contact prediction benchmark when pre-trained on a subset of the sequence database which the MSA is generated from, revealing the potential of the sequence pre-training method to surpass MSA based methods in general. 

</details>

## 7. [Domain-PFP allows protein function prediction using function-aware domain embedding representations](https://www.nature.com/articles/s42003-023-05476-9)
<details>
<summary>Summary</summary>

### Abstract
Domains are functional and structural units of proteins that govern various biological functions performed by the proteins. Therefore, the characterization of domains in a protein can serve as a proper functional representation of proteins. Here, we employ a self-supervised protocol to derive functionally consistent representations for domains by learning domain-Gene Ontology (GO) co-occurrences and associations. The domain embeddings we constructed turned out to be effective in performing actual function prediction tasks. Extensive evaluations showed that protein representations using the domain embeddings are superior to those of large-scale protein language models in GO prediction tasks. Moreover, the new function prediction method built on the domain embeddings, named Domain-PFP, substantially outperformed the state-of-the-art function predictors. Additionally, Domain-PFP demonstrated competitive performance in the CAFA3 evaluation, achieving overall the best performance among the top teams that participated in the assessment.

[Github link](https://github.com/kiharalab/Domain-PFP?tab=readme-ov-file)
</details>

## 8. [Aggregating Residue-Level Protein Language Model Embeddings with Optimal Transport](https://www.biorxiv.org/content/10.1101/2024.01.29.577794v1.abstract)
<details>
<summary>Summary</summary>

### Abstract
Protein language models (PLMs) have emerged as powerful approaches for mapping protein sequences into informative embeddings suitable for a range of applications. PLMs, as well as many other protein representation schemes, generate per-token (i.e., per-residue) representations, leading to variable-sized outputs based on protein length. This variability presents a challenge for protein-level prediction tasks, which require uniform-sized embeddings for consistent analysis across different proteins. Prior work has typically resorted to average pooling to summarize token-level PLM outputs. It is, however, unclear if such an aggregation operation effectively prioritizes the relevant information across token-level representations.

Addressing this, we introduce a novel method utilizing sliced-Wasserstein embeddings to convert variable-length PLM outputs into fixed-length protein-level representations. Inspired by the success of optimal transport techniques in representation learning, we first conceptualize per-token PLM outputs as samples from a probabilistic distribution. We then employ sliced-Wasserstein distances to map these samples against a learnable reference set, creating a Euclidean embedding in the output space. The resulting embedding is agnostic to the length of the input and represents the entire protein. Across a range of state-of-the-art pre-trained ESM-2 PLMs, with varying model sizes, we show the superiority of our method over average pooling for protein-drug and protein-protein interaction. Our aggregation scheme is especially effective when model size is constrained, enabling smaller-scale PLMs to match or exceed the performance of average-pooled larger-scale PLMs. Since using smaller models reduces computational resource requirements, our approach not only promises more accurate inference but can also help democratize access to foundation models.

[Github link](https://github.com/navid-naderi/PLM_SWE)
</details>

