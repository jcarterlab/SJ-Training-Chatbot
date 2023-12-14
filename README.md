# SJ-Training-Chatbot

The Saint James Team training chatbot, or ChatSJT, was designed to answer the questions of new staff by combining the general intelligence of ChatGPT with the hostel's 57 page operations manual. This helps to facilitate the onboarding of new employees and volunteers in a hostel with a particularly high staff turnover. The following steps were taken to build this app:

>  **1) Splits** - a basic algorithm was applied to try and find the most appropriate split points (~100)  
>  **2) Summarization** - chuncks that were deemed too long were shortened to 200 words with an OpenAI call  
>  **3) Edits** - iterative edits were made to a saved version of the text to improve the chatbot's performance  
>  **4) Embeddings** - the embeddings for each chunk were obtained from OpenAI and stored with the original text  
>  **5) Retrieval** - the bot vectorizes a given question and identifies the chunk with the most similar embeddings  
>  **6) Context** - the question and the selected chunk is then fed into ChatGPT as context through which to answer  

