

```markdown
# Generative AI with Vertex AI: Prompt Design

## 🔍 What is Vertex AI?

**Vertex AI** is Google Cloud’s managed platform for developing and deploying machine learning (ML) models. It supports a wide range of tools, including **generative AI models** like **PaLM 2**, **Gemini**, and **Codey** for tasks such as text generation, code generation, and more.

---

## 🧠 What is Prompt Design?

**Prompt Design** is the technique of crafting inputs (prompts) that produce high-quality outputs from large language models (LLMs). Effective prompt design involves:

- Giving clear and specific instructions
- Including few-shot examples if needed
- Using a structured format
- Asking direct and targeted questions

---

## 🧪 Prompt Examples

### 🔹 Zero-shot Prompt

```
Summarize the following article in 3 bullet points: [Paste Article Here]
```

---

### 🔹 Few-shot Prompt

```
Q: What is the capital of France?
A: Paris
Q: What is the capital of Germany?
A: Berlin
Q: What is the capital of Italy?
A:
```

---

### 🔹 Instruction-based Prompt

```
You are an expert in marketing. Write a product description for a smartwatch in under 50 words.
```

---

## 🛠️ Tools for Prompt Design in Vertex AI

- **Model Garden** – Select and test pre-trained LLMs
- **Prompt Design Studio** – Interactive UI for testing prompts
- **Python SDK (`vertexai`)** – Automate prompt testing and model usage

---

## ✅ Working Python Code Using Vertex AI

Make sure you have the required package:

```bash
pip install google-cloud-aiplatform
```

Here’s a sample Python script to use **Vertex AI** for prompt design:

```python
from vertexai.preview.language_models import TextGenerationModel
import vertexai

# Initialize Vertex AI
vertexai.init(project="your-gcp-project-id", location="us-central1")

# Load the model (text-bison or other supported models)
model = TextGenerationModel.from_pretrained("text-bison@001")

# Define a prompt
prompt = "Write a professional summary of a fresher data analyst looking for a job in Mumbai."

# Generate response
response = model.predict(
    prompt,
    temperature=0.7,
    max_output_tokens=256,
    top_k=40,
    top_p=0.8,
)

print(response.text)
```

---

## 🔐 Notes

- Replace `your-gcp-project-id` with your actual GCP project ID.
- Make sure **Vertex AI API** is enabled on Google Cloud.
- You can run this code in a **Vertex AI Notebook** or **Google Colab** (with GCP auth).

---

