# LLM Code Provenance, Memorization, and Membership Inference

This repository brings together two complementary research implementations investigating **code provenance, memorization, and membership inference in Large Language Models (LLMs)**. The projects explore the identification and analysis of human-written and LLM-generated code, with applications in trustworthy AI and programming education.

## Research Implementations

### 1. Black-Box LLM API Auditing

**Paper:** *Auditing Black-Box LLM APIs via Token Probabilities and Data Provenance: A Case Study in Source Code Generation*

**Directory:** [`black-box-api-auditing/`](./black-box-api-auditing/)

This implementation investigates code provenance in black-box LLM APIs using token probabilities and data provenance analysis.

**Key components:**
- End-to-end research pipeline (`icws_github.py`).
- Human-written Python code collected from GitHub (pre-2021).
- LLM-generated Python code samples across different GPT models.
- Sample metadata and data provenance visualization.
- OpenRouter API integration for model-based evaluation.

### 2. Student Code Provenance and Memorization

**Paper:** *Tracing Code Provenance and Memorization in LLMs for Programming Education*

**Directory:** [`student-code-provenance/`](./student-code-provenance/)

This implementation explores Min-K% probability-based membership inference, enhanced with synthetic non-member code generation, to investigate code provenance and memorization in programming education.

**Key components:**
- Min-K% probability-based membership inference.
- SaMIA-based code provenance analysis.
- ProCQA Python programming dataset.
- Evaluation across open-source and commercial LLMs.
- Case studies involving anonymized student programming assignments.

## Repository Structure

```text
llm-code-provenance/
│
├── black-box-api-auditing/
│   ├── icws_github.py
│   ├── data/
│   ├── sample_metadata.json
│   ├── data_provenance_graph.png
│   └── README.md
│
├── student-code-provenance/
│   ├── code_provenance_mink.py
│   ├── samia_for_code.py
│   ├── case_study_code_analysis.py
│   ├── case_study_metrics.py
│   └── README.md
│
├── docs/
├── requirements.txt
├── .gitignore
└── README.md
```

## Installation

Python 3.10 or later is recommended.

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/llm-code-provenance.git
cd llm-code-provenance
```

Install the dependencies:

```bash
python -m pip install -r requirements.txt
```

Configure your OpenRouter API key where required by the individual implementations.

## Running the Implementations

**Black-Box LLM API Auditing**

```bash
cd black-box-api-auditing
python icws_github.py
```

**Student Code Provenance and Memorization**

```bash
cd student-code-provenance

python code_provenance_mink.py
python samia_for_code.py

python case_study_code_analysis.py
python case_study_metrics.py
```

For detailed instructions, dataset information, API configuration, and experiment settings, refer to the README file inside each research directory.

## Data Availability

The repository includes supplementary code and datasets associated with the respective research implementations. Some datasets, including anonymized student programming submissions, are not publicly released.


## Acknowledgements

These implementations support research on LLM data provenance, memorization analysis, membership inference, and trustworthy AI.

