# NLP-model-task3

Approach: In this task, I have tokenized the Pargraph and queries using TfidVectorizer. Then for finding the top 5 relevant paragraph to the queries , i used the cosine_similarity function which gives maximum value 
for the most similar query and paragraph.Thus By sorting the array ,I got from using cosine_similarity for each query with all paragraphs vector , I got the last 5 elements for the array as the 5 most relevant 
paragraphs for the query.Then I used a hugging face transformer from which i used "question-answering" pipeline which uses distilbert-base-cased-distilled-squad model for answering to a query based on the 5 most 
relevant paragraphs. 
Additionally , I implemented Gradio frontend which takes query as input and gives the answer as output.
