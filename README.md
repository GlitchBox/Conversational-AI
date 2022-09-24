# Conversational-AI
I have been experimenting with OpenAI's GPT model to create a conversational AI. I trained the model on conversations extracted from Facebook Messenger. I have yet to experiment with the more potent GPT-2 model. 
There are memory constraints when you use the free version of golab and GPT is much lighter. 

I have been following along this work (https://arxiv.org/abs/1901.08149) and its illustrated version on this (https://medium.com/huggingface/how-to-build-a-state-of-the-art-conversational-ai-with-transfer-learning-2d818ac26313) blog. They created the conversational agent a personality. According to their setup, several sentences would determine the personality of an agent. The agent would be trained on dataset of dialogues and personality sentences.

I wanted my agent to assume the personality of a certain friend of mine. Therefore I didnot model my system exactly like theirs. I had no use for personality sentences. Rather, the model should learn how my friend texts from the dataset. Furthermore, the model checkpoint (HuggingFace) used here is pretrained on English sentences. Being Bangladeshis, more often than not we text in **Banglish** alongside English or plain Bengali. **Banglish** is Bengali written with English letters. I wanted to see if the model could learn Banglish from whatever dataset I had to offer. 

My first attempt involved 900 conversations in the dataset. As expected, the model didnot learn much from such a tiny dataset. The model did spit out Banglish words in response to my texts. But they were incoherent and honestly didnot make any sense. 
![output_text png](https://user-images.githubusercontent.com/34965899/192083327-cdc5ce64-f1e4-497b-9e6f-c2320f4f8dc7.png)


I will be training with larger dataset soon and report back once I work this out.
