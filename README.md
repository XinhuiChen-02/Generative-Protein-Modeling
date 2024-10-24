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
| Protgpt2 is a deep unsupervised language model for protein design | **Nature communications** | 2022 | [\[paper\]](https://www.nature.com/articles/s41467-022-32007-7) |
|Large language models generate functional protein sequences across diverse families | **Nature Biotechnology** | 2022 | [\[paper\]](https://www.nature.com/articles/s41587-022-01618-2) |

**Structure-based Protein Design Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| Learning from Protein Structure with Geometric Vector Perceptrons | **ICLR** | 2021 | [\[paper\]](https://arxiv.org/abs/2009.01411) [\[code\]](https://github.com/drorlab/gvp) |
| psfun: geometry-aware protein sequence function predictions with language models | **Nucleic Acids Res** | 2024 | [\[paper\]](https://pubmed.ncbi.nlm.nih.gov/38738636/) |

**Sequence and Structure Co-generation Models**
| Publication  | Venue | Year | Resource |
|:------|:----:|---------:|---------:|
| rotein sequence and structure co-design with equivariant translation | **arXiv** | 2022 | [\[paper\]](https://arxiv.org/abs/2210.08761) |
| unctional geometry guided protein sequence and backbone structure co-design. | **arXiv** | 2023 | [\[paper\]](https://arxiv.org/abs/2310.04343v3) |

___
## Autoregressive Models
>**Remark**: Autoregressive models have emerged as powerful tools in protein sequence generation, evolving from early ***RNNs*** and ***LSTMs*** that capture long-range dependencies, to advanced ***Transformer*** architectures leveraging self-attention mechanisms and large-scale pre-training, and further to ***Graph Neural Networks*** that naturally represent protein structures.

**RNN-based Models**

**LSTM-based Models**

**Transformer-based Models**

**GNN-based Models**

___
## Diffusion Models
>**Remark**: Diffusion models in protein structure generation have evolved along two significant dimensions. From a geometric perspective, the field has progressed from ***Euclidean*** approaches that treat proteins as simple point sets to more sophisticated ***geometric*** methods that leverage manifold-based representations and graph structures, enabling better capture of intrinsic protein properties. From a transformation perspective, the field has explored both ***equivariant*** methods that maintain rotational and translational symmetry through sophisticated mathematical frameworks, and ***non-equivariant*** approaches that address protein chirality through internal coordinate representations.

**Euclidean Models**

**Geometric Models**

**Equivariant Models**

**Non-equivarian Models**

___







