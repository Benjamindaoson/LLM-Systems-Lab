# LLM Systems Lab

A portfolio hub for **LLM post-training, reward modeling, preference optimization, and model evaluation**.

The Lab emphasizes controlled experiments and failure analysis: a high aggregate score is not sufficient unless the model succeeds for the intended reason.

## Technical focus

- Supervised fine-tuning and parameter-efficient adaptation
- Reward-model training and ranking behavior
- Preference optimization and Agent learning
- Robustness, shortcut, and distribution-shift audits
- Multimodal judges and evidence dependence
- Reproducible evaluation protocols
- Training efficiency and experiment traceability

## Featured work

| Project | Role | Focus |
| --- | --- | --- |
| [Reward Modeling Lab](https://github.com/Benjamindaoson/reward-modeling-lab) | Flagship · independent repo | 8B reward-model post-training with QLoRA and robustness audits |
| [RewardLens](https://github.com/Benjamindaoson/RewardLens) | Research flagship · independent repo | Controlled visual interventions for multimodal judge evidence dependence |
| [Chinese News Classification](https://github.com/Benjamindaoson/chinese-news-classification) | Legacy model case study | Chinese NLP classification and model compression baseline |

See the [project index](./project-index.md) for the role and release state of each line.

## Research questions

The Lab is organized around four recurring questions:

1. Does the model improve on the target task?
2. Does it rely on the intended evidence?
3. Does the improvement survive controlled perturbations?
4. Can the result be reproduced under a declared compute and data budget?

## Experiment lifecycle

```text
Question
  → Dataset and split contract
  → Training protocol
  → Primary metric
  → Shortcut / robustness audit
  → Error analysis
  → Reproducible artifact
```

## Reporting standard

Every promoted experiment should state:

- base model, data, split, and hardware;
- optimization method and trainable parameters;
- primary and diagnostic metrics;
- known limitations and negative results;
- which values are measured and which remain planned.

## Repository policy

Flagship research stays in independent repositories. Small, bounded experiments may move into `projects/` after their data licenses, code provenance, and reproducibility are checked.


## Governance

This Hub follows the shared status taxonomy, link-only policy, private-research boundary, and release/archive synchronization checklist in [GOVERNANCE.md](GOVERNANCE.md).
