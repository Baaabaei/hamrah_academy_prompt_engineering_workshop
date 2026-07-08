# Setup Guide

## 🖥️ System Requirements

- **OS**: Windows, macOS, or Linux
- **Python**: 3.8 or higher
- **Memory**: 4GB minimum (8GB recommended)
- **Internet**: Required for API access

## 📦 Installation Steps

### Step 1: Clone the Repository

```bash
git clone https://github.com/Baaabaei/hamrah_academy_prompt_engineering_workshop.git
cd hamrah_academy_prompt_engineering_workshop
```

### Step 2: Create Virtual Environment

**On macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

**On Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

### Step 3: Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### Step 4: Configure API Keys

Create a `.env` file in the root directory:

```bash
touch .env
```

Add your API keys:
```
OPENAI_API_KEY=your_api_key_here
# Other API keys as needed
```

**⚠️ Important**: Never commit `.env` to version control! It's in `.gitignore`.

### Step 5: Launch Jupyter

```bash
jupyter notebook
```

Or use JupyterLab:
```bash
jupyter lab
```

## 🐍 Python Version Compatibility

| Python Version | Status |
|---|---|
| 3.8 | ✅ Supported |
| 3.9 | ✅ Supported |
| 3.10 | ✅ Supported |
| 3.11 | ✅ Supported |
| 3.7 or lower | ❌ Not supported |

## 🔧 Troubleshooting

### Issue: `python: command not found`

**Solution**: Make sure Python is installed and added to PATH
```bash
python3 --version  # Try with python3
```

### Issue: Permission denied for venv

**Solution**: Use `chmod` on macOS/Linux
```bash
chmod +x venv/bin/activate
source venv/bin/activate
```

### Issue: Module not found errors

**Solution**: Ensure virtual environment is activated
```bash
which python  # Should show path to venv
pip list     # Should show installed packages
```

### Issue: Jupyter kernel not found

**Solution**: Install ipykernel
```bash
pip install ipykernel
python -m ipykernel install --user --name prompt_eng
```

## 🌐 API Setup (OpenAI Example)

1. Get API key from [https://platform.openai.com/api-keys](https://platform.openai.com/api-keys)
2. Create `.env` file with:
   ```
   OPENAI_API_KEY=sk-...
   ```
3. Load in Python:
   ```python
   from dotenv import load_dotenv
   import os
   
   load_dotenv()
   api_key = os.getenv("OPENAI_API_KEY")
   ```

## ✅ Verify Installation

Run this test script:

```python
import subprocess
import sys

# Check Python version
print(f"✓ Python {sys.version}")

# Check packages
packages = ['jupyter', 'openai', 'pandas', 'numpy']
for package in packages:
    try:
        __import__(package)
        print(f"✓ {package} installed")
    except ImportError:
        print(f"✗ {package} NOT installed")
```

## 🚀 Next Steps

1. Review the main [README.md](README.md)
2. Start with `notebooks/01-introduction.ipynb`
3. Check [CONTRIBUTING.md](CONTRIBUTING.md) if you want to contribute

---

Need help? [Open an issue](https://github.com/Baaabaei/hamrah_academy_prompt_engineering_workshop/issues)
