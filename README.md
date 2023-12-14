# ChatSJT

The Saint James Team bot, or ChatSJT, was designed to answer the questions of new staff by combining the general intelligence of ChatGPT with the hostel's 57 page operations manual. This helps facilitate the onboarding of new employees and volunteers in a hostel with a particularly high staff turnover. The bot works via the following steps:

</br>

>  **1) Splits**  
>     A basic algorithm is applied to find the most appropriate split points in the manual (~100)
> 
>  **2) Summarization**  
>     Any chunks deemed too long are shortened to 200 words with an API call to ChatGPT
> 
>  **3) Edits**  
>     Iterative edits are made to a saved version of the text to improve the bot's performance
> 
>  **4) Embeddings**  
>     The embeddings for each chunk are obtained from OpenAI and stored along with the original text
> 
>  **5) Retrieval**    
>     The bot is instructed to vectorize any question and search for the most similar chunk's embeddings
> 
>  **6) Context**  
>     It is then told to feed the question text and that of the most relevant chunk into ChatGPT as context
