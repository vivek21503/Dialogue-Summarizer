## Dialogue Summarizer

This project implements a dialogue summarizer built upon the BART model, fine-tuned using the SAMSUM dataset ([link to SAMSUM dataset](https://huggingface.co/datasets/samsum)). 
It effectively condenses conversations into concise summaries, making it easier to grasp the key points of lengthy dialogues.

**Performance:**

* Average ROUGE-1 F1 Score: 0.54 (Strong unigram overlap with reference summaries)
* Average ROUGE-L F1 Score: 0.44 (Good ability to capture longest common subsequences)
  
**Sample Dialogue**

dialogue = 
"""
Alice: Hi Bob, I'm interested in the new smartphone you have on sale. Can you tell me more about its features?

Bob: Absolutely, Alice. The new smartphone has a 6.7-inch display, 128GB storage, and a 48MP camera. It also
     supports 5G and comes with a long-lasting battery.

Alice: That sounds great. Does it come with any warranty?

Bob: Yes, it comes with a one-year manufacturer's warranty that covers any defects.

Alice: Perfect. Can you also tell me about the return policy?

Bob: Sure. We have a 30-day return policy, so if you're not satisfied, you can return the phone within 30 days
     for a full refund.

Alice: Thanks, Bob. I think I'll go ahead and purchase it.
"""

**'summary_text':**

Alice is interested in the new smartphone Bob has on sale. The new smartphone has a 6.7-inch display, 128GB storage,
and a 48MP camera. It also supports 5G and comes with a long-lasting battery. It has a one-year manufacturer's warranty
and a 30-day return policy.


