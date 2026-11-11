# ⚖️ LegisAI – AI-Powered Court Hearing Preparation Tool

LegisAI is a generative AI assistant that helps Indian lawyers prepare for court hearings. Enter the facts of a case, the key evidence and which side you represent, and LegisAI drafts the material you need for the hearing — then exports it all as a single Word report.

Built with **Python, Streamlit and Google Gemini 1.5 Flash**. In testing it reduced hearing-prep drafting time by about **60%**.

<p align="center">

![LegisAI interface](https://github.com/user-attachments/assets/45beedb4-1b6b-49c8-b95a-d0fb9b63b7cf)

![LegisAI generated output](https://github.com/user-attachments/assets/2ab1b9b5-3f3d-46f5-a77c-e190ee540931)
</p>

## ✨ What it generates

| Feature | Output |
| --- | --- |
| 📄 Case summary | Concise summary of the facts and issues |
| ⚖️ Legal arguments | Arguments for the side you represent |
| ❓ Legal questions | Key questions the court is likely to consider |
| 👥 Witness & evidence | How to use witnesses and evidence |
| 🧾 Examination & cross | Examination-in-chief and cross-examination questions |
| 🛡️ Opponent counter questions | Questions the other side may raise, with responses |
| 🔍 Similar cases | Related precedents to research |
| 📚 Applicable laws & sections | Relevant IPC / CrPC and other sections |
| 📥 Full report | Everything above exported as a `.docx` file |

## 🛠️ Tech stack

- **Frontend / app:** Streamlit
- **LLM:** Google Gemini 1.5 Flash (`google-generativeai`)
- **Export:** `python-docx`

## 🚀 Run locally

```bash
git clone https://github.com/Devraj8068/LegisAI-Court-Hearing-AI-Powered-Preparation-Tool.git
cd LegisAI-Court-Hearing-AI-Powered-Preparation-Tool

python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt

cp .env.example .env            # then add your Gemini API key to .env
streamlit run app.py
```

Get a Gemini API key from [Google AI Studio](https://aistudio.google.com/app/apikey). The key is read from the `GEMINI_API_KEY` environment variable — never commit it.

## ⚠️ Disclaimer

LegisAI produces AI-generated drafts to support preparation. It is not legal advice; always verify citations and arguments before using them in court.
