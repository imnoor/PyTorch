# PyTorch Project Structure

This project follows a standard machine learning project structure for PyTorch development.

## 📁 Project Structure

```
PyTorch/
├── 📁 src/                    # Source code
│   ├── 📁 models/            # Model architectures
│   ├── 📁 data/              # Data loading and processing
│   ├── 📁 utils/             # Utility functions
│   └── 📁 training/          # Training loops and logic
├── 📁 notebooks/             # Jupyter notebooks
│   ├── 📁 experiments/       # Experiment notebooks
│   └── 📁 exploration/       # Data exploration notebooks
├── 📁 data/                  # Data storage
│   ├── 📁 raw/              # Raw, unprocessed data
│   ├── 📁 processed/        # Cleaned and processed data
│   └── 📁 external/         # External datasets
├── 📁 experiments/          # Experiment tracking
├── 📁 outputs/              # Generated outputs
│   ├── 📁 models/           # Trained model weights
│   ├── 📁 figures/          # Generated plots and figures
│   └── 📁 logs/             # Training logs
├── 📁 configs/              # Configuration files
├── 📁 tests/                # Unit tests
├── 📁 scripts/              # Standalone scripts
├── 📁 docs/                 # Documentation
├── 📄 .gitignore           # Git ignore file
├── 📄 README.md            # This file
└── 📄 requirements.txt     # Python dependencies
```

## 🚀 Getting Started

### Environment Setup
1. Your conda environment is already set up at `.conda/`
2. PyTorch with CUDA support is installed
3. To activate: Use the local Python at `d:\dev\PyTorch\.conda\python.exe`

### Running Code
```bash
# Use local Python environment
d:\dev\PyTorch\.conda\python.exe your_script.py

# Or temporarily add to PATH
$env:PATH = "d:\dev\PyTorch\.conda;" + $env:PATH
python your_script.py
```

## 📂 Directory Usage

### `/src/` - Source Code
- **`models/`**: Define your PyTorch model architectures
- **`data/`**: Data loaders, datasets, and preprocessing
- **`utils/`**: Helper functions, metrics, visualization
- **`training/`**: Training loops, optimizers, schedulers

### `/notebooks/` - Jupyter Notebooks
- **`experiments/`**: Formal experiment notebooks
- **`exploration/`**: Data exploration and prototyping

### `/data/` - Data Management
- **`raw/`**: Original, immutable datasets
- **`processed/`**: Cleaned and feature-engineered data
- **`external/`**: Third-party datasets

### `/outputs/` - Generated Files
- **`models/`**: Saved model checkpoints (.pth, .pt files)
- **`figures/`**: Plots, charts, and visualizations
- **`logs/`**: Training logs, TensorBoard files

### `/configs/` - Configuration
- YAML/JSON configuration files for experiments
- Hyperparameter settings

### `/tests/` - Testing
- Unit tests for your code
- Model validation tests

### `/scripts/` - Utilities
- Training scripts
- Data download/preparation scripts
- Evaluation scripts

## 🔧 Best Practices

1. **Keep notebooks clean**: Use notebooks for exploration, move production code to `/src/`
2. **Version control**: The `.gitignore` is configured to exclude large files and environments
3. **Configuration**: Use config files instead of hardcoded parameters
4. **Documentation**: Document your models and functions
5. **Testing**: Write tests for critical functions

## 📊 Workflow Example

1. **Explore data** in `/notebooks/exploration/`
2. **Develop models** in `/src/models/`
3. **Create datasets** in `/src/data/`
4. **Train models** using `/src/training/`
5. **Save outputs** to `/outputs/`
6. **Track experiments** in `/experiments/`

Happy coding! 🎉
