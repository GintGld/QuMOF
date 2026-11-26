# Graph Report - qumof  (2026-11-26)

## Corpus Check
- 115 files · ~118,866 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 19 file(s) not represented in the graph (top: .jsonl 10, (none) 7, .xyz 1)

## Summary
- 1750 nodes · 4643 edges · 93 communities (76 shown, 17 thin omitted)
- Extraction: 94% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 255 edges (avg confidence: 0.89)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `aa497516`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Pipeline
- transfer.py
- structures.py
- agents/datasets.py
- Milestone C/DFT Model Tests
- dft.py
- optimization.py
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
- StageOutcome
- Intake Contract Tests
- Physical case recipe: MOF-5 BDC/amino-BDC
- controls.py
- test_refinement_and_gateway.py
- load_project
- Ground State Evaluation Stage
- pormake_worker.py
- scheme.py
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
- Synthetic no-agent MOF fixture
- conftest.py
- OpenRouterClient
- Controls: Literature Config
- literature.py
- topology_builders.py
- Controls: OpenRouter Config
- Quadratization Tests
- SequentialGraph
- run_muf7_full.py
- Controls: Assessment & Cache
- validation.py
- __main__.py
- Fixture integration instructions for coding agent
- geometry_match.py
- .physical_spec
- Kang et al. design benchmark (agents-design-bench)
- json
- CLAUDE.md
- Fixture Model Ladder M0-M2
- scheme_run
- store.py
- cut_region
- Controls: Material Fields
- test_design_bench.py
- .__call__
- active_space.py
- run_embedding_benchmark
- Subtractive embedding at metal nodes
- DFT-fitted QUBO Hamiltonian (step 3)
- LocalPapers
- Controls: MCP Valency
- electronic_solvers.py
- qpu_worker.py
- Deterministic Hamiltonian selection
- ValencyMCP
- main
- pathlib
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
4. `StageStatus` - 61 edges
5. `Pipeline` - 51 edges
6. `content_hash()` - 49 edges
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

## Communities (93 total, 17 thin omitted)

### Community 1 - "transfer.py"
Cohesion: 0.14
Nodes (12): deduplicate_candidates(), bit_string(), simulated_annealing(), canonical_bits(), orbit_id(), is_replica(), _key(), native_states() (+4 more)

### Community 2 - "structures.py"
Cohesion: 0.11
Nodes (14): check_feature_symmetry(), calibrate(), _endpoint(), generate_seed_decorations(), take(), build_framework(), decode_species(), define_decoration_space() (+6 more)

### Community 3 - "agents/datasets.py"
Cohesion: 0.13
Nodes (11): candidate_descriptors(), _elements_from_formula(), fetch(), gather_datasets(), _h5_array(), match_score(), project_descriptors(), ReferenceDataset (+3 more)

### Community 4 - "Milestone C/DFT Model Tests"
Cohesion: 0.06
Nodes (26): load_artifacts(), _state(), test_acquisition_is_seeded_and_favours_the_undersampled_uncertain_topology(), test_reference_competition_never_certifies_with_missing_references(), test_refinement_acquires_only_unlabelled_orbits_with_reasons(), test_relaxed_geometry_equivalence_uses_structure_not_energy(), test_rerun_and_interrupted_refinement_reuse_every_dft_job(), test_round_cap_before_stability_is_budget_exhausted_not_converged() (+18 more)

### Community 5 - "dft.py"
Cohesion: 0.06
Nodes (11): _carts(), difference_convergence_study(), evaluate_geometry(), formula_units(), _kmesh(), PeriodicDFTBackend, failed(), protocol_fingerprint() (+3 more)

### Community 6 - "optimization.py"
Cohesion: 0.12
Nodes (6): _IntPoly, branch_and_bound(), exact_enumeration(), quantum_solver_status(), table_from_result(), require_single_count()

### Community 8 - "make_record"
Cohesion: 0.06
Nodes (22): select_pool(), JobState, make_record(), StageStatus, StopReason, check_energy_compatibility(), check_snapshot_against_split(), freeze_physical_split() (+14 more)

### Community 9 - "screening.py"
Cohesion: 0.22
Nodes (4): MLPotentialBackend, _resolve(), _mixing(), screen()

### Community 10 - "encoding.py"
Cohesion: 0.06
Nodes (33): predict(), _ancilla_coefficients(), compile_encoding(), compile_one_hot(), complete_assignment(), count_constraints(), count_penalty(), decode_one_hot() (+25 more)

### Community 11 - "pyscf_worker.py"
Cohesion: 0.17
Nodes (14): basis_and_pseudo_hashes(), _dispersion_model(), Evaluator, main(), parse_dispersion(), _per_element(), probe(), _relax() (+6 more)

### Community 12 - "No-Agent Fixture Core"
Cohesion: 0.17
Nodes (28): bit_string(), canonical(), check_energy_compatibility(), compile_pair_qubo(), correction(), evaluate_qubo(), feasible_states(), features() (+20 more)

### Community 13 - "Toy Framework Test Helpers"
Cohesion: 0.15
Nodes (15): base_spec(), pyscf_dft_protocol(), scheme_project(), base_spec(), embedding_protocol(), _merge(), milestone_c_overrides(), pm3m_operations() (+7 more)

### Community 14 - "sqd_simulation"
Cohesion: 0.14
Nodes (13): problem_from_artifact(), _apply(), exact_diagonalization(), hamiltonian_matrix(), _np(), _problem(), _recover(), sector_determinants() (+5 more)

### Community 15 - "test_agents.py"
Cohesion: 0.07
Nodes (41): _allowed_verdicts(), _check_model_rows(), _coverage(), _error_state(), _ok_without_errors(), _record_line(), render_assessment(), number() (+33 more)

### Community 16 - "packets.py"
Cohesion: 0.11
Nodes (26): build_a1_packet(), build_a2_packet(), build_a4_packet(), build_a67_packet(), candidate_quality(), candidate_rows(), compilation_options(), _composition_feasible() (+18 more)

### Community 17 - "Physical Intake Validation Tests"
Cohesion: 0.15
Nodes (18): validate_project(), test_milestone_c_spec_errors_block_at_intake(), codes(), test_construction_failure_is_reported_never_an_energy(), test_invalid_connector_declaration_caught(), test_invalid_structural_inputs_caught_before_any_calculation(), test_known_parent_gives_checked_slot_lattice(), test_physical_policy_fields_block_with_field_path() (+10 more)

### Community 18 - "contract.py"
Cohesion: 0.07
Nodes (24): all_model_features(), assign_folds(), candidate_models(), evaluate_holdout(), expand_tokens(), feature_polynomial(), feature_value(), feature_vector() (+16 more)

### Community 19 - "project_spec.py"
Cohesion: 0.07
Nodes (28): requested_cutoff(), _cluster_prefix(), hamiltonian_from_grouped_selection(), is_known_feature(), is_transferable(), dft_protocol_errors(), tolerance_errors(), protocol_errors() (+20 more)

### Community 20 - "intake.py"
Cohesion: 0.11
Nodes (9): agent_request_ceilings(), _case_from_fidelity(), _deep_merge(), learner_path(), ProjectSpec, _read_json(), _read_jsonl(), runtime_agent_errors() (+1 more)

### Community 21 - "Framework Slot Lattice"
Cohesion: 0.11
Nodes (17): build_framework(), build_slot_lattice(), _centroid(), _components(), deconstruct(), expand_supercell(), formula_counts(), _frac_close() (+9 more)

### Community 22 - "RunStore"
Cohesion: 0.15
Nodes (3): _load(), scheme_trace(), RunStore

### Community 23 - "design.py"
Cohesion: 0.16
Nodes (17): assess(), _bits(), compile_design(), evaluate_polynomial(), fake_device(), feasible_states(), _fmt(), kang_spectrum() (+9 more)

### Community 24 - "Cluster Embedding Correction"
Cohesion: 0.16
Nodes (7): assemble_corrected_energy(), _blocked(), ClusterBackend, correct_pool(), plan_regions(), _structure(), validate_scheme()

### Community 26 - "Intake Contract Tests"
Cohesion: 0.13
Nodes (21): codes(), _edit_topologies(), test_cif_input_mode_unsupported(), test_duplicate_label_rejected(), test_empty_energy_set_rejected(), test_fixture_project_validates(), test_graph_relabelled_as_physical_net_rejected(), test_incompatible_energy_records_rejected() (+13 more)

### Community 27 - "Physical case recipe: MOF-5 BDC/amino-BDC"
Cohesion: 0.18
Nodes (9): BDC / 2-amino-BDC linkers (1:1), Postsynthetic modification of mixed-linker MOFs for ethylene oligomerization (doi:10.1039/C4RA10605A), MOF-5 / IRMOF-1 (Zn4O nodes), Physical case recipe: MOF-5 BDC/amino-BDC, Agent A1 (topology selection), AiiDA workflow engine, ML-potential screening (orb-v3 + D3BJ), Optional extras (agents, mlip, topology, qpu, aiida, gpu) (+1 more)

### Community 28 - "controls.py"
Cohesion: 0.14
Nodes (6): Controls, load_controls(), _merge(), normal_requests(), _redact(), test_controls_use_environment_secrets_and_never_expose_them()

### Community 29 - "test_refinement_and_gateway.py"
Cohesion: 0.19
Nodes (14): review_proposal(), decide(), reject(), _al(), pipeline(), _proposal(), _refinement(), _small_training_fixture() (+6 more)

### Community 30 - "load_project"
Cohesion: 0.11
Nodes (25): load_project(), run_pipeline(), runs(), toy_run(), test_agent_plan_requires_the_agent_policy(), _state(), test_acceptance_reports_failure_instead_of_crashing(), test_failed_evaluator_job_never_becomes_energy() (+17 more)

### Community 31 - "Ground State Evaluation Stage"
Cohesion: 0.18
Nodes (16): New QuMOF Pipeline Diagram, Agent A1: MOF Topology Selector, Agent A2: QUBO Hamiltonian Constructor, Agent A3: Physical Correctness Checker, Agent A4: QUBO Hamiltonian Adjuster, Classical DFT, Confirmation Stage, Ground State Evaluation Stage (+8 more)

### Community 32 - "pormake_worker.py"
Cohesion: 0.13
Nodes (11): main(), _orb(), _relax(), _sha256(), _candidate_nets(), main(), _quiet(), run() (+3 more)

### Community 33 - "scheme.py"
Cohesion: 0.15
Nodes (9): _models_for(), _row(), scripted_a1(), scripted_a2(), scripted_a4(), scripted_a67(), scripted_policies(), write_scheme_trace() (+1 more)

### Community 34 - "runner.py"
Cohesion: 0.14
Nodes (11): AgentCallError, Cache, cache_key(), call_role(), check_schema(), Ledger, _ask(), run_one() (+3 more)

### Community 35 - "PipelineError"
Cohesion: 0.11
Nodes (8): names_for_token(), PipelineError, check_no_holdout(), normalize_cell_energy(), SyntheticFixtureBackend, check_candidate_file(), configuration_id(), validate_occupation()

### Community 36 - "math"
Cohesion: 0.07
Nodes (28): check_run(), _close(), acquisition_model(), _allocate(), bits_of(), _distance(), _normalise(), policy_errors() (+20 more)

### Community 37 - "PySCF Backend Tests"
Cohesion: 0.15
Nodes (19): formate_cif(), write_pyscf_toy_project(), evaluate(), run(), settings(), test_engine_identity_is_part_of_the_fidelity(), test_forces_and_stress_match_finite_differences(), energy_eV() (+11 more)

### Community 38 - "report.py"
Cohesion: 0.19
Nodes (9): _agent_section(), build_report(), _embedding_section(), _md_table(), not_executed(), _physical_section(), _screening_section(), _topology_section() (+1 more)

### Community 39 - "Encoding/Solver Tests & Conftest"
Cohesion: 0.23
Nodes (9): fixture_core(), cubic(), _hamiltonians(), pairwise(), test_cubic_model_rejected_by_qubo_only_target_but_retained_as_hubo(), test_exact_enumeration_matches_known_minima(), test_qubo_matches_fixture_reference_and_identity(), test_simulated_annealing_agrees_with_exact() (+1 more)

### Community 40 - "cif.py"
Cohesion: 0.13
Nodes (15): apply_symop(), cell_matrix(), cif_number(), _frac_distance(), _leading(), Loop, _loop_with(), parse_cif() (+7 more)

### Community 41 - "Controls: Datasets Config"
Cohesion: 0.13
Nodes (15): datasets, enabled, format, hdf5, id, index, kind, license (+7 more)

### Community 42 - "MUF-7 LLM Benchmark Figure"
Cohesion: 0.20
Nodes (15): MUF-7 LLM Benchmark Figure, A1: QUBO Hamiltonian Construction (NMAE), A2: QAOA QUBO Solution (correct output probability), A2: QAOA Raw Energy Prediction (MAE), A3: VQE Final Structure Prediction, DeepSeek V4 Flash, DeepSeek V4 Pro, Kang's [1] MUF-7 QUBO (+7 more)

### Community 44 - "Synthetic no-agent MOF fixture"
Cohesion: 0.31
Nodes (8): Fixture acceptance criteria, Fixture integration instructions for coding agent, Orbit canonicalization, dedup and cross-graph pooling, Correction modes (none, constant, topology_dependent), Synthetic no-agent MOF fixture, Synthetic ground-truth energy formula, prism6 (hexagonal prism graph), ring12 (12-site cycle graph)

### Community 45 - "conftest.py"
Cohesion: 0.14
Nodes (14): copy_fixture(), harness_json(), read_jsonl(), test_holdout_label_smuggled_into_training_halts_run(), spec(), test_decoration_space_and_orbit_quotient(), test_feature_polynomials_match_counts(), test_feature_symmetry_and_swap_reachability() (+6 more)

### Community 46 - "OpenRouterClient"
Cohesion: 0.17
Nodes (4): OpenRouterClient, transport_schema(), run_benchmark(), work()

### Community 47 - "Controls: Literature Config"
Cohesion: 0.15
Nodes (13): literature, enabled, extra_queries, local_papers_dir, max_passage_chars, max_passages, max_sources, references (+5 more)

### Community 48 - "literature.py"
Cohesion: 0.22
Nodes (9): _accept(), _clean(), gather_evidence(), _paper_source(), query_templates(), references_from(), _resolve_calls(), title_similarity() (+1 more)

### Community 49 - "topology_builders.py"
Cohesion: 0.10
Nodes (9): BuildFailure, lattice_info_for_builder(), ParentSubstitutionBuilder, PormakeBuilder, choose_supercell(), _decoration_check(), generate_topologies(), protocol_errors() (+1 more)

### Community 50 - "Controls: OpenRouter Config"
Cohesion: 0.17
Nodes (12): openrouter, api_key, app_title, app_url, base_url, deadline_s, model, provider (+4 more)

### Community 51 - "Quadratization Tests"
Cohesion: 0.26
Nodes (8): _hamiltonians(), test_branch_and_bound_agrees_and_reports_honest_gaps(), test_penalty_bound_sublattice_counts_and_one_hot(), test_pipeline_quantum_benchmark_with_quadratization(), test_published_h2_benchmark_is_reproduced(), test_qaoa_benchmark_agrees_with_exact_and_records_provenance(), test_qaoa_mixers_preserve_constraints_and_bit_order_errors_are_caught(), test_quadratized_cubic_model_reproduces_feasible_cost()

### Community 53 - "run_muf7_full.py"
Cohesion: 0.13
Nodes (4): Builder, log(), Relaxer, zn4o_cluster()

### Community 54 - "Controls: Assessment & Cache"
Cohesion: 0.18
Nodes (10): assessment, required_checks, top_k_candidates, cache, dir, enabled, orchestration, engine (+2 more)

### Community 55 - "validation.py"
Cohesion: 0.16
Nodes (9): write_cif(), bond_graph(), map_to_parent_slots(), min_interatomic_distance(), metal_coordination(), mofchecker_check(), _structure(), validate_structure() (+1 more)

### Community 56 - "__main__.py"
Cohesion: 0.12
Nodes (12): ReplayClient, load_materials(), rescore(), check_connections(), _local_check(), run_pipeline_aiida(), run_electronic_benchmark(), solver_consistency() (+4 more)

### Community 57 - "Fixture integration instructions for coding agent"
Cohesion: 0.14
Nodes (10): finite_substitution_interaction_graph input mode, Composition-preserving QAOA, Exact enumeration (certified minima), Qiskit FakeBrisbane noisy device, Limitations, MUF-7, OpenRouter, project.json / project_spec.template.json (+2 more)

### Community 58 - "geometry_match.py"
Cohesion: 0.18
Nodes (8): _apply(), equivalence_classes(), equivalent(), close(), fingerprint(), _frac_to_cart(), _lattice_params(), supercell_operations()

### Community 60 - "Kang et al. design benchmark (agents-design-bench)"
Cohesion: 0.27
Nodes (8): kang_control (paper weighting in term catalogue), Kang, Kim & Kim 2025: Quantum Computing Based Design of Multivariate Porous Materials, Static provenance report (live literature NOT_RUN), Fixture data files (topologies, candidates, model_candidates, splits, literature_catalog), Agent A2 (Hamiltonian model design), Cu-THQ-HHTP, Kang et al. design benchmark (agents-design-bench), Py-MV-DBA-COF

### Community 61 - "json"
Cohesion: 0.15
Nodes (11): cluster_vqe_sqd(), main(), test_aiida_engine_reproduces_the_local_engine(), test_ml_screening_deprioritises_only_calibrated_gaps_and_narrows_the_run(), test_qaoa_on_fake_brisbane_matches_the_simulator_and_reports_noise(), test_store_rejects_a_concurrent_writer(), test_uncalibrated_or_failed_screening_keeps_every_topology(), _toy() (+3 more)

### Community 62 - "CLAUDE.md"
Cohesion: 0.25
Nodes (6): 1. Think Before Coding, 2. Simplicity First, 3. Surgical Changes, 4. Goal-Driven Execution, graphify, Linting & formatting (ruff)

### Community 63 - "Fixture Model Ladder M0-M2"
Cohesion: 0.28
Nodes (7): Classical exact fixed-composition baseline (924 states), UNSUPPORTED_HIGHER_ORDER_WITHOUT_QUADRATIZATION, core_pairwise case, higher_order case, Model M0 (constant + unlike NN pairs), Model M1 (M0 + distance-two pairs), Model M2 (M1 + all-B path triples, cubic)

### Community 65 - "store.py"
Cohesion: 0.19
Nodes (4): _acceptance(), _agent_metrics(), evaluate(), render()

### Community 66 - "cut_region"
Cohesion: 0.16
Nodes (11): cut_region(), add(), position(), _cart_to_frac(), _close_pairs(), frac_to_cart(), _match(), _min_image_distance() (+3 more)

### Community 67 - "Controls: Material Fields"
Cohesion: 0.25
Nodes (8): doi, formula, metals, mofid, name, record_id, topology, columns

### Community 68 - "test_design_bench.py"
Cohesion: 0.36
Nodes (6): build_packet(), design(), test_design_contract_rejects_invalid_or_constant_hamiltonians(), codes(), test_model_designs_are_compiled_solved_and_scored_against_the_experimental_arrangement(), test_reference_reproduces_the_published_spectrum_and_scores_the_paper_weighting_as_exact()

### Community 69 - ".__call__"
Cohesion: 0.19
Nodes (7): build_cell(), _host(), _initial_guess(), _scf_object(), SCFNotConverged, _stress_cpu(), WorkerError

### Community 70 - "active_space.py"
Cohesion: 0.21
Nodes (5): integral_hash(), prepare_active_space(), read_fcidump(), _require(), test_electronic_solvers_agree_on_identical_tiny_hamiltonian()

### Community 71 - "run_embedding_benchmark"
Cohesion: 0.21
Nodes (6): compute(), main(), _scf(), _molecule_structure(), run_embedding_benchmark(), energy()

### Community 72 - "Subtractive embedding at metal nodes"
Cohesion: 0.39
Nodes (6): CASCI, CCSD, H2 STO-3G electronic benchmark (Szabo & Ostlund), Keto/enol HF-to-CCSD embedding benchmark, SQD (sample-based quantum diagonalization), VQE

### Community 73 - "DFT-fitted QUBO Hamiltonian (step 3)"
Cohesion: 0.29
Nodes (6): Multivariate MOFs (MTV-MOFs), Periodic DFT ranking (step 5), PySCF, QuMOF pipeline, Simulated annealing, Toy frameworks with mock DFT

### Community 75 - "Controls: MCP Valency"
Cohesion: 0.33
Nodes (6): mcp, valency, api_token, enabled, timeout_s, url

### Community 76 - "electronic_solvers.py"
Cohesion: 0.32
Nodes (3): pyscf_casci(), _result(), sqd_hardware()

### Community 77 - "qpu_worker.py"
Cohesion: 0.48
Nodes (5): _device(), dicke(), main(), qaoa_circuit(), _scs()

### Community 80 - "main"
Cohesion: 0.67
Nodes (3): main(), score(), spearman()

### Community 81 - "pathlib"
Cohesion: 0.19
Nodes (4): load_aiida(), sha(), spec_dict(), write_mof5_scheme_project()

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
- **22 isolated node(s):** `qumof`, `BDC / 2-amino-BDC linkers (1:1)`, `Agent A1 (topology selection)`, `Multivariate MOFs (MTV-MOFs)`, `PySCF` (+17 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 618 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **17 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `PipelineError` connect `PipelineError` to `Pipeline`, `transfer.py`, `structures.py`, `Milestone C/DFT Model Tests`, `dft.py`, `optimization.py`, `make_record`, `screening.py`, `encoding.py`, `sqd_simulation`, `packets.py`, `Physical Intake Validation Tests`, `contract.py`, `project_spec.py`, `intake.py`, `Framework Slot Lattice`, `RunStore`, `Cluster Embedding Correction`, `Intake Contract Tests`, `controls.py`, `load_project`, `pormake_worker.py`, `runner.py`, `math`, `Encoding/Solver Tests & Conftest`, `cif.py`, `topology_builders.py`, `Quadratization Tests`, `SequentialGraph`, `validation.py`, `__main__.py`, `json`, `store.py`, `cut_region`, `active_space.py`, `run_embedding_benchmark`, `electronic_solvers.py`, `pathlib`?**
  _High betweenness centrality (0.159) - this node is a cross-community bridge._
- **Are the 40 inferred relationships involving `PipelineError` (e.g. with `SequentialGraph` and `compute()`) actually correct?**
  _`PipelineError` has 40 INFERRED edges - model-reasoned connections that need verification._
- **What connects `qumof`, `BDC / 2-amino-BDC linkers (1:1)`, `Agent A1 (topology selection)` to the rest of the system?**
  _22 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `transfer.py` be split into smaller, more focused modules?**
  _Cohesion score 0.14285714285714285 - nodes in this community are weakly interconnected._
- **Why does `make_record()` connect `make_record` to `Pipeline`, `transfer.py`, `structures.py`, `dft.py`, `optimization.py`, `screening.py`, `encoding.py`, `Physical Intake Validation Tests`, `contract.py`, `project_spec.py`, `intake.py`, `Framework Slot Lattice`, `RunStore`, `Cluster Embedding Correction`, `test_refinement_and_gateway.py`, `load_project`, `runner.py`, `PipelineError`, `math`, `report.py`, `validation.py`, `__main__.py`, `json`, `active_space.py`, `run_embedding_benchmark`, `electronic_solvers.py`?**
  _High betweenness centrality (0.053) - this node is a cross-community bridge._
- **Should `structures.py` be split into smaller, more focused modules?**
  _Cohesion score 0.10582010582010581 - nodes in this community are weakly interconnected._

### Low-confidence Hints
_AMBIGUOUS edges — the extractor was unsure. Verify before acting on these._

- **What is the exact relationship between `refinement.py` and `Optimisation Feedback Loop`?**
  _Edge tagged AMBIGUOUS (relation: references) - confidence is low._