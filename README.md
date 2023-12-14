# ChatSJT

The Saint James Team training chatbot, or ChatSJT, was designed to answer the questions of new staff by combining the general intelligence of ChatGPT with the hostel's 57 page operations manual. This helps to facilitate the onboarding of new employees and volunteers in a hostel with a particularly high staff turnover. The bot works via the following steps:

</br>

>  **1) Splits**  
>     A basic algorithm was applied to find the most appropriate split points in the text (~100)
> 
>  **2) Summarization**  
>     Any chunks deemed too long were shortened to 200 words with an OpenAI call to ChatGPT
> 
>  **3) Edits**  
>     Iterative edits were made to the resulting text to improve the chatbot's performance
> 
>  **4) Embeddings**  
>     The embeddings for each chunk were then obtained from OpenAI and stored along with the original text
> 
>  **5) Retrieval**    
>     When asked a question, the bot is instructed to vectorize it and search for the most similar chunk
> 
>  **6) Context**  
>     Following this, the question text and that of the relevant chunk is fed into ChatGPT as context
