# Graph Report - qumof  (2026-11-15)

## Corpus Check
- 115 files · ~111,803 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 17 file(s) not represented in the graph (top: .jsonl 10, (none) 5, .xyz 1)

## Summary
- 1689 nodes · 4495 edges · 93 communities (74 shown, 19 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 207 edges (avg confidence: 0.88)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `ca460c30`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Pipeline
- agents/datasets.py
- PipelineError
- scheme.py
- Milestone C/DFT Model Tests
- dft.py
- QUBO Encoding & Pipeline Diagram
- Periodic DFT Backend
- make_record
- screening.py
- QAOA & QPU Solvers
- PySCF Worker
- No-Agent Fixture Core
- Toy Framework Test Helpers
- Electronic Structure Solvers
- test_agents.py
- packets.py
- Physical Intake Validation Tests
- contract.py
- project_spec.py
- Hamiltonian Fitting & Refinement
- Framework Slot Lattice
- RunStore
- design.py
- Cluster Embedding Correction
- StageOutcome
- Intake Contract Tests
- content_hash
- load_project
- Agent Output Validation
- run_pipeline
- Ground State Evaluation Stage
- pormake_worker.py
- hashlib
- runner.py
- Synthetic no-agent MOF fixture
- acquisition.py
- PySCF Backend Tests
- report.py
- Encoding/Solver Tests & Conftest
- cif.py
- Controls: Datasets Config
- MUF-7 LLM Benchmark Figure
- MofPipeWorkChain
- Geometry Matching
- Model & Symmetry Tests
- run_one
- Controls: Literature Config
- sys
- Topology Builders
- Controls: OpenRouter Config
- Quadratization Tests
- ReplayClient
- run_muf7_full.py
- Controls: Assessment & Cache
- validation.py
- json
- Refinement & Gateway Tests
- pathlib
- .physical_spec
- Kang et al. design benchmark (agents-design-bench)
- test_milestone_f.py
- CLAUDE.md
- Fixture Model Ladder M0-M2
- Solvers & Deterministic Mode
- controls.py
- cut_region
- Controls: Material Fields
- DFT-fitted QUBO Hamiltonian (step 3)
- rank_candidates
- .run
- OpenRouterClient
- BuildFailure
- aiida_engine.py
- Controls: MCP Valency
- scheme_trace
- ._physical_screening
- mock_mlip.py
- test_openrouter_request_follows_the_guide
- FakeValency
- dft.py
- test_reference_datasets_match_by_code_and_feed_direct_comparisons
- test_design_bench.py
- assess_refinement
- Controls: Budget
- Controls: HF Source
- Controls: Agent Token Limits
- A3/A67 & MOF Databases
- Package Metadata
- Next Steps

## God Nodes (most connected - your core abstractions)
1. `PipelineError` - 156 edges
2. `make_record()` - 85 edges
3. `load_project()` - 82 edges
4. `content_hash()` - 49 edges
5. `run_pipeline()` - 48 edges
6. `Pipeline` - 45 edges
7. `RunStore` - 40 edges
8. `StageStatus` - 36 edges
9. `AgentRun` - 32 edges
10. `validate_project()` - 32 edges

## Surprising Connections (you probably didn't know these)
- `test_job_restart_reuses_successful_work()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `test_physical_pipeline_completes_with_dft_ranking()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `test_stopping_rules_never_report_budget_or_starvation_as_convergence()` --uses--> `StopReason`  [INFERRED]
  tests/test_milestone_c.py → src/qumof/contract.py
- `failing()` --calls--> `make_record()`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/contract.py
- `Agents make judgement calls only (schema-validated)` --semantically_similar_to--> `Agent policy boundaries table`  [INFERRED] [semantically similar]
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

## Communities (93 total, 19 thin omitted)

### Community 1 - "agents/datasets.py"
Cohesion: 0.18
Nodes (9): candidate_descriptors(), _elements_from_formula(), gather_datasets(), match_score(), project_descriptors(), ReferenceDataset, _sha256(), _text() (+1 more)

### Community 2 - "PipelineError"
Cohesion: 0.08
Nodes (25): check_feature_symmetry(), PipelineError, SyntheticFixtureBackend, generate_seed_decorations(), take(), build_framework(), canonical_bits(), check_candidate_file() (+17 more)

### Community 3 - "scheme.py"
Cohesion: 0.17
Nodes (9): _models_for(), _row(), scripted_a1(), scripted_a2(), scripted_a4(), scripted_a67(), scripted_policies(), _allowed_verdicts() (+1 more)

### Community 4 - "Milestone C/DFT Model Tests"
Cohesion: 0.09
Nodes (19): load_artifacts(), c_run(), _state(), test_acquisition_is_seeded_and_favours_the_undersampled_uncertain_topology(), test_reference_competition_never_certifies_with_missing_references(), test_refinement_acquires_only_unlabelled_orbits_with_reasons(), test_relaxed_geometry_equivalence_uses_structure_not_energy(), test_rerun_and_interrupted_refinement_reuse_every_dft_job() (+11 more)

### Community 5 - "dft.py"
Cohesion: 0.16
Nodes (8): _carts(), difference_convergence_study(), evaluate_geometry(), formula_units(), PeriodicDFTBackend, failed(), protocol_fingerprint(), stress_tolerance_kbar()

### Community 6 - "QUBO Encoding & Pipeline Diagram"
Cohesion: 0.11
Nodes (17): _ancilla_coefficients(), compile_encoding(), compile_one_hot(), count_constraints(), count_penalty(), decode_one_hot(), degree(), _IntPoly (+9 more)

### Community 7 - "Periodic DFT Backend"
Cohesion: 0.11
Nodes (4): _kmesh(), PySCFAdapter, QuantumEspressoAdapter, _cart_to_frac()

### Community 8 - "make_record"
Cohesion: 0.10
Nodes (11): deduplicate_candidates(), JobState, StageStatus, StopReason, electronic_stage_status(), table_from_result(), evaluate_reference_mixtures(), evaluate_reference_mixtures() (+3 more)

### Community 9 - "screening.py"
Cohesion: 0.22
Nodes (4): MLPotentialBackend, _resolve(), _mixing(), screen()

### Community 10 - "QAOA & QPU Solvers"
Cohesion: 0.08
Nodes (24): predict(), bit_string(), complete_assignment(), evaluate_encoding(), one_hot_states(), rec(), physical_polynomial(), branch_and_bound() (+16 more)

### Community 11 - "PySCF Worker"
Cohesion: 0.11
Nodes (21): basis_and_pseudo_hashes(), build_cell(), _dispersion_model(), Evaluator, _host(), _initial_guess(), main(), parse_dispersion() (+13 more)

### Community 12 - "No-Agent Fixture Core"
Cohesion: 0.18
Nodes (25): bit_string(), canonical(), check_energy_compatibility(), compile_pair_qubo(), correction(), evaluate_qubo(), feasible_states(), features() (+17 more)

### Community 13 - "Toy Framework Test Helpers"
Cohesion: 0.12
Nodes (16): base_spec(), formate_cif(), pyscf_dft_protocol(), test_milestone_c_spec_errors_block_at_intake(), test_round_cap_before_stability_is_budget_exhausted_not_converged(), scheme_project(), test_every_scheme_box_runs_and_leaves_evidence(), test_scripted_run_uses_one_request_per_role_call_and_records_it() (+8 more)

### Community 14 - "Electronic Structure Solvers"
Cohesion: 0.09
Nodes (27): problem_from_artifact(), compute(), main(), _scf(), _apply(), exact_diagonalization(), hamiltonian_matrix(), _np() (+19 more)

### Community 15 - "test_agents.py"
Cohesion: 0.27
Nodes (16): a1(), a2(), a67(), controls(), run_agents(), test_a1_selects_topologies_from_the_brief_and_the_pipeline_analyses_only_those(), test_a2_validation_rejects_dropped_triplets_and_policy_changes(), test_agent_plan_requires_the_agent_policy() (+8 more)

### Community 16 - "packets.py"
Cohesion: 0.07
Nodes (28): build_a1_packet(), build_a2_packet(), build_a4_packet(), build_a67_packet(), candidate_quality(), candidate_rows(), compilation_options(), _composition_feasible() (+20 more)

### Community 17 - "Physical Intake Validation Tests"
Cohesion: 0.12
Nodes (24): validate_project(), test_fixture_project_validates(), test_pipeline_quantum_benchmark_with_quadratization(), codes(), test_cif_parse_expands_symmetry_and_keeps_provenance(), test_construction_failure_is_reported_never_an_energy(), test_invalid_connector_declaration_caught(), test_invalid_structural_inputs_caught_before_any_calculation() (+16 more)

### Community 18 - "contract.py"
Cohesion: 0.08
Nodes (22): names_for_token(), assign_folds(), candidate_models(), evaluate_holdout(), expand_tokens(), feature_polynomial(), feature_value(), feature_vector() (+14 more)

### Community 19 - "project_spec.py"
Cohesion: 0.05
Nodes (40): _apply(), build_catalogue(), cluster_lookup(), cluster_polynomial(), cluster_value(), _frac_to_cart(), _ikey(), _norm() (+32 more)

### Community 20 - "Hamiltonian Fitting & Refinement"
Cohesion: 0.13
Nodes (12): check_energy_compatibility(), check_no_holdout(), check_snapshot_against_split(), freeze_split(), ingest_labels(), merge_snapshots(), normalize_cell_energy(), _diagnose() (+4 more)

### Community 21 - "Framework Slot Lattice"
Cohesion: 0.13
Nodes (16): build_framework(), build_slot_lattice(), _centroid(), expand_supercell(), formula_counts(), _frac_close(), _fraction(), geometry_hashes() (+8 more)

### Community 23 - "design.py"
Cohesion: 0.14
Nodes (20): _bits(), build_packet(), compile_design(), evaluate_polynomial(), feasible_states(), _fmt(), kang_spectrum(), _mean() (+12 more)

### Community 24 - "Cluster Embedding Correction"
Cohesion: 0.14
Nodes (10): make_record(), assemble_corrected_energy(), _blocked(), ClusterBackend, correct_pool(), _molecule_structure(), plan_regions(), run_embedding_benchmark() (+2 more)

### Community 25 - "StageOutcome"
Cohesion: 0.13
Nodes (4): select_pool(), hamiltonian_from_selection(), StageOutcome, validate_structures()

### Community 26 - "Intake Contract Tests"
Cohesion: 0.14
Nodes (20): codes(), _edit_topologies(), test_cif_input_mode_unsupported(), test_duplicate_label_rejected(), test_empty_energy_set_rejected(), test_graph_relabelled_as_physical_net_rejected(), test_incompatible_energy_records_rejected(), test_ingest_rejects_corrupted_labels() (+12 more)

### Community 27 - "content_hash"
Cohesion: 0.22
Nodes (7): integral_hash(), prepare_active_space(), read_fcidump(), _require(), content_hash(), freeze_physical_split(), test_electronic_solvers_agree_on_identical_tiny_hamiltonian()

### Community 28 - "load_project"
Cohesion: 0.09
Nodes (22): agent_request_ceilings(), _case_from_fidelity(), _deep_merge(), learner_path(), load_project(), ProjectSpec, _read_json(), _read_jsonl() (+14 more)

### Community 29 - "Agent Output Validation"
Cohesion: 0.18
Nodes (14): _check_model_rows(), _coverage(), _error_state(), _ok_without_errors(), _record_line(), render_assessment(), number(), ref() (+6 more)

### Community 30 - "run_pipeline"
Cohesion: 0.09
Nodes (19): run_pipeline(), runs(), toy_run(), test_validated_correction_feeds_the_ranking_and_a_constant_correction_changes_nothing(), unvalidated(), _state(), test_budget_is_enforced_before_submission(), test_build_failure_in_pool_makes_ranking_incomplete() (+11 more)

### Community 31 - "Ground State Evaluation Stage"
Cohesion: 0.18
Nodes (16): New QuMOF Pipeline Diagram, Agent A1: MOF Topology Selector, Agent A2: QUBO Hamiltonian Constructor, Agent A3: Physical Correctness Checker, Agent A4: QUBO Hamiltonian Adjuster, Classical DFT, Confirmation Stage, Ground State Evaluation Stage (+8 more)

### Community 32 - "pormake_worker.py"
Cohesion: 0.29
Nodes (5): _candidate_nets(), main(), _quiet(), run(), _substituent_rule()

### Community 33 - "hashlib"
Cohesion: 0.36
Nodes (4): main(), _orb(), _relax(), _sha256()

### Community 34 - "runner.py"
Cohesion: 0.12
Nodes (11): AgentCallError, Cache, cache_key(), call_role(), check_schema(), Ledger, _ask(), build_graph() (+3 more)

### Community 35 - "Synthetic no-agent MOF fixture"
Cohesion: 0.36
Nodes (7): Orbit canonicalization, dedup and cross-graph pooling, Correction modes (none, constant, topology_dependent), Synthetic no-agent MOF fixture, Fixture data files (topologies, candidates, model_candidates, splits, literature_catalog), Synthetic ground-truth energy formula, prism6 (hexagonal prism graph), ring12 (12-site cycle graph)

### Community 36 - "acquisition.py"
Cohesion: 0.18
Nodes (9): acquisition_model(), _allocate(), bits_of(), _distance(), _normalise(), policy_errors(), _scores(), select_evaluation_batch() (+1 more)

### Community 37 - "PySCF Backend Tests"
Cohesion: 0.27
Nodes (12): evaluate(), run(), settings(), test_forces_and_stress_match_finite_differences(), energy_eV(), test_kpoint_mesh_equals_replicated_cell_at_folded_mesh(), test_relax_reaches_the_declared_force_tolerance(), test_scf_failure_is_reported_without_energy() (+4 more)

### Community 38 - "report.py"
Cohesion: 0.24
Nodes (9): _agent_section(), build_report(), _embedding_section(), _md_table(), not_executed(), _physical_section(), _screening_section(), _topology_section() (+1 more)

### Community 39 - "Encoding/Solver Tests & Conftest"
Cohesion: 0.19
Nodes (10): fixture_core(), harness_json(), cubic(), _hamiltonians(), pairwise(), test_cubic_model_rejected_by_qubo_only_target_but_retained_as_hubo(), test_exact_enumeration_matches_known_minima(), test_qubo_matches_fixture_reference_and_identity() (+2 more)

### Community 40 - "cif.py"
Cohesion: 0.06
Nodes (24): _accept(), _clean(), gather_evidence(), LocalPapers, _paper_source(), _parse_tool_result(), query_templates(), references_from() (+16 more)

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
Cohesion: 0.13
Nodes (16): copy_fixture(), read_jsonl(), test_holdout_label_smuggled_into_training_halts_run(), test_failed_evaluator_job_never_becomes_energy(), test_assembly_blocks_missing_terms_incomplete_coverage_foreign_geometry_and_overlap(), code(), spec(), test_decoration_space_and_orbit_quotient() (+8 more)

### Community 46 - "run_one"
Cohesion: 0.24
Nodes (5): OpenRouterClient, assess(), fake_device(), work(), run_one()

### Community 47 - "Controls: Literature Config"
Cohesion: 0.15
Nodes (13): literature, enabled, extra_queries, local_papers_dir, max_passage_chars, max_passages, max_sources, references (+5 more)

### Community 48 - "sys"
Cohesion: 0.28
Nodes (3): main(), main(), namelist_value()

### Community 49 - "Topology Builders"
Cohesion: 0.23
Nodes (6): lattice_info_for_builder(), choose_supercell(), _decoration_check(), generate_topologies(), protocol_errors(), _resolve_python()

### Community 50 - "Controls: OpenRouter Config"
Cohesion: 0.17
Nodes (12): openrouter, api_key, app_title, app_url, base_url, deadline_s, model, provider (+4 more)

### Community 51 - "Quadratization Tests"
Cohesion: 0.29
Nodes (7): _hamiltonians(), test_branch_and_bound_agrees_and_reports_honest_gaps(), test_penalty_bound_sublattice_counts_and_one_hot(), test_published_h2_benchmark_is_reproduced(), test_qaoa_benchmark_agrees_with_exact_and_records_provenance(), test_qaoa_mixers_preserve_constraints_and_bit_order_errors_are_caught(), test_quadratized_cubic_model_reproduces_feasible_cost()

### Community 53 - "run_muf7_full.py"
Cohesion: 0.15
Nodes (8): Builder, cluster_vqe_sqd(), log(), main(), score(), Relaxer, spearman(), zn4o_cluster()

### Community 54 - "Controls: Assessment & Cache"
Cohesion: 0.18
Nodes (10): assessment, required_checks, top_k_candidates, cache, dir, enabled, orchestration, engine (+2 more)

### Community 55 - "validation.py"
Cohesion: 0.11
Nodes (13): write_cif(), bond_graph(), _components(), deconstruct(), map_to_parent_slots(), min_interatomic_distance(), _relaxation_record(), _lengths_angles() (+5 more)

### Community 56 - "json"
Cohesion: 0.14
Nodes (16): check_run(), _close(), fetch(), load_materials(), _acceptance(), _agent_metrics(), evaluate(), render() (+8 more)

### Community 57 - "Refinement & Gateway Tests"
Cohesion: 0.19
Nodes (13): review_proposal(), decide(), reject(), _al(), _proposal(), _refinement(), _small_training_fixture(), test_active_learning_recovers_cubic_model_from_sparse_start() (+5 more)

### Community 58 - "pathlib"
Cohesion: 0.32
Nodes (3): close(), expect_error(), require()

### Community 60 - "Kang et al. design benchmark (agents-design-bench)"
Cohesion: 0.31
Nodes (7): kang_control (paper weighting in term catalogue), Kang, Kim & Kim 2025: Quantum Computing Based Design of Multivariate Porous Materials, Static provenance report (live literature NOT_RUN), Agent A2 (Hamiltonian model design), Cu-THQ-HHTP, Kang et al. design benchmark (agents-design-bench), Py-MV-DBA-COF

### Community 61 - "test_milestone_f.py"
Cohesion: 0.24
Nodes (7): test_aiida_engine_reproduces_the_local_engine(), test_ml_screening_deprioritises_only_calibrated_gaps_and_narrows_the_run(), test_qaoa_on_fake_brisbane_matches_the_simulator_and_reports_noise(), test_store_rejects_a_concurrent_writer(), test_uncalibrated_or_failed_screening_keeps_every_topology(), _toy(), _venv_has()

### Community 62 - "CLAUDE.md"
Cohesion: 0.29
Nodes (5): 1. Think Before Coding, 2. Simplicity First, 3. Surgical Changes, 4. Goal-Driven Execution, graphify

### Community 63 - "Fixture Model Ladder M0-M2"
Cohesion: 0.16
Nodes (9): Classical exact fixed-composition baseline (924 states), MODEL_INADEQUATE error, UNSUPPORTED_HIGHER_ORDER_WITHOUT_QUADRATIZATION, core_pairwise case, higher_order case, Model M0 (constant + unlike NN pairs), Model M1 (M0 + distance-two pairs), Model M2 (M1 + all-B path triples, cubic) (+1 more)

### Community 64 - "Solvers & Deterministic Mode"
Cohesion: 0.13
Nodes (12): Fixture acceptance criteria, finite_substitution_interaction_graph input mode, Fixture integration instructions for coding agent, Composition-preserving QAOA, Exact enumeration (certified minima), Qiskit FakeBrisbane noisy device, Limitations, MUF-7 (+4 more)

### Community 65 - "controls.py"
Cohesion: 0.14
Nodes (6): Controls, load_controls(), _merge(), normal_requests(), _redact(), test_controls_use_environment_secrets_and_never_expose_them()

### Community 66 - "cut_region"
Cohesion: 0.19
Nodes (10): cut_region(), add(), position(), _close_pairs(), frac_to_cart(), _match(), _min_image_distance(), _norm() (+2 more)

### Community 67 - "Controls: Material Fields"
Cohesion: 0.25
Nodes (8): doi, formula, metals, mofid, name, record_id, topology, columns

### Community 68 - "DFT-fitted QUBO Hamiltonian (step 3)"
Cohesion: 0.10
Nodes (21): BDC / 2-amino-BDC linkers (1:1), Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A), MOF-5 / IRMOF-1 (Zn4O nodes), Physical case recipe: MOF-5 BDC/amino-BDC, Agent A1 (topology selection), AiiDA workflow engine, CASCI, CCSD (+13 more)

### Community 73 - "BuildFailure"
Cohesion: 0.18
Nodes (3): BuildFailure, ParentSubstitutionBuilder, PormakeBuilder

### Community 75 - "Controls: MCP Valency"
Cohesion: 0.33
Nodes (6): mcp, valency, api_token, enabled, timeout_s, url

### Community 76 - "scheme_trace"
Cohesion: 0.33
Nodes (3): _load(), scheme_trace(), write_scheme_trace()

### Community 78 - "mock_mlip.py"
Cohesion: 0.60
Nodes (3): energy(), main(), mirror_pw()

### Community 81 - "dft.py"
Cohesion: 0.48
Nodes (3): sha(), spec_dict(), write_mof5_scheme_project()

### Community 82 - "test_reference_datasets_match_by_code_and_feed_direct_comparisons"
Cohesion: 0.50
Nodes (4): _a67_packet(), gather_datasets_for_fixture_is_not_applicable(), test_a67_cannot_upgrade_checks_or_cite_unsupplied_evidence(), test_reference_datasets_match_by_code_and_feed_direct_comparisons()

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
- **22 isolated node(s):** `qumof`, `Agent A1: MOF Topology Selector`, `Agent A3: Physical Correctness Checker`, `DeepSeek V4 Flash`, `DeepSeek V4 Pro` (+17 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 564 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **19 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `PipelineError` connect `PipelineError` to `Pipeline`, `Milestone C/DFT Model Tests`, `dft.py`, `QUBO Encoding & Pipeline Diagram`, `Periodic DFT Backend`, `make_record`, `screening.py`, `QAOA & QPU Solvers`, `Electronic Structure Solvers`, `packets.py`, `Physical Intake Validation Tests`, `contract.py`, `project_spec.py`, `Hamiltonian Fitting & Refinement`, `Framework Slot Lattice`, `RunStore`, `Cluster Embedding Correction`, `Intake Contract Tests`, `content_hash`, `load_project`, `run_pipeline`, `hashlib`, `runner.py`, `acquisition.py`, `Encoding/Solver Tests & Conftest`, `cif.py`, `Model & Symmetry Tests`, `Topology Builders`, `Quadratization Tests`, `validation.py`, `json`, `test_milestone_f.py`, `controls.py`, `cut_region`, `store.py`, `rank_candidates`, `aiida_engine.py`, `scheme_trace`?**
  _High betweenness centrality (0.195) - this node is a cross-community bridge._
- **Are the 25 inferred relationships involving `PipelineError` (e.g. with `SyntheticFixtureBackend` and `mixture_balance()`) actually correct?**
  _`PipelineError` has 25 INFERRED edges - model-reasoned connections that need verification._
- **What connects `qumof`, `Agent A1: MOF Topology Selector`, `Agent A3: Physical Correctness Checker` to the rest of the system?**
  _22 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `PipelineError` be split into smaller, more focused modules?**
  _Cohesion score 0.08470588235294117 - nodes in this community are weakly interconnected._
- **Why does `make_record()` connect `Cluster Embedding Correction` to `Pipeline`, `PipelineError`, `dft.py`, `QUBO Encoding & Pipeline Diagram`, `make_record`, `screening.py`, `QAOA & QPU Solvers`, `Electronic Structure Solvers`, `Physical Intake Validation Tests`, `contract.py`, `project_spec.py`, `Hamiltonian Fitting & Refinement`, `Framework Slot Lattice`, `RunStore`, `StageOutcome`, `content_hash`, `load_project`, `run_pipeline`, `runner.py`, `acquisition.py`, `report.py`, `validation.py`, `json`, `Refinement & Gateway Tests`, `.physical_spec`, `rank_candidates`, `._physical_screening`?**
  _High betweenness centrality (0.077) - this node is a cross-community bridge._
- **Should `Milestone C/DFT Model Tests` be split into smaller, more focused modules?**
  _Cohesion score 0.08620689655172414 - nodes in this community are weakly interconnected._

### Low-confidence Hints
_AMBIGUOUS edges — the extractor was unsure. Verify before acting on these._

- **What is the exact relationship between `refinement.py` and `Optimisation Feedback Loop`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._