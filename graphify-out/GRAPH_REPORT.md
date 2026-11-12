# Graph Report - qumof  (2026-11-12)

## Corpus Check
- 115 files · ~110,615 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 16 file(s) not represented in the graph (top: .jsonl 10, (none) 4, .xyz 1)

## Summary
- 1670 nodes · 4510 edges · 94 communities (81 shown, 13 thin omitted)
- Extraction: 94% EXTRACTED · 6% INFERRED · 0% AMBIGUOUS · INFERRED: 265 edges (avg confidence: 0.89)
- Token cost: 171,150 input · 0 output

## Community Hubs (Navigation)
- Orchestrator & AiiDA WorkChain
- Literature & Dataset Agents
- Structures & Job Transfer
- Scheme View & Artifact Store
- Milestone C/DFT Model Tests
- Fixture Pipeline Isolation Tests
- QUBO Encoding & Pipeline Diagram
- Periodic DFT Backend
- Candidate Dedup & Optimization
- MLIP Screening & Validation
- QAOA & QPU Solvers
- PySCF Worker
- No-Agent Fixture Core
- Toy Framework Test Helpers
- Electronic Structure Solvers
- Agent Runner Tests
- Agent Prompt Packets
- Physical Intake Validation Tests
- Shared Contract & Ranking
- Project Spec Protocol Checks
- Hamiltonian Fitting & Refinement
- Framework Slot Lattice
- LLM Client & Cache
- A2 Design Compiler
- Cluster Embedding Correction
- Acceptance & Evaluation Artifacts
- Intake Contract Tests
- AgentRun Graph Nodes
- Project Intake Spec
- Agent Output Validation
- Configuration Model Features
- Cluster Catalogue
- MUF-7 Full Benchmark Script
- MLIP/PORMAKE Workers
- Acquisition Model
- Fixture Docs & MOF-5 Case
- CIF Parsing
- PySCF Backend Tests
- Agent Controls
- Encoding/Solver Tests & Conftest
- AiiDA Loader & Dataset Fetch
- Controls: Datasets Config
- MUF-7 LLM Benchmark Figure
- Grouped Model Selection
- Geometry Matching
- Model & Symmetry Tests
- Sequential Agent Graph
- Controls: Literature Config
- Embedding Cut Region
- Topology Builders
- Controls: OpenRouter Config
- Quadratization Tests
- Replay Client
- Holdout Evaluation & Transfer
- Controls: Assessment & Cache
- Framework Bond Graph
- Mock MLIP/PW Workers
- Refinement & Gateway Tests
- PySCF Toy Project Tests
- Kang 2025 Benchmark Docs
- QuMOF Pipeline Overview
- Active Space Preparation
- Cluster Worker
- Fixture Model Ladder M0-M2
- Solvers & Deterministic Mode
- OpenRouter Request Tests
- Gateway Proposal Review
- Controls: Material Fields
- Embedding Benchmarks (CCSD/SQD)
- Parent Substitution Builder
- End-to-End Pipeline Tests
- OpenRouter Benchmark Runner
- Design Bench Tests
- PORMAKE Builder Adapter
- QPU Worker Circuits
- Controls: MCP Valency
- Active Learning & A4 Feedback
- Agent Policy Boundaries
- Agent Output Contracts
- Cluster Polynomials
- Topology Selection Policy
- MOF-5 Scheme Fixture
- QAOA Device Assessment
- A67 Assessment Packet
- Recipe Formula Parsing
- Controls: Budget
- Controls: HF Source
- Controls: Agent Token Limits
- Optional Extras & Builders
- A3/A67 & MOF Databases
- DFT Protocol Errors
- Package Metadata
- Next Steps

## God Nodes (most connected - your core abstractions)
1. `PipelineError` - 171 edges
2. `make_record()` - 85 edges
3. `load_project()` - 82 edges
4. `StageStatus` - 62 edges
5. `content_hash()` - 49 edges
6. `Pipeline` - 49 edges
7. `run_pipeline()` - 48 edges
8. `RunStore` - 43 edges
9. `AgentRun` - 37 edges
10. `validate_project()` - 33 edges

## Surprising Connections (you probably didn't know these)
- `test_stopping_rules_never_report_budget_or_starvation_as_convergence()` --uses--> `StopReason`  [INFERRED]
  tests/test_milestone_c.py → src/qumof/contract.py
- `failing()` --calls--> `make_record()`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/contract.py
- `test_job_restart_reuses_successful_work()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `test_physical_pipeline_completes_with_dft_ranking()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `Agent A4 / A2 expansion (feedback loop)` --semantically_similar_to--> `Bounded active-learning loop (disabled initially)`  [INFERRED] [semantically similar]
  README.md → mof_no_agent_fixture/AGENT_INSTRUCTIONS.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **LLM agent roles A1-A4 in the QuMOF loop** — readme_agent_a1, readme_agent_a2, readme_agent_a3, readme_agent_a4, readme_agents_judgement_only [EXTRACTED 1.00]
- **Nested fixture candidate models M0-M2 selected by complexity policy** — mof_no_agent_fixture_readme_model_m0, mof_no_agent_fixture_readme_model_m1, mof_no_agent_fixture_readme_model_m2, mof_no_agent_fixture_readme_model_selection_policy [EXTRACTED 1.00]
- **High-level metal-node correction solvers in subtractive embedding** — readme_subtractive_embedding, readme_ccsd, readme_casci, readme_vqe, readme_sqd [EXTRACTED 1.00]
- **MUF-7 benchmark pipeline stages A1-A3** — docs_muf7_benchmark_a1_qubo_construction, docs_muf7_benchmark_a2_qaoa_qubo_solution, docs_muf7_benchmark_a2_qaoa_raw_prediction, docs_muf7_benchmark_a3_vqe_prediction [EXTRACTED 1.00]
- **LLM agents compared on MUF-7** — docs_muf7_benchmark_qwen3_8_max, docs_muf7_benchmark_qwen3_8_flash, docs_muf7_benchmark_deepseek_v4_pro, docs_muf7_benchmark_deepseek_v4_flash [EXTRACTED 1.00]
- **Five-stage MOF discovery pipeline flow** — docs_new_pipeline_text_input_stage, docs_new_pipeline_topology_search_stage, docs_new_pipeline_qubo_stage, docs_new_pipeline_ground_state_evaluation_stage, docs_new_pipeline_confirmation_stage [EXTRACTED 1.00]
- **AI agents A1-A4 driving the pipeline** — docs_new_pipeline_agent_a1_topology_selector, docs_new_pipeline_agent_a2_qubo_constructor, docs_new_pipeline_agent_a3_physical_validator, docs_new_pipeline_agent_a4_qubo_adjuster [EXTRACTED 1.00]
- **Confirmation-to-QUBO optimisation feedback loop** — docs_new_pipeline_agent_a3_physical_validator, docs_new_pipeline_agent_a4_qubo_adjuster, docs_new_pipeline_agent_a2_qubo_constructor, docs_new_pipeline_qubo_hamiltonian [EXTRACTED 1.00]

## Communities (94 total, 13 thin omitted)

### Community 0 - "Orchestrator & AiiDA WorkChain"
Cohesion: 0.05
Nodes (16): MofPipeWorkChain, record_stage(), check_no_holdout(), Pipeline, StageOutcome, ranking_order_changed(), validate_structures(), _agent_section() (+8 more)

### Community 1 - "Literature & Dataset Agents"
Cohesion: 0.06
Nodes (24): candidate_descriptors(), _elements_from_formula(), gather_datasets(), match_score(), project_descriptors(), ReferenceDataset, _sha256(), _text() (+16 more)

### Community 2 - "Structures & Job Transfer"
Cohesion: 0.09
Nodes (23): check_feature_symmetry(), generate_seed_decorations(), take(), build_framework(), canonical_bits(), check_candidate_file(), configuration_id(), decode_species() (+15 more)

### Community 3 - "Scheme View & Artifact Store"
Cohesion: 0.08
Nodes (13): _load(), _models_for(), _row(), scheme_trace(), scripted_a1(), scripted_a2(), scripted_a4(), scripted_a67() (+5 more)

### Community 4 - "Milestone C/DFT Model Tests"
Cohesion: 0.06
Nodes (23): load_artifacts(), _state(), test_acquisition_is_seeded_and_favours_the_undersampled_uncertain_topology(), test_reference_competition_never_certifies_with_missing_references(), test_refinement_acquires_only_unlabelled_orbits_with_reasons(), test_relaxed_geometry_equivalence_uses_structure_not_energy(), test_rerun_and_interrupted_refinement_reuse_every_dft_job(), test_stopping_rules_never_report_budget_or_starvation_as_convergence() (+15 more)

### Community 5 - "Fixture Pipeline Isolation Tests"
Cohesion: 0.08
Nodes (33): load_project(), run_pipeline(), copy_fixture(), runs(), toy_run(), test_agent_plan_requires_the_agent_policy(), test_holdout_label_smuggled_into_training_halts_run(), _state() (+25 more)

### Community 6 - "QUBO Encoding & Pipeline Diagram"
Cohesion: 0.07
Nodes (31): New QuMOF Pipeline Diagram, Agent A1: MOF Topology Selector, Agent A2: QUBO Hamiltonian Constructor, Agent A3: Physical Correctness Checker, Agent A4: QUBO Hamiltonian Adjuster, Classical DFT, Confirmation Stage, Ground State Evaluation Stage (+23 more)

### Community 7 - "Periodic DFT Backend"
Cohesion: 0.07
Nodes (11): _carts(), difference_convergence_study(), evaluate_geometry(), formula_units(), _kmesh(), PeriodicDFTBackend, failed(), protocol_fingerprint() (+3 more)

### Community 8 - "Candidate Dedup & Optimization"
Cohesion: 0.09
Nodes (18): deduplicate_candidates(), select_pool(), predict(), bit_string(), make_record(), complete_assignment(), evaluate_encoding(), _IntPoly (+10 more)

### Community 9 - "MLIP Screening & Validation"
Cohesion: 0.09
Nodes (14): ML-potential screening (orb-v3 + D3BJ), write_cif(), MLPotentialBackend, calibrate(), _endpoint(), _mixing(), _relaxation_record(), screen() (+6 more)

### Community 10 - "QAOA & QPU Solvers"
Cohesion: 0.11
Nodes (13): content_hash(), one_hot_states(), rec(), _resolve(), apply_mixer(), evolve(), exchange_pairs(), run_qaoa() (+5 more)

### Community 11 - "PySCF Worker"
Cohesion: 0.11
Nodes (21): basis_and_pseudo_hashes(), build_cell(), _dispersion_model(), Evaluator, _host(), _initial_guess(), main(), parse_dispersion() (+13 more)

### Community 12 - "No-Agent Fixture Core"
Cohesion: 0.17
Nodes (25): bit_string(), canonical(), check_energy_compatibility(), compile_pair_qubo(), correction(), evaluate_qubo(), feasible_states(), features() (+17 more)

### Community 13 - "Toy Framework Test Helpers"
Cohesion: 0.11
Nodes (20): _deep_merge(), base_spec(), pyscf_dft_protocol(), test_round_cap_before_stability_is_budget_exhausted_not_converged(), test_validated_correction_feeds_the_ranking_and_a_constant_correction_changes_nothing(), test_physical_project_refuses_fixture_case_modes(), scheme_project(), test_every_scheme_box_runs_and_leaves_evidence() (+12 more)

### Community 14 - "Electronic Structure Solvers"
Cohesion: 0.13
Nodes (18): problem_from_artifact(), _apply(), exact_diagonalization(), hamiltonian_matrix(), _np(), _problem(), pyscf_casci(), _recover() (+10 more)

### Community 15 - "Agent Runner Tests"
Cohesion: 0.17
Nodes (22): a1(), a2(), a67(), _a67_packet(), controls(), FakeValency, gather_datasets_for_fixture_is_not_applicable(), run_agents() (+14 more)

### Community 16 - "Agent Prompt Packets"
Cohesion: 0.15
Nodes (20): build_a1_packet(), build_a2_packet(), build_a4_packet(), candidate_quality(), compilation_options(), _composition_feasible(), constraint_policy_id(), construction_options() (+12 more)

### Community 17 - "Physical Intake Validation Tests"
Cohesion: 0.14
Nodes (20): validate_project(), test_milestone_c_spec_errors_block_at_intake(), codes(), test_cif_parse_expands_symmetry_and_keeps_provenance(), test_construction_failure_is_reported_never_an_energy(), test_invalid_connector_declaration_caught(), test_invalid_structural_inputs_caught_before_any_calculation(), test_known_parent_gives_checked_slot_lattice() (+12 more)

### Community 18 - "Shared Contract & Ranking"
Cohesion: 0.14
Nodes (10): solve_exact(), JobState, StageStatus, StopReason, electronic_stage_status(), SyntheticFixtureBackend, evaluate_reference_mixtures(), rank_candidates() (+2 more)

### Community 19 - "Project Spec Protocol Checks"
Cohesion: 0.13
Nodes (17): requested_cutoff(), tolerance_errors(), protocol_errors(), protocol_errors(), _block_errors(), _cell_label(), _err(), _get() (+9 more)

### Community 20 - "Hamiltonian Fitting & Refinement"
Cohesion: 0.12
Nodes (15): feature_vector(), fit_and_select(), least_squares_exact(), check_energy_compatibility(), check_snapshot_against_split(), freeze_split(), ingest_labels(), merge_snapshots() (+7 more)

### Community 21 - "Framework Slot Lattice"
Cohesion: 0.13
Nodes (15): build_framework(), build_slot_lattice(), _centroid(), expand_supercell(), formula_counts(), _frac_close(), _fraction(), geometry_hashes() (+7 more)

### Community 22 - "LLM Client & Cache"
Cohesion: 0.14
Nodes (9): AgentCallError, Cache, cache_key(), call_role(), check_schema(), Ledger, _ask(), canonical_json() (+1 more)

### Community 23 - "A2 Design Compiler"
Cohesion: 0.17
Nodes (16): _bits(), compile_design(), evaluate_polynomial(), feasible_states(), _fmt(), kang_spectrum(), _mean(), qaoa_probabilities() (+8 more)

### Community 24 - "Cluster Embedding Correction"
Cohesion: 0.14
Nodes (8): assemble_corrected_energy(), _blocked(), ClusterBackend, correct_pool(), _molecule_structure(), plan_regions(), _structure(), validate_scheme()

### Community 25 - "Acceptance & Evaluation Artifacts"
Cohesion: 0.15
Nodes (8): check_run(), _close(), _acceptance(), _agent_metrics(), evaluate(), render(), predict_exact(), main()

### Community 26 - "Intake Contract Tests"
Cohesion: 0.19
Nodes (17): codes(), _edit_topologies(), test_cif_input_mode_unsupported(), test_duplicate_label_rejected(), test_empty_energy_set_rejected(), test_fixture_project_validates(), test_graph_relabelled_as_physical_net_rejected(), test_incompatible_energy_records_rejected() (+9 more)

### Community 28 - "Project Intake Spec"
Cohesion: 0.12
Nodes (11): project.json / project_spec.template.json, agent_request_ceilings(), _case_from_fidelity(), learner_path(), ProjectSpec, _read_json(), _read_jsonl(), runtime_agent_errors() (+3 more)

### Community 29 - "Agent Output Validation"
Cohesion: 0.18
Nodes (14): _check_model_rows(), _coverage(), _error_state(), _ok_without_errors(), _record_line(), render_assessment(), number(), ref() (+6 more)

### Community 30 - "Configuration Model Features"
Cohesion: 0.16
Nodes (11): all_model_features(), _cluster_prefix(), expand_tokens(), feature_degree(), feature_polynomial(), feature_value(), hamiltonian_from_selection(), is_known_feature() (+3 more)

### Community 31 - "Cluster Catalogue"
Cohesion: 0.20
Nodes (12): _apply(), build_catalogue(), _frac_to_cart(), _ikey(), names_for_token(), _norm(), pair_key(), parent_sites() (+4 more)

### Community 32 - "MUF-7 Full Benchmark Script"
Cohesion: 0.15
Nodes (8): Builder, cluster_vqe_sqd(), log(), main(), score(), Relaxer, spearman(), zn4o_cluster()

### Community 33 - "MLIP/PORMAKE Workers"
Cohesion: 0.20
Nodes (9): main(), _orb(), _relax(), _sha256(), _candidate_nets(), main(), _quiet(), run() (+1 more)

### Community 34 - "Acquisition Model"
Cohesion: 0.16
Nodes (10): acquisition_model(), _allocate(), bits_of(), _distance(), _normalise(), policy_errors(), _scores(), select_evaluation_batch() (+2 more)

### Community 35 - "Fixture Docs & MOF-5 Case"
Cohesion: 0.16
Nodes (15): Fixture acceptance criteria, Fixture integration instructions for coding agent, Orbit canonicalization, dedup and cross-graph pooling, BDC / 2-amino-BDC linkers (1:1), Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A), MOF-5 / IRMOF-1 (Zn4O nodes), Physical case recipe: MOF-5 BDC/amino-BDC, Correction modes (none, constant, topology_dependent) (+7 more)

### Community 36 - "CIF Parsing"
Cohesion: 0.17
Nodes (10): apply_symop(), cell_matrix(), cif_number(), _frac_distance(), _loop_with(), parse_cif(), _parse_items(), _tokens() (+2 more)

### Community 37 - "PySCF Backend Tests"
Cohesion: 0.27
Nodes (12): evaluate(), run(), settings(), test_forces_and_stress_match_finite_differences(), energy_eV(), test_kpoint_mesh_equals_replicated_cell_at_folded_mesh(), test_relax_reaches_the_declared_force_tolerance(), test_scf_failure_is_reported_without_energy() (+4 more)

### Community 38 - "Agent Controls"
Cohesion: 0.15
Nodes (5): Controls, load_controls(), _merge(), normal_requests(), _redact()

### Community 39 - "Encoding/Solver Tests & Conftest"
Cohesion: 0.19
Nodes (10): fixture_core(), harness_json(), cubic(), _hamiltonians(), pairwise(), test_cubic_model_rejected_by_qubo_only_target_but_retained_as_hubo(), test_exact_enumeration_matches_known_minima(), test_qubo_matches_fixture_reference_and_identity() (+2 more)

### Community 40 - "AiiDA Loader & Dataset Fetch"
Cohesion: 0.18
Nodes (8): fetch(), load_materials(), load_aiida(), run_pipeline_aiida(), _accept(), _agents(), main(), _run_one()

### Community 41 - "Controls: Datasets Config"
Cohesion: 0.13
Nodes (15): datasets, enabled, format, hdf5, id, index, kind, license (+7 more)

### Community 42 - "MUF-7 LLM Benchmark Figure"
Cohesion: 0.20
Nodes (15): MUF-7 LLM Benchmark Figure, A1: QUBO Hamiltonian Construction (NMAE), A2: QAOA QUBO Solution (correct output probability), A2: QAOA Raw Energy Prediction (MAE), A3: VQE Final Structure Prediction, DeepSeek V4 Flash, DeepSeek V4 Pro, Kang's [1] MUF-7 QUBO (+7 more)

### Community 43 - "Grouped Model Selection"
Cohesion: 0.14
Nodes (7): assign_folds(), candidate_models(), fit_and_select_grouped(), independent_columns(), low_energy_recall(), ridge_exact(), spearman()

### Community 44 - "Geometry Matching"
Cohesion: 0.18
Nodes (8): _apply(), equivalence_classes(), equivalent(), close(), fingerprint(), _frac_to_cart(), _lattice_params(), supercell_operations()

### Community 45 - "Model & Symmetry Tests"
Cohesion: 0.19
Nodes (10): spec(), test_decoration_space_and_orbit_quotient(), test_feature_polynomials_match_counts(), test_feature_symmetry_and_swap_reachability(), test_inadequate_family_halts_with_model_inadequate(), test_model_selection_and_untouched_holdout(), test_selection_is_policy_driven_not_hardcoded(), test_split_partitions_orbits_without_leakage() (+2 more)

### Community 46 - "Sequential Agent Graph"
Cohesion: 0.16
Nodes (4): build_graph(), SequentialGraph, PipelineError, test_unusable_calculations_never_become_energies()

### Community 47 - "Controls: Literature Config"
Cohesion: 0.15
Nodes (13): literature, enabled, extra_queries, local_papers_dir, max_passage_chars, max_passages, max_sources, references (+5 more)

### Community 48 - "Embedding Cut Region"
Cohesion: 0.22
Nodes (9): cut_region(), add(), position(), _cart_to_frac(), _close_pairs(), frac_to_cart(), _norm(), _perpendicular_widths() (+1 more)

### Community 49 - "Topology Builders"
Cohesion: 0.23
Nodes (6): lattice_info_for_builder(), choose_supercell(), _decoration_check(), generate_topologies(), protocol_errors(), _resolve_python()

### Community 50 - "Controls: OpenRouter Config"
Cohesion: 0.17
Nodes (12): openrouter, api_key, app_title, app_url, base_url, deadline_s, model, provider (+4 more)

### Community 51 - "Quadratization Tests"
Cohesion: 0.26
Nodes (8): _hamiltonians(), test_branch_and_bound_agrees_and_reports_honest_gaps(), test_penalty_bound_sublattice_counts_and_one_hot(), test_pipeline_quantum_benchmark_with_quadratization(), test_published_h2_benchmark_is_reproduced(), test_qaoa_benchmark_agrees_with_exact_and_records_provenance(), test_qaoa_mixers_preserve_constraints_and_bit_order_errors_are_caught(), test_quadratized_cubic_model_reproduces_feasible_cost()

### Community 53 - "Holdout Evaluation & Transfer"
Cohesion: 0.17
Nodes (6): evaluate_holdout(), hamiltonian_from_grouped_selection(), is_transferable(), rmse(), energy_fields(), exact()

### Community 54 - "Controls: Assessment & Cache"
Cohesion: 0.18
Nodes (10): assessment, required_checks, top_k_candidates, cache, dir, enabled, orchestration, engine (+2 more)

### Community 55 - "Framework Bond Graph"
Cohesion: 0.18
Nodes (6): bond_graph(), _components(), deconstruct(), map_to_parent_slots(), _match(), _min_image_distance()

### Community 56 - "Mock MLIP/PW Workers"
Cohesion: 0.25
Nodes (5): energy(), main(), mirror_pw(), main(), namelist_value()

### Community 57 - "Refinement & Gateway Tests"
Cohesion: 0.36
Nodes (8): read_jsonl(), _al(), pipeline(), _refinement(), _small_training_fixture(), test_active_learning_recovers_cubic_model_from_sparse_start(), test_budget_exhaustion_is_not_convergence(), test_more_labels_cannot_fix_missing_interaction_term()

### Community 58 - "PySCF Toy Project Tests"
Cohesion: 0.20
Nodes (7): formate_cif(), write_pyscf_toy_project(), test_engine_identity_is_part_of_the_fidelity(), test_probe_refusals_block_the_labels_stage(), test_pyscf_job_input_carries_every_scientific_setting(), test_pyscf_physical_pipeline_end_to_end(), test_pyscf_protocol_errors_block_at_intake()

### Community 59 - "Kang 2025 Benchmark Docs"
Cohesion: 0.27
Nodes (8): kang_control (paper weighting in term catalogue), Kang, Kim & Kim 2025: Quantum Computing Based Design of Multivariate Porous Materials, Static provenance report (live literature NOT_RUN), Fixture data files (topologies, candidates, model_candidates, splits, literature_catalog), Agent A2 (Hamiltonian model design), Cu-THQ-HHTP, Kang et al. design benchmark (agents-design-bench), Py-MV-DBA-COF

### Community 60 - "QuMOF Pipeline Overview"
Cohesion: 0.22
Nodes (7): Agent A1 (topology selection), Multivariate MOFs (MTV-MOFs), Periodic DFT ranking (step 5), PySCF, QuMOF pipeline, Simulated annealing, Toy frameworks with mock DFT

### Community 61 - "Active Space Preparation"
Cohesion: 0.27
Nodes (5): integral_hash(), prepare_active_space(), read_fcidump(), _require(), test_electronic_solvers_agree_on_identical_tiny_hamiltonian()

### Community 62 - "Cluster Worker"
Cohesion: 0.29
Nodes (5): compute(), main(), _scf(), run_embedding_benchmark(), energy()

### Community 63 - "Fixture Model Ladder M0-M2"
Cohesion: 0.28
Nodes (7): Classical exact fixed-composition baseline (924 states), UNSUPPORTED_HIGHER_ORDER_WITHOUT_QUADRATIZATION, core_pairwise case, higher_order case, Model M0 (constant + unlike NN pairs), Model M1 (M0 + distance-two pairs), Model M2 (M1 + all-B path triples, cubic)

### Community 64 - "Solvers & Deterministic Mode"
Cohesion: 0.22
Nodes (7): finite_substitution_interaction_graph input mode, Composition-preserving QAOA, Exact enumeration (certified minima), Qiskit FakeBrisbane noisy device, Limitations, MUF-7, Results on MUF-7

### Community 66 - "Gateway Proposal Review"
Cohesion: 0.28
Nodes (7): review_proposal(), decide(), reject(), _proposal(), test_malformed_proposal(), test_replayed_proposals_are_validated_and_never_executed(), test_valid_proposal_is_accepted_but_not_executed_when_agents_enabled()

### Community 67 - "Controls: Material Fields"
Cohesion: 0.25
Nodes (8): doi, formula, metals, mofid, name, record_id, topology, columns

### Community 68 - "Embedding Benchmarks (CCSD/SQD)"
Cohesion: 0.39
Nodes (6): CASCI, CCSD, H2 STO-3G electronic benchmark (Szabo & Ostlund), Keto/enol HF-to-CCSD embedding benchmark, SQD (sample-based quantum diagonalization), VQE

### Community 70 - "End-to-End Pipeline Tests"
Cohesion: 0.36
Nodes (4): test_acceptance_against_harness_and_reference(), test_bookkeeping_and_provenance(), test_constant_correction_preserves_full_order(), test_topology_dependent_correction_flips_winner()

### Community 71 - "OpenRouter Benchmark Runner"
Cohesion: 0.33
Nodes (3): OpenRouterClient, run_benchmark(), work()

### Community 72 - "Design Bench Tests"
Cohesion: 0.43
Nodes (5): build_packet(), design(), test_design_contract_rejects_invalid_or_constant_hamiltonians(), test_model_designs_are_compiled_solved_and_scored_against_the_experimental_arrangement(), test_reference_reproduces_the_published_spectrum_and_scores_the_paper_weighting_as_exact()

### Community 74 - "QPU Worker Circuits"
Cohesion: 0.48
Nodes (5): _device(), dicke(), main(), qaoa_circuit(), _scs()

### Community 75 - "Controls: MCP Valency"
Cohesion: 0.33
Nodes (6): mcp, valency, api_token, enabled, timeout_s, url

### Community 79 - "Cluster Polynomials"
Cohesion: 0.33
Nodes (3): cluster_lookup(), cluster_polynomial(), cluster_value()

### Community 81 - "MOF-5 Scheme Fixture"
Cohesion: 0.53
Nodes (3): sha(), spec_dict(), write_mof5_scheme_project()

### Community 82 - "QAOA Device Assessment"
Cohesion: 0.60
Nodes (3): assess(), fake_device(), run_one()

### Community 83 - "A67 Assessment Packet"
Cohesion: 0.40
Nodes (3): build_a67_packet(), candidate_rows(), _structural_checks()

### Community 84 - "Recipe Formula Parsing"
Cohesion: 0.40
Nodes (3): parse_formula(), spec_from_recipe(), test_recipe_inventory_is_parsed_from_blocks()

### Community 85 - "Controls: Budget"
Cohesion: 0.50
Nodes (4): budget, allow_extra_request, allow_model_expansion, max_llm_requests

### Community 86 - "Controls: HF Source"
Cohesion: 0.50
Nodes (4): hf, files, repo, revision

### Community 87 - "Controls: Agent Token Limits"
Cohesion: 0.50
Nodes (4): A1, A2, A67, max_tokens

### Community 88 - "Optional Extras & Builders"
Cohesion: 0.50
Nodes (3): AiiDA workflow engine, Optional extras (agents, mlip, topology, qpu, aiida, gpu), PORMAKE

### Community 89 - "A3/A67 & MOF Databases"
Cohesion: 0.67
Nodes (3): Agent A3 / A67 (candidate assessment), CoRE MOF 2024 database, QMOF database

## Ambiguous Edges - Review These
- `refinement.py` → `Optimisation Feedback Loop`  [AMBIGUOUS]
  docs/new_pipeline.png · relation: references

## Knowledge Gaps
- **22 isolated node(s):** `qumof`, `Multivariate MOFs (MTV-MOFs)`, `Agent A1 (topology selection)`, `CoRE MOF 2024 database`, `QMOF database` (+17 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 552 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **13 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `PipelineError` connect `Sequential Agent Graph` to `Orchestrator & AiiDA WorkChain`, `Literature & Dataset Agents`, `Structures & Job Transfer`, `Scheme View & Artifact Store`, `Milestone C/DFT Model Tests`, `Fixture Pipeline Isolation Tests`, `QUBO Encoding & Pipeline Diagram`, `Periodic DFT Backend`, `Candidate Dedup & Optimization`, `MLIP Screening & Validation`, `QAOA & QPU Solvers`, `Toy Framework Test Helpers`, `Electronic Structure Solvers`, `Physical Intake Validation Tests`, `Shared Contract & Ranking`, `Project Spec Protocol Checks`, `Hamiltonian Fitting & Refinement`, `Framework Slot Lattice`, `LLM Client & Cache`, `Cluster Embedding Correction`, `Acceptance & Evaluation Artifacts`, `Intake Contract Tests`, `Project Intake Spec`, `Configuration Model Features`, `Cluster Catalogue`, `Acquisition Model`, `CIF Parsing`, `Agent Controls`, `Encoding/Solver Tests & Conftest`, `AiiDA Loader & Dataset Fetch`, `Grouped Model Selection`, `Embedding Cut Region`, `Topology Builders`, `Quadratization Tests`, `Holdout Evaluation & Transfer`, `Framework Bond Graph`, `Active Space Preparation`, `Cluster Worker`, `Topology Selection Policy`, `Recipe Formula Parsing`?**
  _High betweenness centrality (0.166) - this node is a cross-community bridge._
- **Are the 40 inferred relationships involving `PipelineError` (e.g. with `SequentialGraph` and `compute()`) actually correct?**
  _`PipelineError` has 40 INFERRED edges - model-reasoned connections that need verification._
- **What connects `qumof`, `Multivariate MOFs (MTV-MOFs)`, `Agent A1 (topology selection)` to the rest of the system?**
  _22 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Orchestrator & AiiDA WorkChain` be split into smaller, more focused modules?**
  _Cohesion score 0.05336951605608322 - nodes in this community are weakly interconnected._
- **Why does `make_record()` connect `Candidate Dedup & Optimization` to `Orchestrator & AiiDA WorkChain`, `Structures & Job Transfer`, `Scheme View & Artifact Store`, `Fixture Pipeline Isolation Tests`, `QUBO Encoding & Pipeline Diagram`, `Periodic DFT Backend`, `MLIP Screening & Validation`, `QAOA & QPU Solvers`, `Electronic Structure Solvers`, `Physical Intake Validation Tests`, `Shared Contract & Ranking`, `Project Spec Protocol Checks`, `Hamiltonian Fitting & Refinement`, `Framework Slot Lattice`, `LLM Client & Cache`, `Cluster Embedding Correction`, `Acceptance & Evaluation Artifacts`, `Project Intake Spec`, `Configuration Model Features`, `Acquisition Model`, `Grouped Model Selection`, `Holdout Evaluation & Transfer`, `Active Space Preparation`, `Cluster Worker`, `Gateway Proposal Review`, `Agent Policy Boundaries`?**
  _High betweenness centrality (0.057) - this node is a cross-community bridge._
- **Are the 38 inferred relationships involving `StageStatus` (e.g. with `evaluate_holdout()` and `fit_and_select()`) actually correct?**
  _`StageStatus` has 38 INFERRED edges - model-reasoned connections that need verification._

### Low-confidence Hints
_AMBIGUOUS edges — the extractor was unsure. Verify before acting on these._

- **What is the exact relationship between `refinement.py` and `Optimisation Feedback Loop`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._