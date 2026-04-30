# Graph Report - corpus-text  (2026-04-27)

## Corpus Check
- 8 files · ~104,566 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 135 nodes · 189 edges · 8 communities detected
- Extraction: 85% EXTRACTED · 15% INFERRED · 1% AMBIGUOUS · INFERRED: 28 edges (avg confidence: 0.76)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_NLE Metrics and Rationalization|NLE Metrics and Rationalization]]
- [[_COMMUNITY_Systematic Unfaithfulness and Bias|Systematic Unfaithfulness and Bias]]
- [[_COMMUNITY_Recovery and Parametric Faithfulness|Recovery and Parametric Faithfulness]]
- [[_COMMUNITY_Unlearning-Based Faithfulness|Unlearning-Based Faithfulness]]
- [[_COMMUNITY_Effectiveness Versus Faithfulness|Effectiveness Versus Faithfulness]]
- [[_COMMUNITY_KG Evaluation and Error Paths|KG Evaluation and Error Paths]]
- [[_COMMUNITY_KG-Grounded CoT Generation|KG-Grounded CoT Generation]]
- [[_COMMUNITY_Recoverability Error Types|Recoverability Error Types]]

## God Nodes (most connected - your core abstractions)
1. `Error Recovery` - 8 edges
2. `NLE Faithfulness` - 7 edges
3. `Output-level Self-consistency` - 7 edges
4. `Active Guidance` - 7 edges
5. `Confidence Trajectories` - 7 edges
6. `Unfaithful Recovery` - 7 edges
7. `Explanation Faithfulness` - 6 edges
8. `Reasoning Faithfulness` - 6 edges
9. `Generative CoT Evaluation` - 6 edges
10. `CoT Effectiveness` - 6 edges

## Surprising Connections (you probably didn't know these)
- `Indirect Effect` --semantically_similar_to--> `Accuracy Drop as Unfaithfulness Metric`  [AMBIGUOUS] [semantically similar]
  corpus-text/02_2024.findings-emnlp.882.txt → corpus-text/01_NeurIPS-2023-language-models-dont-always-say-what-they-think-unfaithful-explanations-in-chain-of-thought-prompting-Paper-Conference.txt
- `Biasing Features Test` --semantically_similar_to--> `Misleading Cue Injection`  [INFERRED] [semantically similar]
  corpus-text/03_2024.acl-long.329v2.txt → corpus-text/04_2025.emnlp-main.1516.txt
- `Faithful Chain-of-Thought` --semantically_similar_to--> `CoT Faithfulness`  [INFERRED] [semantically similar]
  corpus-text/05_2024.findings-acl.168.txt → corpus-text/06_2025.findings-acl.560.txt
- `Answer Accuracy and Reasoning Faithfulness Gap` --semantically_similar_to--> `Unfaithful CoT Issue`  [INFERRED] [semantically similar]
  corpus-text/05_2024.findings-acl.168.txt → corpus-text/06_2025.findings-acl.560.txt
- `CoT-Plan and Self-Consistency Prompting` --conceptually_related_to--> `Question Information Recall and Enhancement`  [INFERRED]
  corpus-text/05_2024.findings-acl.168.txt → corpus-text/06_2025.findings-acl.560.txt

## Hyperedges (group relationships)
- **BBH Bias Test Setup** — 01_bbh_bias_tests, 01_answer_is_always_a_bias, 01_suggested_answer_bias, 01_accuracy_drop_metric [EXTRACTED 0.95]
- **BBQ Explanation Consistency Test** — 01_bbq_social_bias_tests, 01_stereotype_aligned_predictions, 01_explanation_consistency, 01_unfaithful_cot_explanations [EXTRACTED 0.90]
- **Causal Mediation Faithfulness Measurement** — 02_causal_mediation_analysis, 02_reasoning_chain_mediator, 02_direct_effect, 02_indirect_effect, 02_counterfactual_reasoning_chains [EXTRACTED 0.94]
- **FRODO Training Architecture** — 02_frodo_framework, 02_inference_module, 02_reasoning_module, 02_direct_preference_optimization, 02_counterfactual_causal_preference_objective [EXTRACTED 0.96]
- **Cross-Paper CoT Faithfulness Thread** — 01_unfaithful_cot_explanations, 01_counterfactual_simulatability, 02_reasoning_faithfulness, 02_causal_mediation_analysis, 02_frodo_framework [INFERRED 0.78]
- **Faithfulness Tests Recast as Self-consistency** — 03_2024_acl_long_329v2_counterfactual_edits, 03_2024_acl_long_329v2_constructing_inputs_from_explanations, 03_2024_acl_long_329v2_noise_feature_importance_equivalence, 03_2024_acl_long_329v2_biasing_features, 03_2024_acl_long_329v2_corrupting_cot, 03_2024_acl_long_329v2_self_consistency [EXTRACTED 0.91]
- **CC-SHAP Aligns Answer and Explanation Input Contributions** — 03_2024_acl_long_329v2_cc_shap, 03_2024_acl_long_329v2_input_contributions, 03_2024_acl_long_329v2_shapley_values, 03_2024_acl_long_329v2_self_consistency [EXTRACTED 0.94]
- **CoT Influence and Faithfulness Split** — 04_2025_emnlp_main_1516_confidence_trajectories, 04_2025_emnlp_main_1516_active_guidance, 04_2025_emnlp_main_1516_unfaithful_cot, 04_2025_emnlp_main_1516_verbalisation [EXTRACTED 0.93]
- **Cue-based CoT Faithfulness Protocol** — 04_2025_emnlp_main_1516_cue_injection, 04_2025_emnlp_main_1516_professor_cue, 04_2025_emnlp_main_1516_metadata_cue, 04_2025_emnlp_main_1516_verbalisation, 04_2025_emnlp_main_1516_unfaithful_cot [EXTRACTED 0.95]
- **Model-family CoT Dynamics Comparison** — 04_2025_emnlp_main_1516_instruction_tuned_models, 04_2025_emnlp_main_1516_reasoning_models, 04_2025_emnlp_main_1516_distilled_reasoning_models, 04_2025_emnlp_main_1516_confidence_trajectories, 04_2025_emnlp_main_1516_soft_reasoning_tasks [EXTRACTED 0.92]
- **KG-Grounded CoT Evaluation Loop** — 05_2024.findings-acl.168_structured_cot_prompting, 05_2024.findings-acl.168_triple_retrieval, 05_2024.findings-acl.168_reasoning_path, 05_2024.findings-acl.168_reasoning_path_evaluation [EXTRACTED 0.94]
- **Faithful Reasoning Error Modes** — 05_2024.findings-acl.168_factual_error_path, 05_2024.findings-acl.168_incoherent_path, 05_2024.findings-acl.168_misguided_path, 05_2024.findings-acl.168_faithful_cot [EXTRACTED 0.93]
- **CoT Effectiveness Factors** — 06_2025.findings-acl.560_problem_difficulty, 06_2025.findings-acl.560_information_gain, 06_2025.findings-acl.560_information_flow, 06_2025.findings-acl.560_cot_effectiveness [EXTRACTED 0.96]
- **Unfaithful CoT Information Pattern** — 06_2025.findings-acl.560_question_to_cot_info_miss, 06_2025.findings-acl.560_cot_to_answer_info_miss, 06_2025.findings-acl.560_question_to_answer_recall, 06_2025.findings-acl.560_unfaithful_cot_issue [EXTRACTED 0.95]
- **Faithfulness and Effectiveness Bridge** — 05_2024.findings-acl.168_answer_accuracy_gap, 06_2025.findings-acl.560_unfaithful_cot_issue, 06_2025.findings-acl.560_quire, 06_2025.findings-acl.560_cot_effectiveness [INFERRED 0.82]
- **FUR Parametric Faithfulness Pipeline** — 07_2025_emnlp_main_504v2_chain_of_thought, 07_2025_emnlp_main_504v2_reasoning_step_unlearning, 07_2025_emnlp_main_504v2_prediction_shift, 07_2025_emnlp_main_504v2_parametric_faithfulness [EXTRACTED 0.95]
- **Unlearning Validity Controls** — 07_2025_emnlp_main_504v2_efficacy, 07_2025_emnlp_main_504v2_specificity, 07_2025_emnlp_main_504v2_general_capabilities [EXTRACTED 0.93]
- **Faithfulness Metrics for Reasoning Steps** — 07_2025_emnlp_main_504v2_ff_hard, 07_2025_emnlp_main_504v2_ff_soft, 07_2025_emnlp_main_504v2_prediction_shift [EXTRACTED 0.94]
- **Error Recovery Behavior Taxonomy** — 08_1322_faithful_and_unfaithful_e_error_recovery, 08_1322_faithful_and_unfaithful_e_faithful_recovery, 08_1322_faithful_and_unfaithful_e_unfaithful_recovery, 08_1322_faithful_and_unfaithful_e_correct_answer_despite_flawed_reasoning [EXTRACTED 0.96]
- **Error Recovery Interventions** — 08_1322_faithful_and_unfaithful_e_error_magnitude, 08_1322_faithful_and_unfaithful_e_context_noise, 08_1322_faithful_and_unfaithful_e_error_recovery_prompt, 08_1322_faithful_and_unfaithful_e_recoverability [EXTRACTED 0.90]
- **CoT Faithfulness Cross-Paper Bridge** — 07_2025_emnlp_main_504v2_parametric_faithfulness, 07_2025_emnlp_main_504v2_contextual_faithfulness, 08_1322_faithful_and_unfaithful_e_unfaithful_recovery, 08_1322_faithful_and_unfaithful_e_invalid_reasoning_text [INFERRED 0.78]

## Communities

### Community 0 - "NLE Metrics and Rationalization"
Cohesion: 0.09
Nodes (32): Biasing Features Test, CC-SHAP, Chat LLMs, Comparative Consistency Bank, Constructing Inputs from Explanations Test, Corrupting CoT Test, Chain-of-Thought Explanations, Counterfactual Edits Test (+24 more)

### Community 1 - "Systematic Unfaithfulness and Bias"
Cohesion: 0.1
Nodes (30): Accuracy Drop as Unfaithfulness Metric, Answer is Always A Bias, BBH Bias Tests, BBQ Social Bias Tests, Biasing Features, Chain-of-Thought Prompting, Counterfactual Simulatability, Debiasing Prompts (+22 more)

### Community 2 - "Recovery and Parametric Faithfulness"
Cohesion: 0.15
Nodes (19): Add-Mistake Baseline, Alternative Explanations, Chain of Thought, Contextual Faithfulness, Multi-Hop MCQA Datasets, Parametric Faithfulness, Context Noise, Correct Answer Despite Flawed Reasoning (+11 more)

### Community 3 - "Unlearning-Based Faithfulness"
Cohesion: 0.12
Nodes (18): Content Tokens, Unlearning Efficacy, FF-HARD, FF-SOFT, Forget Set, Faithfulness by Unlearning Reasoning Steps, General Capabilities Preservation, LLM-as-a-Judge Reasoning Comparison (+10 more)

### Community 4 - "Effectiveness Versus Faithfulness"
Cohesion: 0.21
Nodes (14): AAE Recall and IG Vote, Towards Better Chain-of-Thought: Effectiveness and Faithfulness, CoT Effectiveness, CoT Faithfulness, CoT-to-Answer Information Miss, CoT-Answer Information Flow, CoT Information Gain, Logical Reasoning Unfaithfulness (+6 more)

### Community 5 - "KG Evaluation and Error Paths"
Cohesion: 0.24
Nodes (10): Answer Accuracy and Reasoning Faithfulness Gap, CoT-Plan and Self-Consistency Prompting, Direct Evaluation of Chain-of-Thought in Multi-hop Reasoning with Knowledge Graphs, Discriminative CoT Evaluation, Factual Error Reasoning Path, Incoherent Reasoning Path, LLM Reasoning Knowledge, Misguided Reasoning Path (+2 more)

### Community 6 - "KG-Grounded CoT Generation"
Cohesion: 0.32
Nodes (8): CWQ and GrailQA over Freebase, Faithful Chain-of-Thought, Generative CoT Evaluation, Human Evaluation of CoT Framework, Knowledge Graph Grounding, Reasoning Path, Structured CoT Prompting, Triple Retrieval from KG

### Community 7 - "Recoverability Error Types"
Cohesion: 0.5
Nodes (4): Calculation Error, Copying Error, Propagated Calculation Error, Recoverability

## Ambiguous Edges - Review These
- `Accuracy Drop as Unfaithfulness Metric` → `Indirect Effect`  [AMBIGUOUS]
  corpus-text/02_2024.findings-emnlp.882.txt · relation: semantically_similar_to

## Knowledge Gaps
- **34 isolated node(s):** `Chain-of-Thought Prompting`, `Direct Effect`, `Counterfactual Edits Test`, `Constructing Inputs from Explanations Test`, `Noise and Feature Importance Equivalence` (+29 more)
  These have ≤1 connection - possible missing edges or undocumented components.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Accuracy Drop as Unfaithfulness Metric` and `Indirect Effect`?**
  _Edge tagged AMBIGUOUS (relation: semantically_similar_to) - confidence is low._
- **Why does `Error Recovery` connect `Recovery and Parametric Faithfulness` to `Recoverability Error Types`?**
  _High betweenness centrality (0.029) - this node is a cross-community bridge._
- **Why does `CoT Faithfulness` connect `Effectiveness Versus Faithfulness` to `KG Evaluation and Error Paths`, `KG-Grounded CoT Generation`?**
  _High betweenness centrality (0.022) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `NLE Faithfulness` (e.g. with `Unfaithful CoT` and `Active Guidance`) actually correct?**
  _`NLE Faithfulness` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `Confidence Trajectories` (e.g. with `Causal-dependence Definition of CoT Faithfulness` and `Output-level Self-consistency`) actually correct?**
  _`Confidence Trajectories` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Chain-of-Thought Prompting`, `Direct Effect`, `Counterfactual Edits Test` to the rest of the system?**
  _34 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `NLE Metrics and Rationalization` be split into smaller, more focused modules?**
  _Cohesion score 0.09 - nodes in this community are weakly interconnected._