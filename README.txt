LexiFix – Hybrid AI Spell, Context, and Grammar Corrector

LexiFix is a lightweight text-correction tool that combines a traditional spell checker with contextual predictions from BERT and optional grammar polishing using FLAN-T5. The system corrects spelling errors while preserving semantic meaning and word intent. A Gradio web interface is included for demonstration and testing.

FEATURES
- Dictionary-based spell correction (PySpellChecker)
- Contextual word replacement using BERT masked language modeling
- POS filtering to avoid incorrect substitutions
- Automatic handling of elongated words (e.g., soooo → soo)
- Optional grammar rewriting (GPU recommended)
- Preserves original punctuation and capitalization
- Simple browser interface via Gradio

REQUIREMENTS
- Python 3.9+
- Optional: NVIDIA GPU for grammar enhancement

INSTALLATION
1) Unzip project and open terminal inside folder:
   cd SpellChecker-main

2) (Optional) Create a virtual environment:
   Windows:
      python -m venv venv
      venv\Scripts\activate
   Mac/Linux:
      python3 -m venv venv
      source venv/bin/activate

3) Install dependencies:
   pip install -r requirements.txt

RUNNING THE APPLICATION
Run:
   python app.py
(or the appropriate interface file like LexiFix.py)

A local browser link will appear. Open it to use LexiFix.

USAGE
1) Enter text in the input box.
2) Click 'Run Spell + Context + Grammar'
3) View:
   - Original text
   - Spell + contextual corrected text
   - Grammar-polished output (GPU only)
   - Word-level correction summary

GPU SUPPORT
If a CUDA GPU is available, grammar rewriting is enabled automatically.
Otherwise, the system still works without grammar rewriting.

FILE OVERVIEW
- AdvancedSpellCheck.py  : Core spell + context engine
- app.py / LexiFix.py    : Gradio web UI
- requirements.txt       : Dependencies
- INSTALL.txt            : Basic setup instructions

LICENSE
Provided for educational use. Models belong to original authors.
