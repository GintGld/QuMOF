# Graph Report - qumof  (2026-11-12)

## Corpus Check
- 115 files · ~111,226 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 16 file(s) not represented in the graph (top: .jsonl 10, (none) 4, .xyz 1)

## Summary
- 1677 nodes · 4515 edges · 84 communities (68 shown, 16 thin omitted)
- Extraction: 94% EXTRACTED · 6% INFERRED · 0% AMBIGUOUS · INFERRED: 264 edges (avg confidence: 0.89)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `8a8a3b98`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Pipeline
- agents/datasets.py
- Structures & Job Transfer
- scheme.py
- Milestone C/DFT Model Tests
- Fixture Pipeline Isolation Tests
- QUBO Encoding & Pipeline Diagram
- Periodic DFT Backend
- Candidate Dedup & Optimization
- screening.py
- QAOA & QPU Solvers
- PySCF Worker
- No-Agent Fixture Core
- Toy Framework Test Helpers
- Electronic Structure Solvers
- Agent Runner Tests
- Agent Prompt Packets
- Physical Intake Validation Tests
- contract.py
- Project Spec Protocol Checks
- Hamiltonian Fitting & Refinement
- Framework Slot Lattice
- RunStore
- design.py
- Cluster Embedding Correction
- json
- Intake Contract Tests
- AgentRun Graph Nodes
- Project Intake Spec
- Agent Output Validation
- feature_vector
- Ground State Evaluation Stage
- time
- literature.py
- Synthetic no-agent MOF fixture
- math
- PySCF Backend Tests
- report.py
- Encoding/Solver Tests & Conftest
- aiida_engine.py
- Controls: Datasets Config
- MUF-7 LLM Benchmark Figure
- MofPipeWorkChain
- Geometry Matching
- Model & Symmetry Tests
- runner.py
- Controls: Literature Config
- Embedding Cut Region
- Topology Builders
- Controls: OpenRouter Config
- Quadratization Tests
- Replay Client
- validate_physical_project
- Controls: Assessment & Cache
- validation.py
- pathlib
- Refinement & Gateway Tests
- PySCF Toy Project Tests
- LocalPapers
- QuMOF Pipeline Overview
- test_milestone_f.py
- CLAUDE.md
- Fixture Model Ladder M0-M2
- Solvers & Deterministic Mode
- ._physical_ranking
- Gateway Proposal Review
- Controls: Material Fields
- Physical case recipe: MOF-5 BDC/amino-BDC
- End-to-End Pipeline Tests
- PORMAKE Builder Adapter
- Controls: MCP Valency
- dft.py
- Recipe Formula Parsing
- Controls: Budget
- Controls: HF Source
- Controls: Agent Token Limits
- A3/A67 & MOF Databases
- Package Metadata
- Next Steps

## God Nodes (most connected - your core abstractions)
1. `PipelineError` - 171 edges
2. `make_record()` - 85 edges
3. `load_project()` - 82 edges
4. `StageStatus` - 61 edges
5. `Pipeline` - 49 edges
6. `content_hash()` - 49 edges
7. `run_pipeline()` - 48 edges
8. `RunStore` - 43 edges
9. `AgentRun` - 37 edges
10. `validate_project()` - 33 edges

## Surprising Connections (you probably didn't know these)
- `test_stopping_rules_never_report_budget_or_starvation_as_convergence()` --uses--> `StopReason`  [INFERRED]
  tests/test_milestone_c.py → src/qumof/contract.py
- `test_job_restart_reuses_successful_work()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `test_physical_pipeline_completes_with_dft_ranking()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `failing()` --calls--> `make_record()`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/contract.py
- `Deterministic agent-free mode (qumof run)` --semantically_similar_to--> `Fixture adapter into existing interfaces`  [INFERRED] [semantically similar]
  README.md → mof_no_agent_fixture/AGENT_INSTRUCTIONS.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **LLM agents compared on MUF-7** — docs_muf7_benchmark_qwen3_8_max, docs_muf7_benchmark_qwen3_8_flash, docs_muf7_benchmark_deepseek_v4_pro, docs_muf7_benchmark_deepseek_v4_flash [EXTRACTED 1.00]
- **MUF-7 benchmark pipeline stages A1-A3** — docs_muf7_benchmark_a1_qubo_construction, docs_muf7_benchmark_a2_qaoa_qubo_solution, docs_muf7_benchmark_a2_qaoa_raw_prediction, docs_muf7_benchmark_a3_vqe_prediction [EXTRACTED 1.00]
- **AI agents A1-A4 driving the pipeline** — docs_new_pipeline_agent_a1_topology_selector, docs_new_pipeline_agent_a2_qubo_constructor, docs_new_pipeline_agent_a3_physical_validator, docs_new_pipeline_agent_a4_qubo_adjuster [EXTRACTED 1.00]
- **Confirmation-to-QUBO optimisation feedback loop** — docs_new_pipeline_agent_a3_physical_validator, docs_new_pipeline_agent_a4_qubo_adjuster, docs_new_pipeline_agent_a2_qubo_constructor, docs_new_pipeline_qubo_hamiltonian [EXTRACTED 1.00]
- **Five-stage MOF discovery pipeline flow** — docs_new_pipeline_text_input_stage, docs_new_pipeline_topology_search_stage, docs_new_pipeline_qubo_stage, docs_new_pipeline_ground_state_evaluation_stage, docs_new_pipeline_confirmation_stage [EXTRACTED 1.00]
- **Nested fixture candidate models M0-M2 selected by complexity policy** — mof_no_agent_fixture_readme_model_m0, mof_no_agent_fixture_readme_model_m1, mof_no_agent_fixture_readme_model_m2, mof_no_agent_fixture_readme_model_selection_policy [EXTRACTED 1.00]
- **LLM agent roles A1-A4 in the QuMOF loop** — readme_agent_a1, readme_agent_a2, readme_agent_a3, readme_agent_a4, readme_agents_judgement_only [EXTRACTED 1.00]
- **High-level metal-node correction solvers in subtractive embedding** — readme_subtractive_embedding, readme_ccsd, readme_casci, readme_vqe, readme_sqd [EXTRACTED 1.00]

## Communities (84 total, 16 thin omitted)

### Community 0 - "Pipeline"
Cohesion: 0.15
Nodes (3): Pipeline, StageOutcome, validate_structures()

### Community 1 - "agents/datasets.py"
Cohesion: 0.18
Nodes (9): candidate_descriptors(), _elements_from_formula(), gather_datasets(), match_score(), project_descriptors(), ReferenceDataset, _sha256(), _text() (+1 more)

### Community 2 - "Structures & Job Transfer"
Cohesion: 0.10
Nodes (22): all_model_features(), check_feature_symmetry(), build_framework(), canonical_bits(), check_candidate_file(), configuration_id(), decode_species(), define_decoration_space() (+14 more)

### Community 3 - "scheme.py"
Cohesion: 0.13
Nodes (11): _models_for(), _row(), scheme_trace(), scripted_a1(), scripted_a2(), scripted_a4(), scripted_a67(), scripted_policies() (+3 more)

### Community 4 - "Milestone C/DFT Model Tests"
Cohesion: 0.06
Nodes (22): load_artifacts(), _state(), test_acquisition_is_seeded_and_favours_the_undersampled_uncertain_topology(), test_reference_competition_never_certifies_with_missing_references(), test_refinement_acquires_only_unlabelled_orbits_with_reasons(), test_relaxed_geometry_equivalence_uses_structure_not_energy(), test_rerun_and_interrupted_refinement_reuse_every_dft_job(), test_stopping_rules_never_report_budget_or_starvation_as_convergence() (+14 more)

### Community 5 - "Fixture Pipeline Isolation Tests"
Cohesion: 0.10
Nodes (28): load_project(), run_pipeline(), copy_fixture(), runs(), toy_run(), test_agent_plan_requires_the_agent_policy(), test_holdout_label_smuggled_into_training_halts_run(), _state() (+20 more)

### Community 6 - "QUBO Encoding & Pipeline Diagram"
Cohesion: 0.09
Nodes (19): feature_polynomial(), _ancilla_coefficients(), compile_encoding(), compile_one_hot(), complete_assignment(), count_constraints(), count_penalty(), decode_one_hot() (+11 more)

### Community 7 - "Periodic DFT Backend"
Cohesion: 0.07
Nodes (11): _carts(), difference_convergence_study(), evaluate_geometry(), formula_units(), _kmesh(), PeriodicDFTBackend, failed(), protocol_fingerprint() (+3 more)

### Community 8 - "Candidate Dedup & Optimization"
Cohesion: 0.10
Nodes (13): deduplicate_candidates(), select_pool(), hamiltonian_from_selection(), bit_string(), make_record(), branch_and_bound(), exact_enumeration(), quantum_solver_status() (+5 more)

### Community 9 - "screening.py"
Cohesion: 0.14
Nodes (7): ML-potential screening (orb-v3 + D3BJ), MLPotentialBackend, _resolve(), calibrate(), _endpoint(), _mixing(), screen()

### Community 10 - "QAOA & QPU Solvers"
Cohesion: 0.10
Nodes (16): predict(), one_hot_states(), rec(), verify_encoding(), apply_mixer(), evolve(), exchange_pairs(), qaoa_benchmark() (+8 more)

### Community 11 - "PySCF Worker"
Cohesion: 0.11
Nodes (21): basis_and_pseudo_hashes(), build_cell(), _dispersion_model(), Evaluator, _host(), _initial_guess(), main(), parse_dispersion() (+13 more)

### Community 12 - "No-Agent Fixture Core"
Cohesion: 0.18
Nodes (25): bit_string(), canonical(), check_energy_compatibility(), compile_pair_qubo(), correction(), evaluate_qubo(), feasible_states(), features() (+17 more)

### Community 13 - "Toy Framework Test Helpers"
Cohesion: 0.12
Nodes (19): _deep_merge(), test_round_cap_before_stability_is_budget_exhausted_not_converged(), test_topologies_keep_their_own_cell_counts(), test_validated_correction_feeds_the_ranking_and_a_constant_correction_changes_nothing(), toy_backend(), test_physical_project_refuses_fixture_case_modes(), scheme_project(), base_spec() (+11 more)

### Community 14 - "Electronic Structure Solvers"
Cohesion: 0.08
Nodes (27): integral_hash(), prepare_active_space(), problem_from_artifact(), read_fcidump(), _require(), compute(), main(), _scf() (+19 more)

### Community 15 - "Agent Runner Tests"
Cohesion: 0.07
Nodes (28): Controls, load_controls(), _merge(), normal_requests(), _redact(), a1(), a2(), a67() (+20 more)

### Community 16 - "Agent Prompt Packets"
Cohesion: 0.12
Nodes (23): build_a1_packet(), build_a2_packet(), build_a4_packet(), build_a67_packet(), candidate_quality(), candidate_rows(), compilation_options(), _composition_feasible() (+15 more)

### Community 17 - "Physical Intake Validation Tests"
Cohesion: 0.15
Nodes (18): validate_project(), test_milestone_c_spec_errors_block_at_intake(), codes(), test_construction_failure_is_reported_never_an_energy(), test_invalid_connector_declaration_caught(), test_invalid_structural_inputs_caught_before_any_calculation(), test_known_parent_gives_checked_slot_lattice(), test_physical_policy_fields_block_with_field_path() (+10 more)

### Community 18 - "contract.py"
Cohesion: 0.08
Nodes (23): assign_folds(), candidate_models(), evaluate_holdout(), fit_and_select(), fit_and_select_grouped(), hamiltonian_from_grouped_selection(), independent_columns(), least_squares_exact() (+15 more)

### Community 19 - "Project Spec Protocol Checks"
Cohesion: 0.11
Nodes (19): requested_cutoff(), dft_protocol_errors(), tolerance_errors(), protocol_errors(), protocol_errors(), _block_errors(), _cell_label(), _err() (+11 more)

### Community 20 - "Hamiltonian Fitting & Refinement"
Cohesion: 0.09
Nodes (15): PipelineError, check_energy_compatibility(), check_no_holdout(), check_snapshot_against_split(), freeze_physical_split(), freeze_split(), ingest_labels(), merge_snapshots() (+7 more)

### Community 21 - "Framework Slot Lattice"
Cohesion: 0.13
Nodes (15): build_framework(), build_slot_lattice(), _centroid(), expand_supercell(), formula_counts(), _frac_close(), _fraction(), geometry_hashes() (+7 more)

### Community 23 - "design.py"
Cohesion: 0.05
Nodes (38): AgentCallError, Cache, cache_key(), call_role(), check_schema(), Ledger, OpenRouterClient, ReplayClient (+30 more)

### Community 24 - "Cluster Embedding Correction"
Cohesion: 0.11
Nodes (12): assemble_corrected_energy(), _blocked(), ClusterBackend, correct_pool(), _molecule_structure(), plan_regions(), run_embedding_benchmark(), _structure() (+4 more)

### Community 25 - "json"
Cohesion: 0.14
Nodes (15): check_run(), _close(), fetch(), load_materials(), _acceptance(), _agent_metrics(), evaluate(), render() (+7 more)

### Community 26 - "Intake Contract Tests"
Cohesion: 0.19
Nodes (17): codes(), _edit_topologies(), test_cif_input_mode_unsupported(), test_duplicate_label_rejected(), test_empty_energy_set_rejected(), test_fixture_project_validates(), test_graph_relabelled_as_physical_net_rejected(), test_incompatible_energy_records_rejected() (+9 more)

### Community 28 - "Project Intake Spec"
Cohesion: 0.12
Nodes (11): project.json / project_spec.template.json, agent_request_ceilings(), _case_from_fidelity(), learner_path(), ProjectSpec, _read_json(), _read_jsonl(), runtime_agent_errors() (+3 more)

### Community 29 - "Agent Output Validation"
Cohesion: 0.18
Nodes (14): _check_model_rows(), _coverage(), _error_state(), _ok_without_errors(), _record_line(), render_assessment(), number(), ref() (+6 more)

### Community 30 - "feature_vector"
Cohesion: 0.18
Nodes (8): names_for_token(), expand_tokens(), feature_value(), feature_vector(), _orbit_sites(), site_orbits(), plan_next_batch(), novelty()

### Community 31 - "Ground State Evaluation Stage"
Cohesion: 0.18
Nodes (16): New QuMOF Pipeline Diagram, Agent A1: MOF Topology Selector, Agent A2: QUBO Hamiltonian Constructor, Agent A3: Physical Correctness Checker, Agent A4: QUBO Hamiltonian Adjuster, Classical DFT, Confirmation Stage, Ground State Evaluation Stage (+8 more)

### Community 32 - "time"
Cohesion: 0.06
Nodes (25): Builder, cluster_vqe_sqd(), log(), main(), score(), Relaxer, spearman(), zn4o_cluster() (+17 more)

### Community 33 - "literature.py"
Cohesion: 0.24
Nodes (9): _accept(), _clean(), gather_evidence(), _paper_source(), query_templates(), references_from(), _resolve_calls(), title_similarity() (+1 more)

### Community 35 - "Synthetic no-agent MOF fixture"
Cohesion: 0.36
Nodes (7): Orbit canonicalization, dedup and cross-graph pooling, Correction modes (none, constant, topology_dependent), Synthetic no-agent MOF fixture, Fixture data files (topologies, candidates, model_candidates, splits, literature_catalog), Synthetic ground-truth energy formula, prism6 (hexagonal prism graph), ring12 (12-site cycle graph)

### Community 36 - "math"
Cohesion: 0.05
Nodes (38): acquisition_model(), _allocate(), bits_of(), _distance(), _normalise(), policy_errors(), _scores(), select_evaluation_batch() (+30 more)

### Community 37 - "PySCF Backend Tests"
Cohesion: 0.22
Nodes (14): evaluate(), run(), settings(), test_forces_and_stress_match_finite_differences(), energy_eV(), test_kpoint_mesh_equals_replicated_cell_at_folded_mesh(), test_probe_refusals_block_the_labels_stage(), test_pyscf_protocol_errors_block_at_intake() (+6 more)

### Community 38 - "report.py"
Cohesion: 0.24
Nodes (9): _agent_section(), build_report(), _embedding_section(), _md_table(), not_executed(), _physical_section(), _screening_section(), _topology_section() (+1 more)

### Community 39 - "Encoding/Solver Tests & Conftest"
Cohesion: 0.19
Nodes (10): fixture_core(), harness_json(), cubic(), _hamiltonians(), pairwise(), test_cubic_model_rejected_by_qubo_only_target_but_retained_as_hubo(), test_exact_enumeration_matches_known_minima(), test_qubo_matches_fixture_reference_and_identity() (+2 more)

### Community 41 - "Controls: Datasets Config"
Cohesion: 0.13
Nodes (15): datasets, enabled, format, hdf5, id, index, kind, license (+7 more)

### Community 42 - "MUF-7 LLM Benchmark Figure"
Cohesion: 0.20
Nodes (15): MUF-7 LLM Benchmark Figure, A1: QUBO Hamiltonian Construction (NMAE), A2: QAOA QUBO Solution (correct output probability), A2: QAOA Raw Energy Prediction (MAE), A3: VQE Final Structure Prediction, DeepSeek V4 Flash, DeepSeek V4 Pro, Kang's [1] MUF-7 QUBO (+7 more)

### Community 44 - "Geometry Matching"
Cohesion: 0.18
Nodes (8): _apply(), equivalence_classes(), equivalent(), close(), fingerprint(), _frac_to_cart(), _lattice_params(), supercell_operations()

### Community 45 - "Model & Symmetry Tests"
Cohesion: 0.19
Nodes (10): spec(), test_decoration_space_and_orbit_quotient(), test_feature_polynomials_match_counts(), test_feature_symmetry_and_swap_reachability(), test_inadequate_family_halts_with_model_inadequate(), test_model_selection_and_untouched_holdout(), test_selection_is_policy_driven_not_hardcoded(), test_split_partitions_orbits_without_leakage() (+2 more)

### Community 46 - "runner.py"
Cohesion: 0.15
Nodes (6): _parse_tool_result(), ValencyMCP, build_graph(), check_connections(), _local_check(), SequentialGraph

### Community 47 - "Controls: Literature Config"
Cohesion: 0.15
Nodes (13): literature, enabled, extra_queries, local_papers_dir, max_passage_chars, max_passages, max_sources, references (+5 more)

### Community 48 - "Embedding Cut Region"
Cohesion: 0.19
Nodes (10): cut_region(), add(), position(), _close_pairs(), frac_to_cart(), _match(), _min_image_distance(), _norm() (+2 more)

### Community 49 - "Topology Builders"
Cohesion: 0.13
Nodes (8): BuildFailure, lattice_info_for_builder(), ParentSubstitutionBuilder, choose_supercell(), _decoration_check(), generate_topologies(), protocol_errors(), _resolve_python()

### Community 50 - "Controls: OpenRouter Config"
Cohesion: 0.17
Nodes (12): openrouter, api_key, app_title, app_url, base_url, deadline_s, model, provider (+4 more)

### Community 51 - "Quadratization Tests"
Cohesion: 0.26
Nodes (8): _hamiltonians(), test_branch_and_bound_agrees_and_reports_honest_gaps(), test_penalty_bound_sublattice_counts_and_one_hot(), test_pipeline_quantum_benchmark_with_quadratization(), test_published_h2_benchmark_is_reproduced(), test_qaoa_benchmark_agrees_with_exact_and_records_provenance(), test_qaoa_mixers_preserve_constraints_and_bit_order_errors_are_caught(), test_quadratized_cubic_model_reproduces_feasible_cost()

### Community 53 - "validate_physical_project"
Cohesion: 0.27
Nodes (7): _feature_catalogue(), _cluster_prefix(), feature_degree(), is_known_feature(), is_transferable(), model_features(), validate_physical_project()

### Community 54 - "Controls: Assessment & Cache"
Cohesion: 0.18
Nodes (10): assessment, required_checks, top_k_candidates, cache, dir, enabled, orchestration, engine (+2 more)

### Community 55 - "validation.py"
Cohesion: 0.15
Nodes (10): write_cif(), map_to_parent_slots(), min_interatomic_distance(), _relaxation_record(), _lengths_angles(), metal_coordination(), mofchecker_check(), _structure() (+2 more)

### Community 56 - "pathlib"
Cohesion: 0.32
Nodes (3): close(), expect_error(), require()

### Community 57 - "Refinement & Gateway Tests"
Cohesion: 0.36
Nodes (8): read_jsonl(), _al(), pipeline(), _refinement(), _small_training_fixture(), test_active_learning_recovers_cubic_model_from_sparse_start(), test_budget_exhaustion_is_not_convergence(), test_more_labels_cannot_fix_missing_interaction_term()

### Community 58 - "PySCF Toy Project Tests"
Cohesion: 0.21
Nodes (7): base_spec(), formate_cif(), pyscf_dft_protocol(), write_pyscf_toy_project(), test_engine_identity_is_part_of_the_fidelity(), test_pyscf_job_input_carries_every_scientific_setting(), test_pyscf_physical_pipeline_end_to_end()

### Community 60 - "QuMOF Pipeline Overview"
Cohesion: 0.13
Nodes (14): kang_control (paper weighting in term catalogue), Kang, Kim & Kim 2025: Quantum Computing Based Design of Multivariate Porous Materials, Static provenance report (live literature NOT_RUN), Agent A1 (topology selection), Agent A2 (Hamiltonian model design), Cu-THQ-HHTP, Kang et al. design benchmark (agents-design-bench), Multivariate MOFs (MTV-MOFs) (+6 more)

### Community 61 - "test_milestone_f.py"
Cohesion: 0.32
Nodes (5): test_ml_screening_deprioritises_only_calibrated_gaps_and_narrows_the_run(), test_store_rejects_a_concurrent_writer(), test_uncalibrated_or_failed_screening_keeps_every_topology(), _toy(), _venv_has()

### Community 62 - "CLAUDE.md"
Cohesion: 0.29
Nodes (5): 1. Think Before Coding, 2. Simplicity First, 3. Surgical Changes, 4. Goal-Driven Execution, graphify

### Community 63 - "Fixture Model Ladder M0-M2"
Cohesion: 0.16
Nodes (9): Classical exact fixed-composition baseline (924 states), MODEL_INADEQUATE error, UNSUPPORTED_HIGHER_ORDER_WITHOUT_QUADRATIZATION, core_pairwise case, higher_order case, Model M0 (constant + unlike NN pairs), Model M1 (M0 + distance-two pairs), Model M2 (M1 + all-B path triples, cubic) (+1 more)

### Community 64 - "Solvers & Deterministic Mode"
Cohesion: 0.14
Nodes (11): Fixture acceptance criteria, finite_substitution_interaction_graph input mode, Fixture integration instructions for coding agent, Composition-preserving QAOA, Exact enumeration (certified minima), Qiskit FakeBrisbane noisy device, Limitations, MUF-7 (+3 more)

### Community 66 - "Gateway Proposal Review"
Cohesion: 0.28
Nodes (7): review_proposal(), decide(), reject(), _proposal(), test_malformed_proposal(), test_replayed_proposals_are_validated_and_never_executed(), test_valid_proposal_is_accepted_but_not_executed_when_agents_enabled()

### Community 67 - "Controls: Material Fields"
Cohesion: 0.25
Nodes (8): doi, formula, metals, mofid, name, record_id, topology, columns

### Community 68 - "Physical case recipe: MOF-5 BDC/amino-BDC"
Cohesion: 0.17
Nodes (13): BDC / 2-amino-BDC linkers (1:1), Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A), MOF-5 / IRMOF-1 (Zn4O nodes), Physical case recipe: MOF-5 BDC/amino-BDC, AiiDA workflow engine, CASCI, CCSD, H2 STO-3G electronic benchmark (Szabo & Ostlund) (+5 more)

### Community 70 - "End-to-End Pipeline Tests"
Cohesion: 0.36
Nodes (4): test_acceptance_against_harness_and_reference(), test_bookkeeping_and_provenance(), test_constant_correction_preserves_full_order(), test_topology_dependent_correction_flips_winner()

### Community 75 - "Controls: MCP Valency"
Cohesion: 0.33
Nodes (6): mcp, valency, api_token, enabled, timeout_s, url

### Community 81 - "dft.py"
Cohesion: 0.26
Nodes (4): _cart_to_frac(), sha(), spec_dict(), write_mof5_scheme_project()

### Community 85 - "Controls: Budget"
Cohesion: 0.50
Nodes (4): budget, allow_extra_request, allow_model_expansion, max_llm_requests

### Community 86 - "Controls: HF Source"
Cohesion: 0.50
Nodes (4): hf, files, repo, revision

### Community 87 - "Controls: Agent Token Limits"
Cohesion: 0.50
Nodes (4): A1, A2, A67, max_tokens

### Community 89 - "A3/A67 & MOF Databases"
Cohesion: 0.67
Nodes (3): Agent A3 / A67 (candidate assessment), CoRE MOF 2024 database, QMOF database

## Ambiguous Edges - Review These
- `refinement.py` → `Optimisation Feedback Loop`  [AMBIGUOUS]
  docs/new_pipeline.png · relation: references

## Knowledge Gaps
- **22 isolated node(s):** `qumof`, `BDC / 2-amino-BDC linkers (1:1)`, `Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A)`, `DeepSeek V4 Flash`, `DeepSeek V4 Pro` (+17 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 558 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **16 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `PipelineError` connect `Hamiltonian Fitting & Refinement` to `Pipeline`, `Structures & Job Transfer`, `Milestone C/DFT Model Tests`, `Fixture Pipeline Isolation Tests`, `QUBO Encoding & Pipeline Diagram`, `Periodic DFT Backend`, `Candidate Dedup & Optimization`, `screening.py`, `QAOA & QPU Solvers`, `Toy Framework Test Helpers`, `Electronic Structure Solvers`, `Agent Runner Tests`, `Physical Intake Validation Tests`, `contract.py`, `Project Spec Protocol Checks`, `Framework Slot Lattice`, `RunStore`, `design.py`, `Cluster Embedding Correction`, `json`, `Intake Contract Tests`, `Project Intake Spec`, `feature_vector`, `._physical_refinement`, `math`, `Encoding/Solver Tests & Conftest`, `aiida_engine.py`, `runner.py`, `Embedding Cut Region`, `Topology Builders`, `Quadratization Tests`, `validate_physical_project`, `test_milestone_f.py`, `store.py`, `dft.py`, `Recipe Formula Parsing`?**
  _High betweenness centrality (0.169) - this node is a cross-community bridge._
- **Are the 40 inferred relationships involving `PipelineError` (e.g. with `SequentialGraph` and `compute()`) actually correct?**
  _`PipelineError` has 40 INFERRED edges - model-reasoned connections that need verification._
- **What connects `qumof`, `BDC / 2-amino-BDC linkers (1:1)`, `Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A)` to the rest of the system?**
  _22 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Structures & Job Transfer` be split into smaller, more focused modules?**
  _Cohesion score 0.10256410256410256 - nodes in this community are weakly interconnected._
- **Why does `make_record()` connect `Candidate Dedup & Optimization` to `Structures & Job Transfer`, `Fixture Pipeline Isolation Tests`, `QUBO Encoding & Pipeline Diagram`, `Periodic DFT Backend`, `screening.py`, `QAOA & QPU Solvers`, `Electronic Structure Solvers`, `Physical Intake Validation Tests`, `contract.py`, `Project Spec Protocol Checks`, `Hamiltonian Fitting & Refinement`, `Framework Slot Lattice`, `design.py`, `Cluster Embedding Correction`, `json`, `AgentRun Graph Nodes`, `Project Intake Spec`, `._physical_refinement`, `math`, `report.py`, `runner.py`, `validate_physical_project`, `validation.py`, `Gateway Proposal Review`, `dft.py`?**
  _High betweenness centrality (0.056) - this node is a cross-community bridge._
- **Should `scheme.py` be split into smaller, more focused modules?**
  _Cohesion score 0.13438735177865613 - nodes in this community are weakly interconnected._

### Low-confidence Hints
_AMBIGUOUS edges — the extractor was unsure. Verify before acting on these._

- **What is the exact relationship between `refinement.py` and `Optimisation Feedback Loop`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._