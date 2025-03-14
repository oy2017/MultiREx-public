# MultiREx Repository Structure

This document provides a detailed overview of the MultiREx repository structure and its main components.

## Repository Layout

```
.
├── .banner                 # Banner file
├── .gitignore             # Git ignore rules
├── .readthedocs.yml       # ReadTheDocs configuration
├── .versions              # Version tracking
├── LICENSE                # Project license
├── README.md             # Project documentation
├── WHATSNEW.md           # Changelog
├── bin/                  # Binary and script files
│   └── release.sh        # Release script
├── dev/                  # Development resources
│   ├── TODO.md           # Development tasks
│   ├── attic/            # Development notebooks
│   │   ├── example.ipynb
│   │   ├── multirex-explore-compositions.ipynb
│   │   └── test.ipynb
│   └── use-cases.ipynb   # Use cases documentation
├── docs/                 # Documentation
│   ├── Makefile          # Documentation build file
│   ├── _static/          # Static resources
│   │   └── custom.css    # Custom styling
│   ├── conf.py          # Sphinx configuration
│   ├── index.rst        # Documentation index
│   ├── make.bat         # Windows build script
│   ├── modules.rst      # Modules documentation
│   └── notebooks/       # Documentation notebooks
│       └── quickstart.ipynb
├── examples/             # Example files
│   ├── multirex-quickstart.ipynb  # Quick start guide
│   ├── papers/          # Paper-related examples
│   │   ├── .gitignore
│   │   ├── DZF-MLBiosignatureClassification/
│   │   └── README.md
│   └── resources/       # Example resources
│       ├── contributions-transmission-spectrum.png
│       └── synthetic-transmission-spectra.png
├── makefile             # Project makefile
├── multirex/            # Main package source
│   ├── __init__.py     # Package initialization
│   ├── __randinstrument.py
│   ├── data/           # Package data
│   │   ├── opacCH4.dat
│   │   ├── opacCO2.dat
│   │   ├── opacH2O.dat
│   │   ├── opacO2.dat
│   │   └── opacO3.dat
│   ├── spectra.py      # Spectra handling
│   ├── utils.py        # Utility functions
│   ├── version.py      # Version information
│   └── tests/          # Test directory
├── pyproject.toml      # Project configuration
└── setup.py           # Setup script
```

## Main Components

### Source Code
The main package source code is located in the `multirex/` directory, containing the core functionality of the package.

### Documentation
Documentation is managed in the `docs/` directory using Sphinx, with configuration in `conf.py` and source files in RST format.

### Examples
The `examples/` directory contains Jupyter notebooks demonstrating package usage, including a quickstart guide and paper-related examples.

### Development
Development resources are in the `dev/` directory, including TODO lists and development notebooks.

### Tests
Test files are located in the `tests/` directory.

### Configuration Files
- `pyproject.toml`: Project dependencies and build configuration
- `setup.py`: Package installation script
- `.readthedocs.yml`: Documentation build configuration
- `makefile`: Build and maintenance tasks
