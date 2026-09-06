<div align="center">

# Omar Mohsen

### AI Engineer · Qena, Egypt

I build the layer between models and the people using them — orchestration, routing, evaluation,<br>and the decisions about where a model *shouldn't* be used at all.

B.Sc. Computer Science and Artificial Intelligence, South Valley National University · 2026

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aidevomarmohsen/)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/omar1mohsen)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:omar1mohsen23@gmail.com)

</div>

---

## Projects

### [Sanad · سند](https://github.com/Omar-Mohsen22/sanad) — AI support companion for autistic users

> Built to help, never to diagnose.

I built the **entire AI orchestration layer**: a 38-node n8n workflow — one webhook in, three routed pipelines, multimodal input detection (text / audio / image), intent classification, and stateful memory in Supabase.

<div align="center">
<img src="https://raw.githubusercontent.com/Omar-Mohsen22/sanad/main/docs/architecture/workflow-canvas.png" width="820">
<br><em>The full 38-node workflow on the n8n canvas</em>
</div>

<table>
<tr>
<td width="50%" valign="top">

**Design decisions I'd defend**

The self-assessment is scored in **deterministic JavaScript, not an LLM** — a user's profile has to be reproducible, and language models are the wrong tool where consistency beats fluency.

When an upstream API fails, the recommendation node **falls back to an embedded set instead of erroring**. A user in distress must never hit a blank screen.

System prompts **hard-block diagnostic language**; crisis responses are scripted, not generated.

</td>
<td width="50%" valign="top">

<div align="center">
<img src="https://raw.githubusercontent.com/Omar-Mohsen22/sanad/main/docs/app/06-ai-chat.png" width="200">
<br><em>Multimodal chat — text, voice, image</em>
</div>

</td>
</tr>
</table>

`n8n` · `LangChain` · `OpenRouter (Qwen)` · `ElevenLabs` · `Supabase` · `Docker`

<sub>Team graduation project — teammates built the Flutter app and Django backend.</sub>

---

### [Diabetes Risk Prediction](https://github.com/Omar-Mohsen22/diabetes-risk-prediction-genetic-algorithm) — genetic algorithm vs. randomised search

A screening classifier on CDC BRFSS survey data — **98,527 records**, 21 indicators, ~15% positive class.

|  | Result |
|---|---|
| **Recall** | 16% → **85.5%** after threshold tuning (0.4) |
| **Precision** | 27.4% — accepted deliberately |
| **GA vs. randomised search** | +0.5% F1, at **4× the compute** |

Optimised for recall over accuracy, because a missed case costs more than a false alarm. The genetic-algorithm result is reported as what it was: a marginal gain, not a headline.

`scikit-learn` · `XGBoost` · `HistGradientBoosting` · `sklearn-genetic-opt` · `Gradio`

---

### [Gemma 3 ML Tutor](https://github.com/Omar-Mohsen22/gemma3-ml-tutor-chatbot) — LoRA fine-tuning

Fine-tuned `google/gemma-3-1b-it` into a machine learning teaching assistant.

**PEFT LoRA** (r=8, α=16) on the query and value attention projections — **745,472 trainable parameters, 0.075% of the model**. bfloat16 with gradient accumulation on a single consumer GPU, adapter merge, Gradio chat interface. A 1B model chosen deliberately over reaching for the largest available.

`PyTorch` · `Hugging Face Transformers` · `PEFT` · `Gradio`

---

## Stack

| | |
|---|---|
| **Languages** | Python · C++ · SQL · JavaScript |
| **ML / DL** | PyTorch · TensorFlow · scikit-learn · XGBoost · Hugging Face · PEFT/LoRA |
| **AI systems** | n8n · LangChain · OpenRouter · OpenAI API · Gradio |
| **Data** | pandas · NumPy · Matplotlib · Seaborn · Power BI |
| **Infra** | Docker · Supabase (PostgreSQL) · MongoDB · FastAPI · Nginx · Git |

---

## Currently

Working through **LangChain for LLM Application Development** and **Intermediate SQL**.

Completed the **Machine Learning Specialization** (Stanford / DeepLearning.AI) and the **NTI / Huawei Egyptian Talent Academy** AI track — 80 hours, scored 100%.

**Open to remote AI engineering work** — omar1mohsen23@gmail.com
