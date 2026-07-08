# Hamrah Academy Prompt Engineering Workshop 🎓

> A comprehensive tutorial repository on prompt engineering and advanced LLM techniques developed during the Hamrah Academy workshop.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)

## 📌 Overview

This repository contains hands-on tutorials, notebooks, and exercises for mastering prompt engineering with Large Language Models (LLMs). Perfect for learners who want to understand how to effectively communicate with AI models and unlock their full potential.

## 🎯 What You'll Learn

- ✅ **Fundamentals of Prompt Engineering** - Principles and best practices
- ✅ **Advanced Prompting Techniques** - Few-shot learning, chain-of-thought, role-playing
- ✅ **Mathematical Reasoning with LLMs** - Solving complex problems step-by-step
- ✅ **Real-World Applications** - Case studies and practical examples
- ✅ **Optimization & Troubleshooting** - Improving model outputs

## 📚 Table of Contents

| Notebook | Topic | Difficulty |
|----------|-------|-----------|
| `01-introduction.ipynb` | Prompt Engineering Basics | Beginner |
| `02-math-llm.ipynb` | Mathematical Problem Solving | Intermediate |
| `03-advanced-techniques.ipynb` | Advanced Prompting Strategies | Advanced |

## 🚀 Quick Start

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- An OpenAI API key (or compatible LLM provider)

### Installation

```bash
# Clone the repository
git clone https://github.com/Baaabaei/hamrah_academy_prompt_engineering_workshop.git
cd hamrah_academy_prompt_engineering_workshop

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Start Jupyter
jupyter notebook
```

### First Steps

1. Start with `notebooks/01-introduction.ipynb`
2. Follow along with the examples
3. Modify and experiment with the prompts
4. Progress to advanced topics

## 📋 Requirements

```
jupyter>=1.0.0
openai>=1.0.0
python-dotenv>=0.19.0
pandas>=1.3.0
numpy>=1.21.0
```

Install all requirements:
```bash
pip install -r requirements.txt
```

## 💡 Key Concepts Covered

### Prompt Engineering Principles
- **Clarity** - Be specific and direct
- **Context** - Provide relevant background
- **Examples** - Show few-shot demonstrations
- **Constraints** - Define output format and boundaries

### Techniques Explained

1. **Chain-of-Thought** - Breaking down complex problems
2. **Few-Shot Prompting** - Learning from examples
3. **Role-Playing** - Adopting specific personas
4. **Retrieval-Augmented Generation (RAG)** - Combining external knowledge

## 🔧 Usage Examples

### Basic Prompt
```python
from openai import OpenAI

client = OpenAI()
response = client.chat.completions.create(
    model="gpt-3.5-turbo",
    messages=[
        {"role": "user", "content": "What is prompt engineering?"}
    ]
)
print(response.choices[0].message.content)
```

See `notebooks/` for more detailed examples.

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Add your improvements or new tutorials
4. Commit your changes (`git commit -m 'Add new tutorial on X'`)
5. Push to the branch (`git push origin feature/your-feature`)
6. Open a Pull Request

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

## 📖 Resources & References

- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [Chain-of-Thought Paper](https://arxiv.org/abs/2201.11903)
- [Few-Shot Learning with LLMs](https://arxiv.org/abs/2005.14165)
- [RAG: Retrieval-Augmented Generation](https://arxiv.org/abs/2005.11401)

## 🎓 Course Structure

**Module 1: Foundations** (Weeks 1-2)
- Basics of LLMs
- Introduction to prompting
- Hands-on exercises

**Module 2: Intermediate** (Weeks 3-4)
- Advanced techniques
- Real-world applications
- Project work

**Module 3: Advanced** (Weeks 5-6)
- Optimization strategies
- Fine-tuning vs. prompting
- Capstone project

## 🐛 Troubleshooting

### Common Issues

**Q: API Rate Limit Exceeded**
```python
import time
time.sleep(60)  # Wait 60 seconds before retrying
```

**Q: ImportError for openai**
```bash
pip install --upgrade openai
```

**Q: Jupyter notebook not found**
```bash
pip install jupyter
jupyter notebook
```

See [TROUBLESHOOTING.md](TROUBLESHOOTING.md) for more help.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ✨ Acknowledgments

- Hamrah Academy for organizing the workshop
- Contributors and learners in the community
- OpenAI and other LLM providers

## 📧 Contact & Support

- **Issues & Questions**: [Open an issue](https://github.com/Baaabaei/hamrah_academy_prompt_engineering_workshop/issues)
- **Email**: contact@yoursite.com
- **Twitter**: [@yourhandle](https://twitter.com/yourhandle)

## 🌟 Show Your Support

If this tutorial helped you, please:
- ⭐ Star this repository
- 🔗 Share with others
- 💬 Leave feedback
- 🤝 Contribute improvements

---

**Happy Learning!** 🚀

Last Updated: December 2025 | Maintained by [@Baaabaei](https://github.com/Baaabaei)
