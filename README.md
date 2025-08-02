# 🗣️ Dialogue Summarizer

**Dialogue Summarizer** is a conversational summarization system built using the **BART** transformer model. It is fine-tuned on the [SAMSum dataset](https://huggingface.co/datasets/samsum) to condense informal dialogues into concise and informative summaries, helping users quickly grasp the essence of lengthy conversations.

---

## 📌 Project Overview

- 📚 **Model:** BART (Bidirectional and Auto-Regressive Transformers)  
- 🧠 **Dataset:** SAMSum — a dataset containing real-world chat-like dialogues and their human-written summaries  
- 🔍 **Purpose:** Automatically generate concise summaries from multi-turn conversations in messaging/chat formats

---

## 📊 Performance Metrics

| Metric         | Score |
|----------------|-------|
| ROUGE-1 F1     | 0.54  |
| ROUGE-L F1     | 0.44  |

- **ROUGE-1 F1**: High unigram overlap with reference summaries  
- **ROUGE-L F1**: Good ability to capture the longest common subsequence

---

## 💡 Example

### 🔹 Sample Dialogue
```text
Alice: Hi Bob, I'm interested in the new smartphone you have on sale. Can you tell me more about its features?

Bob: Absolutely, Alice. The new smartphone has a 6.7-inch display, 128GB storage, and a 48MP camera. It also supports 5G and comes with a long-lasting battery.

Alice: That sounds great. Does it come with any warranty?

Bob: Yes, it comes with a one-year manufacturer's warranty that covers any defects.

Alice: Perfect. Can you also tell me about the return policy?

Bob: Sure. We have a 30-day return policy, so if you're not satisfied, you can return the phone within 30 days for a full refund.

Alice: Thanks, Bob. I think I'll go ahead and purchase it.
'''
## ✅ Generated Summary
Alice is interested in the new smartphone Bob has for sale. The new smartphone has a 6.7-inch display, 128GB storage, and a 48MP camera. It also supports 5G and comes with a long-lasting battery. It has a one-year manufacturer's warranty and a 30-day return policy.
```

## 🛠️ Tech Stack
Model: BART (via Hugging Face Transformers)
Dataset: SAMSum
Language: Python
Frameworks & Libraries: PyTorch
Hugging Face Transformers
Datasets (from Hugging Face)
ROUGE metrics
