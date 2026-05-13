Random Automata Experiments for Robust Pattern Diagnosability

This folder contains the code and generated artifacts for the random-automata experiments used to compare the joint-diagnoser-based method and the verifier-based method for robust pattern diagnosability under sensor insertion/erasure attacks.

1. Folder Structure

random_automata_RP_experiments/
|-- README.txt
|-- README.md
|-- run_experiment.py
|-- robust_p_experiments.py
|-- random_automata_computation_statistics.xlsx
|-- nature_style_state_counts.png
|-- nature_style_state_counts.svg
`-- rp_experiment/
    |-- __init__.py
    |-- api.py
    |-- data.py
    |-- excel_export.py
    |-- model.py
    `-- plotting.py

2. Main Files

run_experiment.py:
Recommended entry point for regenerating all outputs.

robust_p_experiments.py:
Compatibility entry point with the same behavior.

rp_experiment/api.py:
Public interface. The main function is run_experiment(output_dir).

rp_experiment/model.py:
Data structure and table headers.

rp_experiment/data.py:
The 25 experiment records.

rp_experiment/excel_export.py:
Excel workbook generation.

rp_experiment/plotting.py:
PNG and SVG figure generation.


3. Table Columns

Runs:
Experiment index.

|X|:
Number of plant states.

|E|:
Number of events.

|T|:
Number of transitions.

|E_o|:
Number of observable events.

|E_ins|:
Number of events subject to insertion attacks.

|E_era|:
Number of events subject to erasure attacks.

RP:
Robust pattern diagnosability result, Yes or No.

JD:
Number of states in the joint diagnoser.

T_jd (s):
Computation time of the joint diagnoser.

|G_v|:
Number of states in the verifier.

T_v (s):
Computation time of the verifier.

