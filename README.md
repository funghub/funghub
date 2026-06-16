# Hi, I'm Lawrence Fung

I work in bioinformatics and computational biology, with a focus on data analysis, statistical modeling, machine learning, and reproducible workflows applied to multi-omics and clinical datasets. My projects emphasize transforming high-dimensional biological data into interpretable insights using R and Python.

# Featured Projects

## Traditional Bioinformatics Related Projects

- **[RNA-Seq/TempO-Seq Data Processing Pipeline](https://github.com/funghub/PFAS_project)**  
  For a PFAS exposure transcriptomics study, I built an automated Nextflow pipeline that leverages bioinformatics tools (SRA-tools, FastP/FastQC, STAR, Picard, and featureCounts) to take raw public RNA-seq data from an SRA accession through to analysis-ready gene expression counts, complete with quality control reports at each stage. My goal was to lower the barrier to reproducible RNA-seq analysis by: automating retrieval and processing of public sequencing data end-to-end, packaging every tool's dependencies in conda environments so the pipeline runs identically on any machine, and giving researchers clean, comparable count matrices ready for downstream differential expression analysis.

- **[Converting HGVS Notation to Protein Sequences](https://github.com/funghub/cysticfibrosis-project)**  
  Through CFTR-Fr datasets, we seek to visualize the list of mutations on AlphaFold by inputting the DNA sequences and protein sequences created from the HGVS nomenclature and reference gene on NCBI with Python. We investigate how mutations in those regions of the gene affect the final shape and function of the CFTR protein, specifically the crucial parts of the protein, such as Phe508del in 90% of cystic fibrosis patients.

## Machine Learning + Biology Related Projects

- **[Fine Tuning Protein Folding Model: ESMFold](https://github.com/funghub/finetune_ESMFold)**  
Supervised finetuneing of Meta's protein prediction model ESMFold (hosted on Hugging Face at facebook/esmfold_v1) on Toxin-Antitoxin Protein Sequences. Improve pLDDT confidence scores on low-confidence proteins. The results were modest as fine-tuning helped about half the proteins improve their pLDDT score. Built with Hugging Face Transformers (EsmForProteinFolding, AutoTokenizer, Trainer, TrainingArguments), PyTorch (layer freezing & custom loss), and Biopython for data parsing.

- **[Machine Learning: Logistic Regression Model Training for Melanoma SNV](https://github.com/funghub/predict_snv_effect)**  
  This project utilizes a logistic regression, a supervised machine learning model, to predict the pathogenicity of specific non-coding variants in melanoma given epigenetic features. Pandas was used to organize, clean, and merge the data. Scikit-learn was used to train and evaluate the model, along with one-hot encoding for nucleotides because logistic regression only takes numerical features. Pyplot from matplotlib and seaborn was used to generate a heatmap of the confusion matrix and plot the ROC-AUC curve.

- **[NGS Normalization](https://github.com/funghub/gene_expression_data-normalization)**  
  This R notebook normalizes the raw counts with TMM (trimmed mean of M-values) and CPM (counts per million) from Pasilla gene expression. A heatmap via a distance matrix is generated with pheatmap library. With edgeR, plots of normalized values cpm & tmm are created. With dplyr, tidyr, and ggplot2 libraries a density plot of expression values for all samples is created.
  
- **[NGS Clustering](https://github.com/funghub/gene_expression_data-clustering)**  
  This R notebook will use statistical techniques to understand a NGS data set and compare gene expression by hierarchical clustering and k-means clustering (unsupervised learning). Explanations of the diagrams are included in the notebook. 

- **[NGS Classification](https://github.com/funghub/gene_expression_data-classification)**  
  This R notebook takes a NGS data set and applies a binary classification method to sort out replicate1 and other replicates. Then this is plot on a ROC curve to explore different thresholds. The notebook also explores the use of confusion matrix to calculate specificity (tnr), sensitivity (tpr), and false positive rate. Explanations of the diagrams are included in the notebook.

- **[Hidden Markov Model Protein Family](https://github.com/funghub/proteinfamHMM)**  
  This R notebook creates a HMM model that represents a given diagram showing all the path of the hidden states. I will find the most likely sequence of hidden states for each protein family. In addition, given a sequence of observations, I will also find the likely family that would have generated those observations and then find the most likely sequence of hidden states of that family with the Viterbi algorithm.

## Applied Machine Learning/AI Real World Application

- **[Drug Discovery Web Application](https://github.com/funghub/YC_HACK2026)**  
  At the Y Combinator Hackathon, my team leveraged bioinformatics machine learning tools (DrugFlow, PLACER, and ADMET-AI) to build a centralized platform that helps researchers evaluate generated ligand compounds and identify the most promising candidates for further research and development. Our goal was to lower the barrier to computational drug discovery by: centralizing multiple bioinformatics tools, explaining tools and results in a way that new researchers can understand, and helping scientists identify promising compounds faster during the exploratory phase of research.

- **[MCP-Grounded AI Agent for Teaching ML in Bioinformatics](https://github.com/funghub/ML_Bioinfo_Teach)**  
  At the Bioinformatics Hackathon, my team built Geneius, an AI agent that explains machine learning concepts in bioinformatics by connecting a Gemini LLM to a PubMed MCP server, letting the agent query NCBI's E-utilities directly for real peer-reviewed articles instead of relying on the model's own potentially outdated or hallucinated recall. We also used LangChain to trace and evaluate the agent's tool calls and outputs, monitoring performance to make sure the MCP integration was actually improving reliability. Our goal was to lower the barrier to learning computational biology by: using MCP to ground every explanation in live, verifiable PubMed sources rather than unchecked model knowledge, making dense ML concepts accessible through plain-language breakdowns and generated diagrams, and giving researchers clickable links to the exact papers the agent cited so they can verify claims themselves.

## Connect With Me

- LinkedIn: (https://www.linkedin.com/in/funglawrence/)
