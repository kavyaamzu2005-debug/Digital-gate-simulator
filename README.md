# Digital Logic Gate Simulator

Digital Logic Gate Simulator is a web-based interactive application that
allows users to simulate basic digital logic gates and arithmetic
circuits. Users can change binary inputs and observe the corresponding
outputs and truth tables dynamically.

## Features

-   AND Gate
-   OR Gate
-   NOT Gate
-   NAND Gate
-   NOR Gate
-   XOR Gate
-   XNOR Gate
-   Half Adder
-   Full Adder
-   Interactive binary inputs
-   Dynamic output calculation
-   Dynamic truth tables
-   Current input combination highlighting
-   Boolean logic expressions
-   Responsive user interface

## Technology Stack

### Frontend

-   HTML5
-   CSS3
-   JavaScript

### Development Tools

-   Visual Studio Code
-   Git
-   GitHub

## Application Flow

``` text
User
  ↓
HTML / CSS / JavaScript
  ↓
Select Logic Gate / Circuit
  ↓
Change Binary Inputs
  ↓
JavaScript Logic Calculation
  ↓
Output
  ↓
Truth Table
```

## Logic Gates

### AND Gate

The AND gate produces an output of `1` only when both inputs are `1`.

``` text
Y = A AND B
```

Truth table:

``` text
A  B  Y
0  0  0
0  1  0
1  0  0
1  1  1
```

### OR Gate

The OR gate produces an output of `1` when at least one input is `1`.

``` text
Y = A OR B
```

Truth table:

``` text
A  B  Y
0  0  0
0  1  1
1  0  1
1  1  1
```

### NOT Gate

The NOT gate produces the opposite value of the input.

``` text
Y = NOT A
```

Truth table:

``` text
A  Y
0  1
1  0
```

### NAND Gate

The NAND gate produces the opposite output of an AND gate.

``` text
Y = NOT(A AND B)
```

Truth table:

``` text
A  B  Y
0  0  1
0  1  1
1  0  1
1  1  0
```

### NOR Gate

The NOR gate produces the opposite output of an OR gate.

``` text
Y = NOT(A OR B)
```

Truth table:

``` text
A  B  Y
0  0  1
0  1  0
1  0  0
1  1  0
```

### XOR Gate

The XOR gate produces an output of `1` when the two inputs are
different.

``` text
Y = A XOR B
```

Truth table:

``` text
A  B  Y
0  0  0
0  1  1
1  0  1
1  1  0
```

### XNOR Gate

The XNOR gate produces an output of `1` when both inputs are the same.

``` text
Y = A XNOR B
```

Truth table:

``` text
A  B  Y
0  0  1
0  1  0
1  0  0
1  1  1
```

## Arithmetic Circuits

### Half Adder

A Half Adder is a combinational circuit that adds two binary inputs.

Inputs:

``` text
A
B
```

Outputs:

``` text
SUM
CARRY
```

Logic equations:

``` text
SUM = A XOR B
CARRY = A AND B
```

Truth table:

``` text
A  B  SUM  CARRY
0  0   0     0
0  1   1     0
1  0   1     0
1  1   0     1
```

### Full Adder

A Full Adder adds three binary inputs.

Inputs:

``` text
A
B
Cin
```

Outputs:

``` text
SUM
CARRY
```

Logic equations:

``` text
SUM = A XOR B XOR Cin

CARRY = (A AND B) OR (Cin AND (A XOR B))
```

Truth table:

``` text
A  B  Cin  SUM  CARRY
0  0   0    0     0
0  0   1    1     0
0  1   0    1     0
0  1   1    0     1
1  0   0    1     0
1  0   1    0     1
1  1   0    0     1
1  1   1    1     1
```

## Truth Tables

The application dynamically generates truth tables according to the
selected gate or circuit.

For two-input logic gates:

``` text
2² = 4 input combinations
```

For the NOT gate:

``` text
2¹ = 2 input combinations
```

For the Half Adder:

``` text
2² = 4 input combinations
```

For the Full Adder:

``` text
2³ = 8 input combinations
```

The currently selected input combination is highlighted in the truth
table.

## JavaScript Logic

The application uses JavaScript to perform the logic calculations and
update the interface dynamically.

The selected gate or circuit determines:

-   Number of inputs
-   Input values
-   Output calculation
-   Logic expression
-   Truth table
-   Current row highlighting

No backend or database is required for this project.

## Project Structure

``` text
Digitalgate
│
├── index.html
```

### index.html

Contains:

-   HTML structure
-   CSS styling
-   JavaScript functionality
-   Logic gate calculations
-   Half Adder calculation
-   Full Adder calculation
-   Dynamic truth table generation
-   Input and output controls


## Requirements

Before running the project, install/configure:

-   Visual Studio Code
-   A modern web browser
-   Git (optional, for version control)
-   Live Server extension (optional)

## Running the Project

### Method 1 -- Direct Browser

1.  Download or clone the repository.
2.  Open the project folder.
3.  Open `index.html` in a web browser.
4.  Select a gate or circuit.
5.  Change the input values.
6.  Observe the output and truth table.

### Method 2 -- VS Code Live Server

1.  Open the project in Visual Studio Code.
2.  Open `index.html`.
3.  Install the Live Server extension if required.
4.  Right-click `index.html`.
5.  Select `Open with Live Server`.
6.  The application opens in the browser.

## GitHub

The project can be maintained using Git and GitHub for version control.


## Deployment

Since this project uses only HTML, CSS, and JavaScript, it can be
deployed as a static website.

Possible deployment options include:

-   GitHub Pages
-   Other static website hosting platforms

## Future Enhancements

-   Additional arithmetic circuits
-   Multiplexer and Demultiplexer
-   Encoder and Decoder
-   Flip-Flops
-   Sequential circuits
-   Multi-gate circuit simulation
-   Circuit diagram visualization
-   Drag-and-drop circuit builder
-   Improved mobile responsiveness
-   Light and dark theme options

## Learning Outcomes

This project provides practical understanding of:

-   Digital Logic Gates
-   Boolean Logic
-   Truth Tables
-   Binary Operations
-   Half Adder
-   Full Adder
-   Combinational Circuits
-   HTML
-   CSS
-   JavaScript
-   DOM Manipulation
-   Event Handling
-   Dynamic UI Updates
-   Git and GitHub




