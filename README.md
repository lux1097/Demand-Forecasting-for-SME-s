# Demand Forecasting

A template repository for building demand forecasting models with GitHub Copilot assistance.

## Prerequisites

### 1. Install VS Code

Download and install Visual Studio Code from [https://code.visualstudio.com/](https://code.visualstudio.com/)

### 2. Create GitHub Account

1. Go to [https://github.com](https://github.com)
2. Click **Sign up** in the top right corner
3. Enter your email address and follow the setup steps
4. Verify your email address when prompted
5. Complete your GitHub profile

### 3. Sign in to GitHub in VS Code

This step is **crucial** for using GitHub Copilot and accessing repositories:

1. Open VS Code
2. Click the **Accounts** icon in the bottom-left corner (person icon)
3. Select **Sign in with GitHub to use GitHub Copilot**
4. A browser window will open - click **Authorize Visual Studio Code**
5. You may be asked to confirm in VS Code - click **Open** if prompted
6. Verify you're signed in by checking the Accounts icon shows your GitHub username

> **Important:** You must be signed in to GitHub in VS Code to use Copilot features throughout this project.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/v0lab/triode-demand-forecasting.git
cd triode-demand-forecasting
```

### 2. Install UV (Python Package Manager)

This project uses [uv](https://github.com/astral-sh/uv) for Python virtual environment and package management.

**Installation (requires PowerShell):**

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

For more installation options, see: [https://docs.astral.sh/uv/getting-started/installation/#installation-methods](https://docs.astral.sh/uv/getting-started/installation/#installation-methods)

### 3. Setup Environment

Create virtual environment and install dependencies:

```bash
uv sync
```

**Managing Packages:**
- Add new package: `uv add <package-name>`
- Remove package: `uv remove <package-name>`

> **Note:** The `pyproject.toml` file includes all necessary packages for demand forecasting.

### 4. Select Jupyter Notebook Kernel

Configure the Python kernel for all Jupyter notebooks:

1. Press `Ctrl + Shift + P` to open the Command Palette
2. Type and select **"Notebook: Select Notebook Kernel"**
3. Choose **"Python Environments..."**
4. Select the Python interpreter from the `.venv` folder (it should show the path with `.venv`)

This setting will apply to all notebooks in the project.

## Working with the Project

### Starting Your Demand Forecasting

1. **Add Your Data**: Place your data files in the `data/` folder
2. **Open GitHub Copilot Chat**: 
   - Click the chat icon in the VS Code sidebar, or
   - Press `Ctrl + Shift + I` to open Copilot Chat
3. **Start the Conversation**: Simply say "hi" or "who are you" to begin
   - Copilot has all the necessary instructions and context
   - It will guide you through the entire demand forecasting process
   - Just follow along and provide information when asked

All demand forecasting work is done in Jupyter notebooks located in the `notebooks/` folder. GitHub Copilot is configured to assist you throughout the process.

### Customizing Copilot Instructions

To update how Copilot assists you, edit the `copilot-instructions.md` file in the `.github/` folder.

## Project Structure

```
├── .github/            # GitHub configuration and Copilot instructions
├── data/               # Data files
├── notebooks/          # Jupyter notebooks for forecasting
├── pyproject.toml      # Project dependencies
└── README.md           # This file
```

