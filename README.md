# LuxDev Assignment - Week 12 Analysis
This repository contains the solution for the [LuxDevHQ Week 12 Assignment] (https://github.com/LuxDevHQ/assignment_week_12).
The project is built using **uv** for dependency management.

## Project Structure

```text
luxdev_assignment_12/
├── .venv/                            
├── notebooks/            
├── src/                  
├── pyproject.toml      
└── README.md           

```
## Windows Installation & Setup

### 1. Install uv
If not installed,  Open PowerShell and run:

```powershell
powershell -ExecutionPolicy ByPass -c "irm [https://astral.sh/uv/install.ps1](https://astral.sh/uv/install.ps1) | iex"

```
### 2. Initialize Project & Folders

```powershell
#Navigate to project root
uv init

# Create project folders
mkdir notebooks, src

```
### 3. Install required dependencies

```powershell
# Add basic analysis libraries, not really required.
uv add pandas numpy

# Add development tools for Jupyter
uv add --dev jupyter ipykernel

```
### 4. Configure Jupyter Kernel

Register the environment so it appears in notebook kernel list:

```powershell
uv run python -m ipykernel install --user --name=luxdev_w12 --display-name "Python (LuxDev W12)"

```
## How to Run

1. **VS Code:** Open the folder, open any `.ipynb` file, and select the **Python (LuxDev W12)** kernel.
2. **Jupyter Lab:** Run `uv run jupyter lab` in your terminal.

