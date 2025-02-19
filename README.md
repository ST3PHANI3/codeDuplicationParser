# Code Duplication Project

This Python 3 script takes two repositories and checks for "code clones," or code which has likely been taken from elsewhere, between the two. The algorithm used comes from Lee et al. (2018) - *Tree-Pattern-Based Clone Detection with High Precision and Recall*. There are four main types of code clones:

- Type 1: exact copies
- Type 2: copies with renamed elements (ex. variables)
- Type 3: copies that have been slightly modified
- Type 4: "semantic" copies (code that is not copied, but does the same thing)

This code checks for Type 1, 2, and 3 clones.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software

- Python 3.7+ ([Download Link](https://www.python.org/downloads/))
- pip 19+ (typically already installed with Python)
- Git ([Download Link](https://git-scm.com/downloads))

### Installation

1. Clone the repository
   - `git clone github.com/calebdehaan/codeDuplicationParser.git`
2. Enter the repository directory
   - `cd codeDuplicationParser`
3. Install dependencies
   - `pip3 install -r requirements.txt`
4. Run the program
   - `python3 -m code_duplication [args]`

Alternatively you can run the program in a Python virtual environment
`./code-duplication.sh`

### Dependencies

Python packages required for the tool to run

- `gitpython`
- `bitstring`
- `fastlog`
- `windows-curses` (Windows only, required by `fastlog`)

## Built With

- [Python 3.7.3](https://www.python.org/downloads/release/python-373/) - The Python version used
- [GitPython](https://gitpython.readthedocs.io/en/stable/) - Used to pull git repositories

## Authors

- **Caleb DeHaan** - *Initial work* - [Github](https://github.com/calebdehaan)
- **Denton Wood** - *Initial work* - [Github](https://github.com/dentonmwood)
- **Stephanie Alvord** - *Initial work* - [Github](https://github.com/ST3PHANI3)
- **Schaeffer Duncan** - *Initial work* - [Github](https://github.com/SchaefferDuncan)
- **Ivo Meixner** - *Initial work* - [Github](https://github.com/natiiix)

## Acknowledgments

- [Tomáš Černý](https://cs.baylor.edu/~cerny/)
- [Pavel Tišnovský](https://github.com/tisnik)
- [Red Hat](https://www.redhat.com/en)
