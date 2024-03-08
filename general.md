# Papers related to deep learning / biology

### 1. [Understanding biology in the age of artificial intelligence](https://arxiv.org/pdf/2403.04106.pdf) (unfinished)
<details>
<summary>Summary</summary>

Use of ML for bio is widespread but it is a deviation from traditional methods of scientific inquiry. Authors observe many approaches are difficult to characterize epistemologically. Philisophical justification for various aspects of 
ML is underdeveloped. Usually, we try to explain natural phenomena as the consequences of scientific explanations (Ball falls because of gravity? Things like that?) In biological science, scientific models
underlying phenomena are qualitatively described. In physics, goal is to develop computational "shortcuts" to predict behavior of natural systems (v=v0+at), but it is harder to do so in bio.
Bio problems have multidimensionality (many moving parts), conditionality (enviroment affects behavior; in vitro vs in vivo), and emergence (bio is not like lego where you can piece things together). 
In bio, answering scientific questions relies on inductive reasoning, where we get data and try to make an inference about some wider phenomena. But because of the three challenges above, ML may be able to
effectively model bio phenomena. Questions to answer: how can ML be designed to model bio phenomena, what extent do ML understand bio, what advantages/limiations of ML in bio?

ML for bio aims to identify patterns from observations, generalize that knowledge to new data. Challenge is overfitting, which can fall into two categories (model-related and data-related). 
Multidimensional complexity of bio systems --> hard to collect data that captures sufficient information. Curse of dimensionality --> ML models need more data as dimensionality of input increases.
High dim models maybe less conducive to science because maybe not model true causal dependencies. Also data is usually in vitro but try to predict for in vivo systems. "Many bio phen. difficult to describe
numerically due to... significant dependence on other factors)

**Comments on PCA:** 
Bio systems have high dim. data, and manual selection of features is not possible. PCA is one approach for dim reduction. In PCA, components must be described as a weighted sum of input variables --> leads
to non-linear dim reduct. techniques (t-SNE, autoencoders, UMAP). 

**Inductive biases for designing ML architectures:** IBs are the underlying assumptions a ML model makes to make predictions on unseen data (priori assumption to generalize). Role of ML practitioners is 
to develop models with IBs that synergize with the problem (guided by domain knowledge). 3 types of IBs esp. relevant.

Locality-related: assume proximity between input provides information about characteristics of those entities which may not be positional in nature. 


</details>
