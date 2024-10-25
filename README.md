# Generative-Protein-Modeling 

A systematic survey of **generative approaches in protein engineering**, organized through two fundamental taxonomies: **(1) task-oriented classification** - including ***sequence-based generation***, ***structure-based generation***, and ***joint sequence-structure generation***; **(2) inference framework classification** - with particular focus on ***autoregressive models*** and ***diffusion models*** that have demonstrated remarkable progress in this domain. This survey provides a comprehensive analysis of state-of-the-art generative methods, offering detailed examination of their theoretical foundations, architectural innovations, and practical applications in protein design and engineering, supported by extensive research papers, implementations, and benchmarks.

**OPEN TO COLLABORATION! If you have any new insights in any relevant research direction or just want to chat, please drop us an email (xinhuichen.be@gmail.com).**

**<font color="red">[*New*, Paper]</font>** Our research paper: [Generative Models in Protein Engineering: A
Comprehensive Survey](https://arxiv.org/submit/5950681/view) has accepted by **FM2Science workshop, NeurIPS 2024 (Oral)**, which synthesizes recent advances in generative modeling approaches for protein engineering and provides a systematic categorization of existing methods.

>**Abstract**:
>Proteins are fundamental molecules performing diverse functions in living organisms. Protein engineering, the process of designing or modifying proteins to enhance or create new functions, has therefore become a research focus in the fields of biotechnology and medicine. A primary challenge in protein engineering is to efficiently discover and design new proteins with desired functions. Traditional approaches like directed evolution and rational design, though widely used, are limited by high computational costs and restricted exploration of potential protein structures. The recent success of generative models in efficiently synthesizing high-quality data across various domains has inspired researchers to investigate their potential applications in protein engineering. In this survey, we systematically summarize recent works on generative models for protein engineering, with a particular focus on protein design. Specifically, we categorize three main frameworks in existing generative protein design methods: sequence-based, structure-based, and joint sequence-structure generation. Besides, we provide a detailed review of representative generative models, including autoregressive models and diffusion models, and their application in protein sequence prediction and structure generation. Finally, we pinpoint existing challenges and propose future directions, such as leveraging large datasets, improving complex structure validation, and integrating advanced modeling techniques.

**We will continue to update this list with the newest resources. If you find any missed resources (paper/code) or errors, please feel free to open an issue or make a pull request.**

___
## Task-oriented Classification
>**Sequence-based Protein Design**: Focuses on generating novel protein sequences by learning from the vast space of amino-acid sequences, incorporating both unconstrained and constrained design scenarios (functional/structural requirements).
>
>**Structure-based Protein Design**: Focuses on leveraging structural information for protein sequence prediction and design through various sophisticated approaches.
>
>**Joint Sequence-structure Generation**: Focuses on leveraging structural information for protein sequence prediction and design. 

**Sequence-based Protein Design Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Protgpt2 is a deep unsupervised language model for protein design | **Nature Communications** | 2022 | [\[paper\]](https://www.nature.com/articles/s41467-022-32007-7) [\[code\]](https://github.com/TeletcheaLab/protGPT2) |
| Large language models generate functional protein sequences across diverse families | **Nature Biotechnology** | 2022 | [\[paper\]](https://www.nature.com/articles/s41587-022-01618-2) |
| Proteinnpt: Improving protein property prediction and design with non-parametric transformers | **NeurIPS** | 2023 | [\[paper\]](https://dl.acm.org/doi/10.5555/3666122.3667580) [\[code\]](https://github.com/OATML-Markslab/ProteinNPT) |
| Rita: a study on scaling up generative protein sequence models | **arXiv** | 2022 | [\[paper\]](https://arxiv.org/abs/2205.05789) [\[code\]](https://github.com/lightonai/RITA) |
| Protein Design by Sampling an Undirected Graphical Model of Residue Constraints | **IEEE-ACM Trans. Comput. Biol. Bioinform.** | 2008 | [\[paper\]](https://ieeexplore.ieee.org/document/4685894) |
| Expanding functional protein sequence spaces using generative adversarial networks | **Nature Machine Intelligence** | 2021 | [\[paper\]](https://www.nature.com/articles/s42256-021-00310-5) [\[code\]](https://github.com/Biomatter-Designs/ProteinGAN) |

**Structure-based Protein Design Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Learning from Protein Structure with Geometric Vector Perceptrons | **ICLR** | 2020 | [\[paper\]](https://arxiv.org/abs/2009.01411) [\[code\]](https://github.com/drorlab/gvp) |
| Gpsfun: geometry-aware protein sequence function predictions with language models | **Nucleic Acids Res** | 2024 | [\[paper\]](https://pubmed.ncbi.nlm.nih.gov/38738636/) [\[code\]](https://github.com/kostin-aleks/gpsfun/blob/main/README.md)|
| Diffsds: A language diffusion model for protein backbone inpainting under geometric conditions and constraints | **arXiv** | 2023 | [\[paper\]](https://arxiv.org/abs/2301.09642)  [\[code\]](https://github.com/A4Bio/DiffSDS) |
| Framedipt: Se (3) diffusion model for protein structure inpainting | **BioRxiv** | 2023 | [\[paper\]](https://www.biorxiv.org/content/10.1101/2023.11.21.568057v1.full.pdf)  [\[code\]](https://github.com/instadeepai/FrameDiPT) |
| Diffusion probabilistic modeling of protein backbones in 3d for the motif-scaffolding problem | **arXiv** | 2022 | [\[paper\]](https://arxiv.org/abs/2206.04119)  [\[code\]](https://github.com/blt2114/ProtDiff_SMCDiff) |
| ProteinSGM: Score-based generative modeling for de novo protein design | **BioRxiv** | 2022 | [\[paper\]](https://www.biorxiv.org/content/10.1101/2022.07.13.499967v1.full.pdf) |
| Robust deep learning–based protein sequence design using ProteinMPNN | **Science** | 2022 | [\[paper\]](https://www.science.org/doi/10.1126/science.add2187) [\[code\]](https://github.com/dauparas/ProteinMPNN) |
| High-resolution de novo structure prediction from primary sequence | **BioRxiv** | 2022 | [\[paper\]](https://www.biorxiv.org/content/biorxiv/early/2022/07/22/2022.07.21.500999.full.pdf) [\[code\]](https://github.com/HeliXonProtein/OmegaFold) |


**Sequence and Structure Co-generation Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Protein sequence and structure co-design with equivariant translation | **arXiv** | 2022 | [\[paper\]](https://arxiv.org/abs/2210.08761) [\[code\]](https://github.com/shichence/ProtSeed/releases) |
| Functional geometry guided protein sequence and backbone structure co-design | **arXiv** | 2023 | [\[paper\]](https://arxiv.org/abs/2310.04343v3) [\[code\]](https://github.com/jocelynsong/naepro) |
| Broadly applicable and accurate protein design by integrating structure prediction networks and diffusion generative models | **BioRxiv** | 2022 | [\[paper\]](https://www.biorxiv.org/content/10.1101/2022.12.09.519842v1) [\[code\]](https://github.com/RosettaCommons/RFdiffusion) |
| Iterative refinement graph neural network for antibody sequence-structure co-design | **arXiv** | 2021 | [\[paper\]](https://arxiv.org/abs/2110.04624v1) [\[code\]](https://github.com/wengong-jin/RefineGNN) |
| Generative models for graph-based protein design | **NeurIPS** | 2019 | [\[paper\]](https://papers.nips.cc/paper_files/paper/2019/file/f3a4ff4839c56a5f460c88cce3666a2b-Paper.pdf) [\[code\]](https://github.com/jingraham/neurips19-graph-protein-design) |
 
___
## Autoregressive Models
>**Remark**: Autoregressive models have emerged as powerful tools in protein sequence generation, evolving from early ***RNNs*** and ***LSTMs*** that capture long-range dependencies, to advanced ***Transformer*** architectures leveraging self-attention mechanisms and large-scale pre-training, and further to ***Graph Neural Networks*** that naturally represent protein structures.

**RNN-based Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Deep Recurrent Neural Network for Protein Function Prediction from Sequence | **arXiv** | 2017 | [\[paper\]](https://arxiv.org/abs/1701.08318) |
| Prediction of 8-state protein secondary structures by a novel deep learning architecture | **BMC bioinformatics** | 2018 | [\[paper\]](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-018-2280-5) |

**LSTM-based Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| DeepANIS: Predicting antibody paratope from concatenated CDR sequences by integrating bidirectional long-short-term memory and transformer neural networks | **IEEE** | 2021 | [\[paper\]](https://ieeexplore.ieee.org/abstract/document/9669631) [\[code\]](https://github.com/HideInDust/DeepANIS) |

**Transformer-based Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Protgpt2 is a deep unsupervised language model for protein design | **Nature Communications** | 2022 | [\[paper\]](https://www.nature.com/articles/s41467-022-32007-7) [\[code\]](https://github.com/TeletcheaLab/protGPT2) |
| ZymCTRL: a conditional language model for the controllable generation of artificial enzymes | **NeurIPS MLSB Workshop** | 2022 | [\[paper\]](https://nips.cc/virtual/2022/59047) [\[code\]](https://huggingface.co/AI4PD/ZymCTRL) |
| ProteinSGM: Score-based generative modeling for de novo protein design | **BioRxiv** | 2022 | [\[paper\]](https://www.biorxiv.org/content/10.1101/2022.07.13.499967v1.full.pdf) |
| High-resolution de novo structure prediction from primary sequence | **BioRxiv** | 2022 | [\[paper\]](https://www.biorxiv.org/content/biorxiv/early/2022/07/22/2022.07.21.500999.full.pdf) [\[code\]](https://github.com/HeliXonProtein/OmegaFold) |
| Protein sequence and structure co-design with equivariant translation | **arXiv** | 2022 | [\[paper\]](https://arxiv.org/abs/2210.08761) [\[code\]](https://github.com/shichence/ProtSeed/releases) |
| Progen2: exploring the boundaries of protein language models | **Cell Systems** | 2023 | [\[paper\]](https://www.cell.com/cell-systems/abstract/S2405-4712(23)00272-7?s=35) [\[code\]](https://github.com/enijkamp/progen2) |

**GNN-based Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Learning from Protein Structure with Geometric Vector Perceptrons | **ICLR** | 2020 | [\[paper\]](https://arxiv.org/abs/2009.01411) [\[code\]](https://github.com/drorlab/gvp) |
| EquiBind: Geometric Deep Learning for Drug Binding Structure Prediction | **ICML** | 2022 | [\[paper\]](https://arxiv.org/abs/2202.05146) [\[code\]](https://github.com/HannesStark/EquiBind) |
| Robust deep learning–based protein sequence design using ProteinMPNN | **Science** | 2022 | [\[paper\]](https://www.science.org/doi/10.1126/science.add2187) [\[code\]](https://github.com/dauparas/ProteinMPNN) |
| Iterative refinement graph neural network for antibody sequence-structure co-design | **arXiv** | 2021 | [\[paper\]](https://arxiv.org/abs/2110.04624v1) [\[code\]](https://github.com/wengong-jin/RefineGNN) |
| AbODE: Ab Initio Antibody Design using Conjoined ODEs | **ICML** | 2023 | [\[paper\]](https://arxiv.org/abs/2306.01005) [\[code\]](https://github.com/Aalto-QuML/AbODE) |


___
## Diffusion Models
>**Remark**: Diffusion models in protein structure generation have evolved along two significant dimensions. From a geometric perspective, the field has progressed from ***Euclidean*** approaches that treat proteins as simple point sets to more sophisticated ***geometric*** methods that leverage manifold-based representations and graph structures, enabling better capture of intrinsic protein properties. From a transformation perspective, the field has explored both ***equivariant*** methods that maintain rotational and translational symmetry through sophisticated mathematical frameworks, and ***non-equivariant*** approaches that address protein chirality through internal coordinate representations.

**Euclidean Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Protein Structure and Sequence Generation with Equivariant Denoising Diffusion Probabilistic Models | **arXiv** | 2022 | [\[paper\]](https://arxiv.org/abs/2205.15019) |
| Diffusion probabilistic modeling of protein backbones in 3d for the motif-scaffolding problem | **ICLR** | 2023 | [\[paper\]](https://arxiv.org/abs/2206.04119) [\[code\]](https://github.com/blt2114/ProtDiff_SMCDiff) |
| Nvdiff: Graph generation through the diffusion of node vectors | **arXiv** | 2023 | [\[paper\]](https://arxiv.org/abs/2211.10794) |

**Geometric Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Riemannian score-based generative modelling | **NeurIPS** | 2022 | [\[paper\]](https://proceedings.neurips.cc/paper_files/paper/2022/file/105112d52254f86d5854f3da734a52b4-Paper-Conference.pdf) [\[code\]](https://github.com/GeometricBCI/riemannian-score-sde/blob/main/README.md) |
| Graphgdp: Generative diffusion processes for permutation invariant graph generation | **IEEE** | 2022 | [\[paper\]](https://arxiv.org/abs/2212.01842) [\[code\]](https://github.com/GRAPH-0/GraphGDP) |
| Broadly applicable and accurate protein design by integrating structure prediction networks and diffusion generative models | **BioRxiv** | 2022 | [\[paper\]](https://www.biorxiv.org/content/10.1101/2022.12.09.519842v1) [\[code\]](https://github.com/RosettaCommons/RFdiffusion) |
| SE(3) diffusion model with application to protein backbone generation | **arXiv** | 2023 | [\[paper\]](https://arxiv.org/abs/2302.02277) [\[code\]](https://github.com/jasonkyuyim/se3_diffusion) |
| Equivariant 3D-conditional diffusion model for molecular linker design | **Nature Machine Intelligence** | 2024 | [\[paper\]](https://arxiv.org/abs/2210.05274) [\[code\]](https://github.com/igashov/DiffLinker) |
| Protein structure generation via folding diffusion | **Nature Communications** | 2024 | [\[paper\]](https://www.nature.com/articles/s41467-024-45051-2) [\[code\]](https://github.com/microsoft/foldingdiff) |

**Equivariant Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Riemannian score-based generative modelling | **NeurIPS** | 2022 | [\[paper\]](https://proceedings.neurips.cc/paper_files/paper/2022/file/105112d52254f86d5854f3da734a52b4-Paper-Conference.pdf) [\[code\]](https://github.com/GeometricBCI/riemannian-score-sde/blob/main/README.md) |
| Graphgdp: Generative diffusion processes for permutation invariant graph generation | **IEEE** | 2022 | [\[paper\]](https://arxiv.org/abs/2212.01842) [\[code\]](https://github.com/GRAPH-0/GraphGDP) |
| SE(3) diffusion model with application to protein backbone generation | **arXiv** | 2023 | [\[paper\]](https://arxiv.org/abs/2302.02277) [\[code\]](https://github.com/jasonkyuyim/se3_diffusion) |
| Broadly applicable and accurate protein design by integrating structure prediction networks and diffusion generative models | **BioRxiv** | 2022 | [\[paper\]](https://www.biorxiv.org/content/10.1101/2022.12.09.519842v1) [\[code\]](https://github.com/RosettaCommons/RFdiffusion) |
| Equivariant 3D-conditional diffusion model for molecular linker design | **Nature Machine Intelligence** | 2024 | [\[paper\]](https://arxiv.org/abs/2210.05274) [\[code\]](https://github.com/igashov/DiffLinker) |

**Non-equivarian Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Riemannian score-based generative modelling | **NeurIPS** | 2022 | [\[paper\]](https://proceedings.neurips.cc/paper_files/paper/2022/file/105112d52254f86d5854f3da734a52b4-Paper-Conference.pdf) [\[code\]](https://github.com/oxcsml/riemannian-score-sde)
| Nvdiff: Graph generation through the diffusion of node vectors | **arXiv** | 2023 | [\[paper\]](https://arxiv.org/abs/2211.10794) |
| Graphgdp: Generative diffusion processes for permutation invariant graph generation | **IEEE** | 2022 | [\[paper\]](https://arxiv.org/abs/2212.01842) [\[code\]](https://github.com/GRAPH-0/GraphGDP) |
| Protein structure generation via folding diffusion | **Nature Communications** | 2024 | [\[paper\]](https://www.nature.com/articles/s41467-024-45051-2) [\[code\]](https://github.com/microsoft/foldingdiff) |
___







