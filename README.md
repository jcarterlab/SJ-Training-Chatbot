</br>

# Training Chatbot

The Saint James Backpackers chatbot, or ChatSJB, was designed to answer new staff questions by combining the intelligence of ChatGPT with the hostel's 57 page operations manual. This better facilitates the onboarding of new employees and volunteers in an establishment with a high level of staff turnover. The text for this project can be added to over time and even expanded to cover guest queries. The bot is constructed via the following steps:  

</br>

> **1) Splits**  
> A basic algorithm is applied to try and find appropriate split points in the operations manual (~100)

> **2) Summarization**  
> Any chunks over 200 words are shortened to a maximum length not exceeding this through a ChatGPT API call

> **3) Edits**  
> Iterative edits are made to a saved version of of the text (.csv) to improve the bot's answers

> **4) Embeddings**  
> The embeddings (numbers describing the meaning of words) for each chunk are obtained from OpenAI

> **5) Retrieval**    
> The bot obtains the embeddings for any given question and uses them to find the the most similar chunk

> **6) Context**  
> The bot then feeds the question, the text of the most relevant chunk and several other cues into ChatGPT for a response  

</br>
</br>

The notebook can be found [here.](Save-Embeddings.ipynb)

<br/>
