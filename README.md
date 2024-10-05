# Quantum-Clash
Quantum Clash simulates the Prisoner's Dilemma using quantum circuits, exploring how entanglement influences decision-making. This project analyzes quantum strategies versus classical outcomes, providing insights into quantum mechanics' impact on game theory and cooperation.

## Installation
To run this project, you need to have Python and Qiskit installed. You can install the required packages using pip:

bash
pip install qiskit qiskit-aer matplotlib

## CODE DESIGN

### 1. Import Libraries
Import essential libraries including numpy, qiskit, and qiskit.visualization for quantum computing and data visualization.

### 2. Create Quantum Circuit:
Function: create_quantum_circuit()
1. Initializes a quantum circuit with 2 qubits and 2 classical bits.
2. Applies a Hadamard gate to the first qubit to create superposition.
3. Utilizes a CNOT gate to entangle the qubits.
4. Measures both qubits to prepare for outcome retrieval.

### 3. Run Quantum Circuit:
Function: run_quantum_circuit(qc)
1. Sets up an instance of AerSimulator for local simulation.
2. Transpiles the quantum circuit to optimize it for the simulator.
3. Executes the circuit with a specified number of shots (4096).
4. Returns the results of the simulation.

### 4. Simulate the Prisoner's Dilemma:
Function: prisoners_dilemma()
1. Calls create_quantum_circuit() to generate the quantum circuit.
2. Executes the quantum circuit using run_quantum_circuit().
3. Extracts the outcome counts from the simulation results.
4. Prints the results to the console for review.
5. Utilizes plot_histogram() to visualize the results, displaying the distribution of outcomes.

### 5. Execution:
Calls the prisoners_dilemma() function to execute the entire simulation process.

### 6. Output:
The project generates a histogram representing the results of the quantum simulation of the Prisoner's Dilemma, showing the distribution of possible outcomes based on the quantum strategy employed.

## Usage
Run the QUANUTM_ENTANGLEMENT_PRISONER'S_DILEMMA.ipynb code blocks to simulate the Prisoner's Dilemma game. The script will execute the quantum circuit, print the results, and save the histogram of outcomes.

## Contributor
Manaswi Singh
