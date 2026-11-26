# Graph Report - qumof  (2026-11-26)

## Corpus Check
- 119 files · ~118,946 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 26 file(s) not represented in the graph (top: .jsonl 10, (none) 7, .pyi 7)

## Summary
- 1772 nodes · 4652 edges · 87 communities (73 shown, 14 thin omitted)
- Extraction: 94% EXTRACTED · 6% INFERRED · 0% AMBIGUOUS · INFERRED: 264 edges (avg confidence: 0.89)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `90ab557f`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Pipeline
- refinement.py
- structures.py
- validate.py
- Milestone C/DFT Model Tests
- dft.py
- qaoa.py
- AgentRun
- make_record
- screening.py
- encoding.py
- pyscf_worker.py
- No-Agent Fixture Core
- Toy Framework Test Helpers
- sqd_simulation
- test_agents.py
- packets.py
- Physical Intake Validation Tests
- contract.py
- project_spec.py
- intake.py
- Framework Slot Lattice
- RunStore
- design.py
- Cluster Embedding Correction
- review_proposal
- Intake Contract Tests
- Physical case recipe: MOF-5 BDC/amino-BDC
- controls.py
- test_refinement_and_gateway.py
- load_project
- lint.yml
- pormake_worker.py
- run_one
- runner.py
- PipelineError
- math
- PySCF Backend Tests
- report.py
- Encoding/Solver Tests & Conftest
- cif.py
- Controls: Datasets Config
- MUF-7 LLM Benchmark Figure
- MofPipeWorkChain
- hashlib
- conftest.py
- contracts.py
- Controls: Literature Config
- literature.py
- topology_builders.py
- Controls: OpenRouter Config
- repos
- SequentialGraph
- pathlib
- Controls: Assessment & Cache
- validation.py
- __main__.py
- Fixture integration instructions for coding agent
- geometry_match.py
- fit_diagnostics
- Kang et al. design benchmark (agents-design-bench)
- sys
- CLAUDE.md
- Fixture Model Ladder M0-M2
- scheme_run
- mock_mlip.py
- cut_region
- Controls: Material Fields
- PormakeBuilder
- active_space.py
- run_embedding_benchmark
- Subtractive embedding at metal nodes
- LocalPapers
- Controls: MCP Valency
- qpu_worker.py
- Deterministic Hamiltonian selection
- aiida_engine.py
- Controls: Budget
- Controls: HF Source
- Controls: Agent Token Limits
- A3/A67 & MOF Databases
- Package Metadata
- Next Steps

## God Nodes (most connected - your core abstractions)
1. `PipelineError` - 172 edges
2. `make_record()` - 85 edges
3. `load_project()` - 82 edges
4. `StageStatus` - 60 edges
5. `Pipeline` - 51 edges
6. `content_hash()` - 49 edges
7. `run_pipeline()` - 48 edges
8. `RunStore` - 43 edges
9. `AgentRun` - 37 edges
10. `validate_project()` - 33 edges

## Surprising Connections (you probably didn't know these)
- `test_job_restart_reuses_successful_work()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `test_physical_pipeline_completes_with_dft_ranking()` --uses--> `RunStore`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/store.py
- `test_stopping_rules_never_report_budget_or_starvation_as_convergence()` --uses--> `StopReason`  [INFERRED]
  tests/test_milestone_c.py → src/qumof/contract.py
- `failing()` --calls--> `make_record()`  [INFERRED]
  tests/test_physical_dft_and_model.py → src/qumof/contract.py
- `MOF-5 / IRMOF-1 (Zn4O nodes)` --conceptually_related_to--> `MUF-7 full-scheme run (approximate)`  [INFERRED]
  mof_no_agent_fixture/physical_case/README.md → README.md

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

## Communities (87 total, 14 thin omitted)

### Community 0 - "Pipeline"
Cohesion: 0.09
Nodes (7): check_snapshot_against_split(), electronic_stage_status(), Backend, Pipeline, StageOutcome, ranking_order_changed(), validate_structures()

### Community 1 - "refinement.py"
Cohesion: 0.09
Nodes (16): acquisition_model(), _allocate(), bits_of(), _distance(), _normalise(), policy_errors(), _scores(), select_evaluation_batch() (+8 more)

### Community 2 - "structures.py"
Cohesion: 0.09
Nodes (15): deduplicate_candidates(), select_pool(), table_from_result(), build_framework(), canonical_bits(), check_candidate_file(), configuration_id(), decode_species() (+7 more)

### Community 3 - "validate.py"
Cohesion: 0.13
Nodes (19): _allowed_verdicts(), _check_model_rows(), _coverage(), _error_state(), _ok_without_errors(), _record_line(), render_assessment(), number() (+11 more)

### Community 4 - "Milestone C/DFT Model Tests"
Cohesion: 0.06
Nodes (23): load_artifacts(), _state(), test_acquisition_is_seeded_and_favours_the_undersampled_uncertain_topology(), test_reference_competition_never_certifies_with_missing_references(), test_refinement_acquires_only_unlabelled_orbits_with_reasons(), test_relaxed_geometry_equivalence_uses_structure_not_energy(), test_rerun_and_interrupted_refinement_reuse_every_dft_job(), test_stopping_rules_never_report_budget_or_starvation_as_convergence() (+15 more)

### Community 5 - "dft.py"
Cohesion: 0.06
Nodes (11): _carts(), difference_convergence_study(), evaluate_geometry(), formula_units(), _kmesh(), PeriodicDFTBackend, failed(), protocol_fingerprint() (+3 more)

### Community 6 - "qaoa.py"
Cohesion: 0.08
Nodes (22): bit_string(), one_hot_states(), rec(), branch_and_bound(), exact_enumeration(), quantum_solver_status(), simulated_annealing(), apply_mixer() (+14 more)

### Community 8 - "make_record"
Cohesion: 0.08
Nodes (14): JobState, make_record(), StageStatus, StopReason, check_energy_compatibility(), freeze_physical_split(), freeze_split(), verify_encoding() (+6 more)

### Community 9 - "screening.py"
Cohesion: 0.12
Nodes (9): feature_value(), MLPotentialBackend, _resolve(), calibrate(), _endpoint(), generate_seed_decorations(), _mixing(), _relaxation_record() (+1 more)

### Community 10 - "encoding.py"
Cohesion: 0.06
Nodes (36): New QuMOF Pipeline Diagram, Agent A1: MOF Topology Selector, Agent A2: QUBO Hamiltonian Constructor, Agent A3: Physical Correctness Checker, Agent A4: QUBO Hamiltonian Adjuster, Classical DFT, Confirmation Stage, Ground State Evaluation Stage (+28 more)

### Community 11 - "pyscf_worker.py"
Cohesion: 0.11
Nodes (21): basis_and_pseudo_hashes(), build_cell(), _dispersion_model(), Evaluator, _host(), _initial_guess(), main(), parse_dispersion() (+13 more)

### Community 12 - "No-Agent Fixture Core"
Cohesion: 0.13
Nodes (36): Fixture acceptance criteria, Fixture integration instructions for coding agent, Orbit canonicalization, dedup and cross-graph pooling, Correction modes (none, constant, topology_dependent), Synthetic no-agent MOF fixture, Synthetic ground-truth energy formula, prism6 (hexagonal prism graph), ring12 (12-site cycle graph) (+28 more)

### Community 13 - "Toy Framework Test Helpers"
Cohesion: 0.08
Nodes (27): base_spec(), formate_cif(), pyscf_dft_protocol(), write_pyscf_toy_project(), test_round_cap_before_stability_is_budget_exhausted_not_converged(), test_aiida_engine_reproduces_the_local_engine(), test_ml_screening_deprioritises_only_calibrated_gaps_and_narrows_the_run(), test_qaoa_on_fake_brisbane_matches_the_simulator_and_reports_noise() (+19 more)

### Community 14 - "sqd_simulation"
Cohesion: 0.13
Nodes (17): _apply(), exact_diagonalization(), hamiltonian_matrix(), _np(), _problem(), pyscf_casci(), _recover(), _result() (+9 more)

### Community 15 - "test_agents.py"
Cohesion: 0.06
Nodes (33): ReplayClient, candidate_descriptors(), _elements_from_formula(), gather_datasets(), _h5_array(), match_score(), project_descriptors(), ReferenceDataset (+25 more)

### Community 16 - "packets.py"
Cohesion: 0.12
Nodes (24): build_a1_packet(), build_a2_packet(), build_a4_packet(), build_a67_packet(), candidate_rows(), compilation_options(), _composition_feasible(), constraint_policy_id() (+16 more)

### Community 17 - "Physical Intake Validation Tests"
Cohesion: 0.15
Nodes (18): toy_backend(), codes(), test_cif_parse_expands_symmetry_and_keeps_provenance(), test_construction_failure_is_reported_never_an_energy(), test_invalid_connector_declaration_caught(), test_invalid_structural_inputs_caught_before_any_calculation(), test_known_parent_gives_checked_slot_lattice(), test_physical_policy_fields_block_with_field_path() (+10 more)

### Community 18 - "contract.py"
Cohesion: 0.08
Nodes (22): assign_folds(), candidate_models(), check_feature_symmetry(), evaluate_holdout(), expand_tokens(), feature_vector(), fit_and_select(), fit_and_select_grouped() (+14 more)

### Community 19 - "project_spec.py"
Cohesion: 0.06
Nodes (30): requested_cutoff(), _cluster_prefix(), is_known_feature(), is_transferable(), dft_protocol_errors(), tolerance_errors(), protocol_errors(), agent_request_ceilings() (+22 more)

### Community 20 - "intake.py"
Cohesion: 0.12
Nodes (12): _case_from_fidelity(), _deep_merge(), learner_path(), _read_json(), _read_jsonl(), _hamiltonians(), test_branch_and_bound_agrees_and_reports_honest_gaps(), test_penalty_bound_sublattice_counts_and_one_hot() (+4 more)

### Community 21 - "Framework Slot Lattice"
Cohesion: 0.12
Nodes (15): build_slot_lattice(), _centroid(), _components(), deconstruct(), expand_supercell(), formula_counts(), _frac_close(), _fraction() (+7 more)

### Community 22 - "RunStore"
Cohesion: 0.06
Nodes (14): _agent_metrics(), _load(), _models_for(), _row(), scheme_trace(), scripted_a1(), scripted_a2(), scripted_a4() (+6 more)

### Community 23 - "design.py"
Cohesion: 0.13
Nodes (24): assess(), _bits(), build_packet(), compile_design(), evaluate_polynomial(), feasible_states(), _fmt(), kang_spectrum() (+16 more)

### Community 24 - "Cluster Embedding Correction"
Cohesion: 0.18
Nodes (7): assemble_corrected_energy(), _blocked(), ClusterBackend, correct_pool(), plan_regions(), _structure(), validate_scheme()

### Community 25 - "review_proposal"
Cohesion: 0.18
Nodes (7): review_proposal(), decide(), reject(), _proposal(), test_malformed_proposal(), test_replayed_proposals_are_validated_and_never_executed(), test_valid_proposal_is_accepted_but_not_executed_when_agents_enabled()

### Community 26 - "Intake Contract Tests"
Cohesion: 0.14
Nodes (19): codes(), _edit_topologies(), test_cif_input_mode_unsupported(), test_duplicate_label_rejected(), test_empty_energy_set_rejected(), test_graph_relabelled_as_physical_net_rejected(), test_incompatible_energy_records_rejected(), test_ingest_rejects_corrupted_labels() (+11 more)

### Community 27 - "Physical case recipe: MOF-5 BDC/amino-BDC"
Cohesion: 0.20
Nodes (9): BDC / 2-amino-BDC linkers (1:1), Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A), MOF-5 / IRMOF-1 (Zn4O nodes), Physical case recipe: MOF-5 BDC/amino-BDC, Agent A1 (topology selection), ML-potential screening (orb-v3 + D3BJ), Multivariate MOFs (MTV-MOFs), QuMOF pipeline (+1 more)

### Community 28 - "controls.py"
Cohesion: 0.14
Nodes (6): Controls, load_controls(), _merge(), normal_requests(), _redact(), test_controls_use_environment_secrets_and_never_expose_them()

### Community 29 - "test_refinement_and_gateway.py"
Cohesion: 0.40
Nodes (7): _al(), pipeline(), _refinement(), _small_training_fixture(), test_active_learning_recovers_cubic_model_from_sparse_start(), test_budget_exhaustion_is_not_convergence(), test_more_labels_cannot_fix_missing_interaction_term()

### Community 30 - "load_project"
Cohesion: 0.08
Nodes (37): load_project(), validate_project(), run_pipeline(), copy_fixture(), runs(), toy_run(), test_agent_plan_requires_the_agent_policy(), test_fixture_project_validates() (+29 more)

### Community 31 - "lint.yml"
Cohesion: 0.22
Nodes (8): jobs, lint, runs-on, steps, name, on, run, uses

### Community 32 - "pormake_worker.py"
Cohesion: 0.19
Nodes (9): main(), _orb(), _relax(), _sha256(), _candidate_nets(), main(), _quiet(), run() (+1 more)

### Community 33 - "run_one"
Cohesion: 0.22
Nodes (4): OpenRouterClient, fake_device(), work(), run_one()

### Community 34 - "runner.py"
Cohesion: 0.13
Nodes (9): AgentCallError, Cache, cache_key(), call_role(), check_schema(), Ledger, _ask(), canonical_json() (+1 more)

### Community 35 - "PipelineError"
Cohesion: 0.09
Nodes (12): names_for_token(), content_hash(), PipelineError, check_no_holdout(), ingest_labels(), normalize_cell_energy(), SyntheticFixtureBackend, build_framework() (+4 more)

### Community 36 - "math"
Cohesion: 0.17
Nodes (14): _apply(), build_catalogue(), cluster_lookup(), cluster_polynomial(), cluster_value(), _frac_to_cart(), _ikey(), _norm() (+6 more)

### Community 37 - "PySCF Backend Tests"
Cohesion: 0.25
Nodes (13): evaluate(), run(), settings(), test_engine_identity_is_part_of_the_fidelity(), test_forces_and_stress_match_finite_differences(), energy_eV(), test_kpoint_mesh_equals_replicated_cell_at_folded_mesh(), test_relax_reaches_the_declared_force_tolerance() (+5 more)

### Community 38 - "report.py"
Cohesion: 0.20
Nodes (9): _agent_section(), build_report(), _embedding_section(), _md_table(), not_executed(), _physical_section(), _screening_section(), _topology_section() (+1 more)

### Community 39 - "Encoding/Solver Tests & Conftest"
Cohesion: 0.19
Nodes (10): fixture_core(), harness_json(), cubic(), _hamiltonians(), pairwise(), test_cubic_model_rejected_by_qubo_only_target_but_retained_as_hubo(), test_exact_enumeration_matches_known_minima(), test_qubo_matches_fixture_reference_and_identity() (+2 more)

### Community 40 - "cif.py"
Cohesion: 0.13
Nodes (14): apply_symop(), cell_matrix(), cif_number(), _frac_distance(), _leading(), Loop, _loop_with(), parse_cif() (+6 more)

### Community 41 - "Controls: Datasets Config"
Cohesion: 0.13
Nodes (15): datasets, enabled, format, hdf5, id, index, kind, license (+7 more)

### Community 42 - "MUF-7 LLM Benchmark Figure"
Cohesion: 0.20
Nodes (15): MUF-7 LLM Benchmark Figure, A1: QUBO Hamiltonian Construction (NMAE), A2: QAOA QUBO Solution (correct output probability), A2: QAOA Raw Energy Prediction (MAE), A3: VQE Final Structure Prediction, DeepSeek V4 Flash, DeepSeek V4 Pro, Kang's [1] MUF-7 QUBO (+7 more)

### Community 44 - "hashlib"
Cohesion: 0.48
Nodes (3): sha(), spec_dict(), write_mof5_scheme_project()

### Community 45 - "conftest.py"
Cohesion: 0.17
Nodes (12): take(), read_jsonl(), spec(), test_decoration_space_and_orbit_quotient(), test_feature_polynomials_match_counts(), test_feature_symmetry_and_swap_reachability(), test_inadequate_family_halts_with_model_inadequate(), test_model_selection_and_untouched_holdout() (+4 more)

### Community 47 - "Controls: Literature Config"
Cohesion: 0.15
Nodes (13): literature, enabled, extra_queries, local_papers_dir, max_passage_chars, max_passages, max_sources, references (+5 more)

### Community 48 - "literature.py"
Cohesion: 0.15
Nodes (11): _accept(), _clean(), gather_evidence(), _paper_source(), _parse_tool_result(), query_templates(), references_from(), _resolve_calls() (+3 more)

### Community 49 - "topology_builders.py"
Cohesion: 0.11
Nodes (9): BuildFailure, _cart_to_frac(), lattice_info_for_builder(), ParentSubstitutionBuilder, choose_supercell(), _decoration_check(), generate_topologies(), protocol_errors() (+1 more)

### Community 50 - "Controls: OpenRouter Config"
Cohesion: 0.17
Nodes (12): openrouter, api_key, app_title, app_url, base_url, deadline_s, model, provider (+4 more)

### Community 51 - "repos"
Cohesion: 0.29
Nodes (6): args, id, repos, hooks, repo, rev

### Community 53 - "pathlib"
Cohesion: 0.09
Nodes (8): Builder, cluster_vqe_sqd(), log(), main(), score(), Relaxer, spearman(), zn4o_cluster()

### Community 54 - "Controls: Assessment & Cache"
Cohesion: 0.18
Nodes (10): assessment, required_checks, top_k_candidates, cache, dir, enabled, orchestration, engine (+2 more)

### Community 55 - "validation.py"
Cohesion: 0.14
Nodes (10): write_cif(), bond_graph(), map_to_parent_slots(), min_interatomic_distance(), _lengths_angles(), metal_coordination(), mofchecker_check(), _structure() (+2 more)

### Community 56 - "__main__.py"
Cohesion: 0.13
Nodes (14): check_run(), _close(), fetch(), load_materials(), _acceptance(), evaluate(), render(), check_connections() (+6 more)

### Community 57 - "Fixture integration instructions for coding agent"
Cohesion: 0.17
Nodes (10): finite_substitution_interaction_graph input mode, Composition-preserving QAOA, Exact enumeration (certified minima), Qiskit FakeBrisbane noisy device, Limitations, MUF-7, OpenRouter, project.json / project_spec.template.json (+2 more)

### Community 58 - "geometry_match.py"
Cohesion: 0.18
Nodes (8): _apply(), equivalence_classes(), equivalent(), close(), fingerprint(), _frac_to_cart(), _lattice_params(), supercell_operations()

### Community 59 - "fit_diagnostics"
Cohesion: 0.29
Nodes (4): candidate_quality(), fit_diagnostics(), _spearman(), spearman()

### Community 60 - "Kang et al. design benchmark (agents-design-bench)"
Cohesion: 0.27
Nodes (8): kang_control (paper weighting in term catalogue), Kang, Kim & Kim 2025: Quantum Computing Based Design of Multivariate Porous Materials, Static provenance report (live literature NOT_RUN), Fixture data files (topologies, candidates, model_candidates, splits, literature_catalog), Agent A2 (Hamiltonian model design), Cu-THQ-HHTP, Kang et al. design benchmark (agents-design-bench), Py-MV-DBA-COF

### Community 61 - "sys"
Cohesion: 0.28
Nodes (3): main(), main(), namelist_value()

### Community 62 - "CLAUDE.md"
Cohesion: 0.25
Nodes (6): 1. Think Before Coding, 2. Simplicity First, 3. Surgical Changes, 4. Goal-Driven Execution, graphify, Linting & formatting (ruff)

### Community 63 - "Fixture Model Ladder M0-M2"
Cohesion: 0.28
Nodes (7): Classical exact fixed-composition baseline (924 states), UNSUPPORTED_HIGHER_ORDER_WITHOUT_QUADRATIZATION, core_pairwise case, higher_order case, Model M0 (constant + unlike NN pairs), Model M1 (M0 + distance-two pairs), Model M2 (M1 + all-B path triples, cubic)

### Community 65 - "mock_mlip.py"
Cohesion: 0.47
Nodes (3): energy(), main(), mirror_pw()

### Community 66 - "cut_region"
Cohesion: 0.19
Nodes (10): cut_region(), add(), position(), _close_pairs(), frac_to_cart(), _match(), _min_image_distance(), _norm() (+2 more)

### Community 67 - "Controls: Material Fields"
Cohesion: 0.25
Nodes (8): doi, formula, metals, mofid, name, record_id, topology, columns

### Community 70 - "active_space.py"
Cohesion: 0.19
Nodes (6): integral_hash(), prepare_active_space(), problem_from_artifact(), read_fcidump(), _require(), test_electronic_solvers_agree_on_identical_tiny_hamiltonian()

### Community 71 - "run_embedding_benchmark"
Cohesion: 0.21
Nodes (6): compute(), main(), _scf(), _molecule_structure(), run_embedding_benchmark(), energy()

### Community 72 - "Subtractive embedding at metal nodes"
Cohesion: 0.25
Nodes (9): CASCI, CCSD, H2 STO-3G electronic benchmark (Szabo & Ostlund), Keto/enol HF-to-CCSD embedding benchmark, Periodic DFT ranking (step 5), PySCF, SQD (sample-based quantum diagonalization), Toy frameworks with mock DFT (+1 more)

### Community 75 - "Controls: MCP Valency"
Cohesion: 0.33
Nodes (6): mcp, valency, api_token, enabled, timeout_s, url

### Community 77 - "qpu_worker.py"
Cohesion: 0.48
Nodes (5): _device(), dicke(), main(), qaoa_circuit(), _scs()

### Community 81 - "aiida_engine.py"
Cohesion: 0.20
Nodes (4): AiiDA workflow engine, Optional extras (agents, mlip, topology, qpu, aiida, gpu), PORMAKE, load_aiida()

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
- **22 isolated node(s):** `qumof`, `BDC / 2-amino-BDC linkers (1:1)`, `Agent A1 (topology selection)`, `Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A)`, `Agent A1: MOF Topology Selector` (+17 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 634 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **14 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `PipelineError` connect `PipelineError` to `Pipeline`, `refinement.py`, `structures.py`, `Milestone C/DFT Model Tests`, `dft.py`, `qaoa.py`, `make_record`, `screening.py`, `encoding.py`, `Toy Framework Test Helpers`, `sqd_simulation`, `packets.py`, `Physical Intake Validation Tests`, `contract.py`, `project_spec.py`, `intake.py`, `Framework Slot Lattice`, `RunStore`, `Cluster Embedding Correction`, `Intake Contract Tests`, `controls.py`, `load_project`, `runner.py`, `math`, `Encoding/Solver Tests & Conftest`, `cif.py`, `topology_builders.py`, `SequentialGraph`, `pathlib`, `validation.py`, `__main__.py`, `cut_region`, `active_space.py`, `run_embedding_benchmark`, `aiida_engine.py`?**
  _High betweenness centrality (0.168) - this node is a cross-community bridge._
- **Are the 40 inferred relationships involving `PipelineError` (e.g. with `SequentialGraph` and `compute()`) actually correct?**
  _`PipelineError` has 40 INFERRED edges - model-reasoned connections that need verification._
- **What connects `qumof`, `BDC / 2-amino-BDC linkers (1:1)`, `Agent A1 (topology selection)` to the rest of the system?**
  _22 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Pipeline` be split into smaller, more focused modules?**
  _Cohesion score 0.08865248226950355 - nodes in this community are weakly interconnected._
- **Why does `make_record()` connect `make_record` to `Pipeline`, `refinement.py`, `structures.py`, `dft.py`, `qaoa.py`, `screening.py`, `encoding.py`, `Toy Framework Test Helpers`, `sqd_simulation`, `packets.py`, `contract.py`, `project_spec.py`, `intake.py`, `Framework Slot Lattice`, `RunStore`, `Cluster Embedding Correction`, `review_proposal`, `load_project`, `runner.py`, `PipelineError`, `report.py`, `validation.py`, `active_space.py`, `run_embedding_benchmark`?**
  _High betweenness centrality (0.060) - this node is a cross-community bridge._
- **Are the 5 inferred relationships involving `load_project()` (e.g. with `gather_datasets_for_fixture_is_not_applicable()` and `test_a2_validation_rejects_dropped_triplets_and_policy_changes()`) actually correct?**
  _`load_project()` has 5 INFERRED edges - model-reasoned connections that need verification._

### Low-confidence Hints
_AMBIGUOUS edges — the extractor was unsure. Verify before acting on these._

- **What is the exact relationship between `refinement.py` and `Optimisation Feedback Loop`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._