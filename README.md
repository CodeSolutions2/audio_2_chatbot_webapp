# audio_2_chatbot_webapp

A combination of steps from [audio_2_text_webapp](https://github.com/CodeSolutions2/audio_2_text_webapp) and [text_2_chatbot_webapp](https://github.com/CodeSolutions2/text_2_chatbot_webapp) to make one end-to-end process. (**in progress**)

Using the transcription models created in [audio_2_text_webapp](https://github.com/CodeSolutions2/audio_2_text_webapp), transcribed text is added to a text log file. The text log file is used to train a chatbot (at the moment: OpenAI GPT) using Retrieval Augmented Generation (RAG):

Retreival step:
1. Text log file sentences are converted to embedding vectors and vectors are stored on a vector database
2. User question is converted to an embedding vector
3. Relevant information related to the user's question in the log file is found using cosine similarity

Generation step:

4. Chatbot is fine-tuned with relevant information only
5. Chatbot responds to user question and highlights/returns log file sentences that support the response. 


## Upwork
[Available for purchase on Upwork](https://www.upwork.com/services/product/development-it-audio-transcription-chatbot-using-q-a-finetuning-1783550902752177813)
