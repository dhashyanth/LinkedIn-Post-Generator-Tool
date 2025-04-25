# LinkedIn-Post-Generator-Tool 🚀

This end-to-end Generative AI project focuses on building a LinkedIn Post Generator Tool that transforms raw content ideas into engaging, professional posts. The solution leverages the power of the LLaMA 3.2 open-source large language model (LLM), deployed via Streamlit for an interactive user interface, and accelerated using Groq Cloud for high-performance inference.

The tool is designed to streamline the content creation process for professionals, marketers, and thought leaders, enabling them to effortlessly generate tailored LinkedIn posts based on user-defined inputs such as topic, language, and length.



---

## 💡 Overview

The **LinkedIn-Post-Generator-Tool** transforms your initial thoughts or raw drafts into structured, well-written LinkedIn posts using LLMs in a staged process. It allows customization by **topic**, **language**, and **length**, ensuring the generated content aligns with your professional voice and target audience.

---

## 🛠️ How It Works

The tool operates in **two main stages**, leveraging few-shot learning and prompt engineering techniques.

### 🔐 API Key Configuration

Before running the tool, ensure your **Groq Cloud API key** is configured:

```bash
export GROQ_API_KEY="your_api_key_here"
```

Or place it in a `.env` file:

```
GROQ_API_KEY=your_api_key_here
```

---

## 🔄 Pipeline Breakdown

### 🧪 Stage 1: Preprocessing & Enrichment

1. **Input**: Raw, unstructured post ideas or text snippets.
2. **Preprocessing**: Clean and normalize input using LLaMA 3.2 (token filtering, correction, grammar cleanup).
3. **Enrichment**: Add metadata such as:
   - **Topic**: e.g., AI, career tips, startup journey
   - **Language**: English, French, etc.
   - **Length**: Short, medium, long

> 🧠 This stage ensures the model understands context, tone, and intent.

---

### ✨ Stage 2: Prompt Engineering & Post Generation

1. **Input**: Enriched metadata (topic, language, length)
2. **Prompt Generation**: Uses few-shot learning to dynamically craft prompts suitable for LinkedIn formatting and tone.
3. **Post Generation**: Final post is generated using LLaMA 3.2 with the custom prompt.
4. **Output**: A fully formatted, platform-optimized LinkedIn post ready to publish.

---

## 📦 Output Example

**Input** (Raw):  
> "AI in workplace future"

**Enriched**:  
Topic: AI  
Language: English  
Length: Medium

**Output** (Final Post):  
> The future of work is being shaped by AI, not in the distant future—but right now. From automating tasks to personalizing learning experiences, AI is revolutionizing how we operate. Are you ready to adapt and lead in the age of intelligent transformation?

---

## 🚀 Future Plans

- Add support for scheduling LinkedIn posts
- UI for non-technical users
- Additional tone/style customization (formal, witty, inspirational)
