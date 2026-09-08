# Finite Automata Operations Project

A Python program that provides various operations on Finite Automata, including reading, displaying, standardizing, determinizing, completing, minimizing, and testing word recognition.

## Description

Finite Automata are mathematical models used to recognize and process formal languages.

The goal of this project is to provide a Python program capable of performing several operations on Finite Automata, from reading an automaton from a file to transforming and minimizing it.

The program reads a Finite Automaton from a text file, stores it in memory, and provides different functions to analyse and transform it.

The project supports the following operations: Read a Finite Automaton from a file, display information about a Finite Automaton, check if a Finite Automaton is deterministic, check if a Finite Automaton is complete, check if a Finite Automaton is standard, standardize a Finite Automaton, determinize and complete a Finite Automaton, minimize a complete deterministic Finite Automaton, rest whether a word is recognized by a Finite Automatonand create the complementary language of a Finite Automaton.


## Getting Started

### Dependencies

To run the project, you need:

* **Python 3.x**
* A terminal or command prompt
* A Python development environment such as **Visual Studio Code**, **PyCharm**, or **IDLE** (optional)

The project uses standard Python libraries such as `csv` and `os` and does not require external libraries.

The project is designed to run on common operating systems such as Windows, Linux, and macOS, provided a compatible Python version is available.

### Installing

Clone the project:

```bash
git clone https://github.com/hezaqqq/finite_automata_ope.git
```

Then navigate to the project directory:

```bash
cd finite_automata_ope
```

Alternatively, you can download the project directly from the [GitHub repository](https://github.com/hezaqqq/finite_automata_ope).

Make sure that the Finite Automaton input files are located in the correct directory.

### Executing program

Run the project using Python:

```bash
python main.py
```

If your system uses `python3`, use:

```bash
python3 main.py
```

Once the program starts, follow the instructions displayed by the program.

1. Load a Finite Automaton from an input file.
2. Display the information of the Finite Automaton.
3. Check whether the Finite Automaton is deterministic, complete, or standard.
4. Standardize the Finite Automaton if necessary.
5. Determinize and complete the Finite Automaton.
6. Minimize the complete deterministic Finite Automaton.
7. Test word recognition.
8. Create the complementary automaton if required.

## Help

### The program does not start

Make sure that Python is correctly installed and accessible from the terminal.

For Python, you can check your installation with:

```bash
python --version
```

If your system uses `python3`, try:

```bash
python3 --version
```

### The program cannot find the input file

Make sure that the Finite Automaton input file is located in the correct directory and that the file path provided to the program is correct.

### Testing individual functions

The different Finite Automaton operations can be tested individually by importing the corresponding functions or class into a Python file.

For example:

```python
fa = finite_automata("fa_example.txt")

fa.get_fa_information()
fa.get_csv_from_fa("fa_output.csv")

fa.is_deterministic(display=True)

if not fa.is_standard():
    fa.standardization()

fa.determinization_and_completion("determinized_fa.csv")

fa.minimized_fa()

fa.complementary()
```

The results of the Finite Automaton tests are available in the `fa_result` file.
