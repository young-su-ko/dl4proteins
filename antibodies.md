# Papers related to antibodies

## 1. [Efficient evolution of human antibodies from general protein language models](https://www.nature.com/articles/s41587-023-01763-2) (Unfinished)
<details>
<summary>Summary</summary>

Here we report that general protein language models can efficiently evolve human antibodies by suggesting mutations that are evolutionarily plausible
### Ideas
ESM2 can be used to generate "realistic" sequence for augmentation purposes? 

[Github link](https://github.com/brianhie/efficient-evolution)
</details>

## 2. [AbDiffuser: full-atom generation of in-vitro functioning antibodies](https://openreview.net/pdf?id=7GyYpomkEa)
<details>
<summary>Summary</summary>
AbDiffuser is an equivariant and physics-informed diffusion model that generates antibody 3D structures and sequences. It has a new protein structure representation method, new architecture for aligned proteins, and inductive biases to improve denoising. 

Previous works generate Abs by making new sequences that resemble natural ones. Limitation to sequence-based is it is hard to determine an antibody potency without inspecting 3D active site. Structure determines function. New paradigm is equivariant diffusion. Usually generate partial structures, and thenr efined by adding side chains and optimizing atom positions to forma full protein. Most protein models rely on SE(3) equivariance and represents part of protein geometry in angle space (which is complex). Use family-specific priors. (In this case antibody family). Use new SE(3) neural network arch. called APMixer. 

Denoising diffusion for protein generation:
Denoising diffusion framework, given datapoint X0, the forward diffusion adds noise to form corrupted samples Xt, getting noisier as it moves forward. Markovian process, so each step of adding noise depends on the immediately previous step, not the entire history. Gaussian is an easy to sample prior. To generate new data, the NN learns to approximate the true denoising process by minimizing the variational upper bound of NLL. 

AlignedProtein Mixer: 
Process proteins from a family of aligned proteins. (**Idea**: train PPI model using clusters, with apmixer?) We can represent antibodies as a fixed length sequence. **Aligned sequences provide more allow model to learn the specific role of that residue.** Other models such as 1D CNN or transformer can be used in place of the MLP. 

Physics-informed Residue Reps by Projection:
Atoms in a protein abide by physical constraints. In theory a NN can learn these constraints with enough data. But in low data regime, it can be better to constrain model. Prev. work represent proteins in terms of rotation and translation of rigid frams. Operating in angle space adds complexity. Instead, use non-parametric projection layer. The model and noising process allow atoms to move freely, but projection layer corrects their positions to fit constraints.

Experiments:
Evaluate ability to design antibodies. Quality of generated sequences is measured in terms of naturalness (inverse perplexity of AntiBERTy), closeness to training antibody, and stability estimated by IgFold. 

</details>
