# 🧪 Machine Learning Projects Environment Setup (with Miniconda)

This guide helps you install **Miniconda**, create a virtual environment, install dependencies, and launch Jupyter Notebook to run the machine learning projects in this repository.

---

## 📥 Step 1: Install Miniconda

1. Visit the official Miniconda download page:  
   👉 [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)

2. Download the installer for your operating system (Windows, macOS, or Linux).

3. Follow the installation instructions for your platform:
   - On Windows, run the `.exe` installer.
   - On macOS/Linux, run the `.sh` installer from the terminal:
     ```bash
     bash Miniconda3-latest-MacOSX-x86_64.sh
     ```

---

## ⚙️ Step 2: Create a New Conda Environment

Open your terminal (or Anaconda Prompt on Windows) and run:

```bash
conda create -n ml-env python=3.11 -y
```
🔹 Replace ml-env with your preferred environment name.
🔹 You can also specify a different Python version if needed.

Activate the environment:
```bash
conda activate ml-env
```

You can install the latest versions of the core ML libraries using:
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

Launch Jupyter Notebook:
```bash
jupyter notebook
```

Optional: Save Environment to YAML File
```bash
conda env export > environment.yml
```

To recreate the environment later:
```bash
conda env create -f environment.yml
```


Happy Learning! 🚀