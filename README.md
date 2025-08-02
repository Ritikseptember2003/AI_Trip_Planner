# AI Trip Planner

This project sets up a Python development environment using **uv** (a fast and minimal Python environment manager) with Python 3.12.11, and installs the `langchain` library for AI trip planning development.

---

## ⚙️ Local Environment Setup

Follow these steps to set up your local development environment:

### 1. Install and Verify `uv`

If you don't have `uv` installed yet:

```bash
# Install pipx if not already installed
sudo apt install pipx
pipx ensurepath

# Use pipx to install uv globally
pipx install uv

# Verify uv installation
uv --version


# Create a virtual environment with Python 3.12.11 (Linux example):
uv venv env --python cpython-3.12.11-linux-x86_64-gnu
source ./env/bin/activate

# Note:
# For Windows, after creating the environment, activate it using:
.\env\Scripts\activate.bat

# If you have Conda activated, run conda deactivate before activating this env.

# List installed packages:
uv pip list

# Install the LangChain Library
uv pip install langchain

# Confirm Library
uv pip list

# Initialize Project (Optional)
# If starting fresh with uv project initialization:
uv init AI_Trip_Planner
cd AI_Trip_Planner/

# Additional Python Versions / Packages
# If you want to install or switch Python versions within uv:
# Example installing Python 3.10.18 for Windows
uv python install cpython-3.10.18-windows-x86_64-none

# Create venv with this python version
uv venv env --python cpython-3.10.18-windows-x86_64-none

# You can also add packages globally within the uv environment:
uv add pandas

# Running the Application
# Once your environment is ready, you can start your application:

# For Streamlit apps:
streamlit run streamlit_app.py

# For FastAPI apps (if applicable):
uvicorn main:app --reload --port 8000

