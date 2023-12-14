</br>

# Training Chatbot

The Saint James Team chatbot, or ChatSJT, was designed to answer the questions of new staff by combining the general intelligence of ChatGPT with the hostel's 57 page operations manual. This helps facilitate the onboarding of new employees and volunteers in a hostel with a high staff turnover. The bot works through the following steps:

</br>

>  **1) Splits**  
>     A basic algorithm is applied to find the most appropriate split points in the operations manual (~100)
> 
>  **2) Summarization**  
>     Any chunks over 200 words are shortened to a maximum not exceeding this length through a ChatGPT API call
> 
>  **3) Edits**  
>     Iterative textual edits are made to a saved csv of the resulting chunks to improve the bot's answers
> 
>  **4) Embeddings**  
>     The embeddings, numbers describing the meaning of words in relation to others, for each chunk are obtained from OpenAI
> 
>  **5) Retrieval**    
>     The bot is instructed to vectorize any question asked of it and find the chunk with the the most similar embeddings
> 
>  **6) Context**  
>     The bot then feeds the question, the text of the most relevant chunk and several other cues into ChatGPT for a response
