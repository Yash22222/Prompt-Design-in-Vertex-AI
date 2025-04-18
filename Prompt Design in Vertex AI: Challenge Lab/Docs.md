# 🧪 Prompt Design in Vertex AI: Challenge Lab

```markdown
This lab is designed to test your understanding of prompt engineering using the tools provided in Google Cloud's Vertex AI, specifically focusing on **text generation** and **Gemini/PaLM models**.
  ```
---

## 🎯 Objectives

- ✅ Access Vertex AI Studio
- ✅ Create and refine effective prompts
- ✅ Use temperature, top-p, and max token controls
- ✅ Apply few-shot learning techniques
- ✅ Interpret outputs for quality and relevance

---

## 🔧 Step-by-Step Lab Instructions

### 1️⃣ Launch Vertex AI Studio

- Go to: [Vertex AI Studio](https://makersuite.google.com/app)  
- Or via: [https://console.cloud.google.com/vertex-ai/prompt-studio](https://console.cloud.google.com/vertex-ai/prompt-studio)

---

### 2️⃣ Create a New Prompt

Choose **Text Prompting** and write your first prompt:

```text
Generate 3 bullet points summarizing the advantages of using AI in customer support.
```

Then experiment with:

- 🔥 **Temperature** (0.2 for factual, 0.8 for creativity)
- 🔢 **Top-k** and **Top-p**
- ✏️ **Max Output Tokens**

---

### 3️⃣ Apply Prompt Best Practices

Refine your prompt using best practices:

- Add **context**:  
  ```text
  You are a technical content writer. Write a paragraph on why prompt design matters in AI.
  ```

- Specify **output format**:  
  ```text
  List key benefits of prompt engineering as bullet points.
  ```

- Use **few-shot examples**:
  ```text
  Input: "Summarize importance of ML in finance"  
  Output:  
  - Detects fraud  
  - Enables credit scoring  
  - Improves trading strategies  

  Input: "Summarize benefits of AI in marketing"  
  Output:
  ```

---

### 4️⃣ Analyze & Iterate

Observe:
- Relevance of response
- Fluency and factual accuracy
- Output consistency across trials

Keep iterating and improving the prompt design for better control and results.

---

## 🧠 Tips for Prompt Design

- ✅ Start simple, then layer complexity
- ✅ Specify role, tone, and format
- ✅ Use few-shot when appropriate
- ✅ Evaluate and revise based on response behavior

---

## 🏁 Completion Criteria

- [ ] Successfully create and run at least 3 distinct prompts
- [ ] Use and modify generation settings (temperature, tokens)
- [ ] Apply at least one few-shot example
- [ ] Reflect on outputs and document findings

---

## 📚 Helpful Resources

- [Prompt Design Guide (Google)](https://cloud.google.com/vertex-ai/docs/generative-ai/text/prompt-design)
- [Vertex AI Studio Overview](https://cloud.google.com/vertex-ai/docs/generative-ai/learn/overview)
- [Prompt Engineering 101 (Google Developers)](https://developers.google.com/machine-learning/prompt-design)

---

## 📦 Bonus Challenge

Try this advanced prompt:

```text
Act as a data analyst and generate a 5-bullet executive summary of a fictional e-commerce company’s performance using this data: Revenue ↑12%, Conversion Rate ↑2.3%, Cart Abandonment ↓10%, Ad ROI ↑1.8x, Churn Rate ↓1.1%.
```

Can you improve the prompt to make the summary more executive-focused? 🎯

---

> 🧑‍💻 Ready to level up? Try exporting your prompt to Python using the Vertex AI SDK and integrate it into a Flask app!
```

