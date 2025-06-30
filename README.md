# AI Trip Planner

This project sets up a Python environment using `uv` with Python 3.12.11 and installs the `langchain` library for future development.

---

## ⚙️ Local Environment Setup

```bash
# Step 1: Create virtual environment using uv with Python 3.12.11
uv venv env --python cpython-3.12.11-linux-x86_64-gnu

# Step 2: Activate the environment
source /home/ritik-kumar/AI_Trip_Planner/env/bin/activate

# Step 3: List installed packages
uv pip list

# Step 4: Install langchain
uv pip install langchain

# Step 5: Confirm installation
uv pip list

# If not already installed
python3 -m pip install uv

# Install pipx and ensure path
sudo apt install pipx
pipx ensurepath

# Use pipx to install uv globally
pipx install uv

# Verify installation
uv --version

uv init AI_Trip_Planner
cd AI_Trip_Planner/
