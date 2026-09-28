## Digital gate Simulator

A web-based **Digital gate Simulator** that allows users to interactively simulate logic gates, combinational circuits, and sequential circuits. The simulator provides live input/output updates, circuit visualization, logic expressions, truth tables, characteristic tables, and sequential-state simulation.

##  Features

###  Logic Gates

Supports the following fundamental logic gates:

* AND
* OR
* NOT
* NAND
* NOR
* XOR
* XNOR

Users can change the input values and instantly observe the corresponding output.

###  Combinational Circuits

The simulator supports:

* Half Adder
* Full Adder
* Half Subtractor
* Full Subtractor
* 2:1 Multiplexer
* 4:1 Multiplexer
* 1:2 Demultiplexer
* 1:4 Demultiplexer
* 2:4 Decoder
* 4:2 Encoder

Each circuit displays its inputs, outputs, logic expression, and corresponding truth table.

###  Sequential Circuits

The project also simulates basic sequential circuits:

* SR Latch
* D Flip-Flop
* JK Flip-Flop
* T Flip-Flop

For clock-controlled flip-flops, users can apply clock pulses and observe the change in the stored state `Q`.

###  Interactive Truth & Characteristic Tables

The simulator automatically generates:

* Truth tables for logic gates and combinational circuits
* Characteristic tables for sequential circuits
* Current-input highlighting
* Next-state (`Q⁺`) information for sequential circuits

The tables are generated dynamically based on the selected circuit and number of inputs.

###  Live Circuit Visualization

A dynamic SVG-based circuit view displays:

* Input wires
* Output wires
* Circuit name
* Current input values
* Current output values
* Sequential circuit state
* Clock connection for flip-flops

Wire states are visually represented according to their binary value.

###  Logic Expressions

Each supported circuit displays its corresponding Boolean expression.

Examples:

```text
AND       → Y = A · B
OR        → Y = A + B
XOR       → Y = A ⊕ B
Half Adder → SUM = A ⊕ B
            CARRY = A · B
```

###  Sequential State & Clock History

For clock-controlled sequential circuits, the simulator maintains the current state and records the output state after each clock edge.

Example:

```text
Q after each clock edge:
0 → 1 → 1 → 0 → 1
```

##  Technologies Used

* **HTML5** – Web page structure
* **CSS3** – Styling and responsive layout
* **JavaScript** – Circuit logic, simulation, dynamic tables, and visualization
* **SVG** – Live circuit diagram generation

##  Project Structure

```text
Digital-Logic-Simulator/
│
└── index.html
```

The project is implemented as a lightweight standalone web application containing the interface, styling, circuit logic, simulation functions, and SVG visualization.

##  How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Open the project

Navigate to the project folder.

### 3. Run the application

Open:

```text
index.html
```

in any modern web browser.

No server or external database is required.

##  How to Use

1. Open the simulator.
2. Select a logic gate or circuit from the dropdown.
3. Change the input values using the input buttons.
4. Observe the live output.
5. View the corresponding Boolean expression.
6. Examine the generated circuit diagram.
7. Check the truth table or characteristic table.
8. For flip-flops, apply clock pulses and observe the state transitions.

##  Concepts Demonstrated

This project demonstrates practical implementation of:

* Boolean Algebra
* Logic Gates
* Truth Tables
* Combinational Logic
* Sequential Logic
* Adders and Subtractors
* Multiplexers
* Demultiplexers
* Encoders and Decoders
* Latches
* Flip-Flops
* Clock-based State Transitions
* Next-State Logic
* SVG-based Circuit Visualization
* Dynamic DOM Manipulation

##  Circuit Examples

### Half Adder

```text
SUM   = A ⊕ B
CARRY = A · B
```

### Full Adder

```text
SUM   = A ⊕ B ⊕ Cin
CARRY = AB + Cin(A ⊕ B)
```

### 2:1 Multiplexer

```text
Y = S'·D0 + S·D1
```

### D Flip-Flop

```text
Q⁺ = D
```

### JK Flip-Flop

```text
J = 0, K = 0 → Hold
J = 1, K = 0 → Set
J = 0, K = 1 → Reset
J = 1, K = 1 → Toggle
```

## Input Validation

The simulator also handles invalid sequential-circuit conditions. For example, the SR latch identifies the `S = R = 1` condition as an invalid input combination and indicates that the next state is undefined.

##  Purpose of the Project

The main purpose of this project is to provide an interactive and easy-to-understand environment for learning and experimenting with **digital logic circuits**.

Instead of manually calculating every output using truth tables, users can modify inputs and immediately observe the resulting circuit behavior.

## Future Enhancements

Possible future improvements include:

* Drag-and-drop circuit design
* User-defined circuit construction
* More sequential circuits
* Counters and registers
* Timing diagrams
* Circuit simulation animation
* Boolean expression simplification
* Circuit export as an image
* Save/load custom circuits
* Mobile-friendly circuit editor







