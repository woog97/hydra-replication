# hydra-extension

Replication of "The Hydra Effect: Emergent Self-repair in Language Model Computations" ([link](https://arxiv.org/abs/2307.15771))

WORK IN PROGRESS  
This is a self contained jupyter notebook containing the original paper's contents, along with code that implements all of its methods.  
Once this is done, another copy will be made to extend the results to study its emergence over model size and training, as well as the effects of multiple ablations and other phenomena.  


To Do (Section 2):
- [x] Boilerplate pip installs
- [x] All latex equations and text
- [x] All figures
- [x] Insert codeblocks and pseudocode for all methods
- [x] Section 2.1: Print model config
- [x] Section 2.2: Load and munge Counterfact dataset
- [ ] General equivalence classes to handle all Counterfact prompt formats
- [x] Ordinary resampling ablation
- [ ] Averaged resampling ablation
- [x] $\text{do}(\ .)$
- [ ] Multiple layer ablations
- [x] Section 2.3: $u$ unembedding, $\hat{pi_t}$, $\Delta_{\text{unembed},l}$
- [x] Section 2.4: $\Delta_{\text{ablate},l}$
- [x] Section 2.5: Produce the plots in figure 2
- [x] Implement $\tilde{\Delta}_{\text{unembed},l}^k$
- [x] Produce plots in figure 1, 3
- [x] Derive same or different conclusions across model suite
  - Pythia models are too weak for the given task of "What is the twin city of {}? It is"
  - [ ] Try a different recall task
  - [ ] Try few k-shot prompt to encourage the model to play nice

To do (Sections 3 & 4):
- [ ] Total effect
- [ ] Direct effect
- [ ] Indirect effect
- [ ] Generalized: $Y(x_{\leq t} \mid \text{do}(Z = z'))$
  - Not really worth doing
- [x] Determine whether "unrolled" RMS math in Section 3.1 applies to our LayerNormPre (it should, if we center first?)
- [ ] Section 4: Compensatory effect
- [ ] Generate CE/DE dataset
- [ ] Produce plots in figure 7, 8
- [ ] Derive same or different conclusions across model suite
