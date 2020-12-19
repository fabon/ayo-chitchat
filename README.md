# AYO-orchestration

- Alternate between a Fashion chit-chat model and a FAQ replies bot
- Implement an intent dispatcher between query type and non query type messages
- Create conversation scenarios to maintain an engaging flow (e.g greetings, chit-chat, diagnosis, goodbyes)

# AYO-chitchat

Fine-tune an engaging chit-chat dialog system for Fashion using extracts from the Social Media and examples of Customer conversations.

- Set up an env to access your GPU machine
- Install ParlAI
- Download and run Blender 2.7B + Safety net for toxic language
- Chat with Blender
- Fine-tune the model (ParlAI tutorial: https://colab.research.google.com/drive/1bRMvN0lGXaTF5fuTidgvlAl-Lb41F7AD#scrollTo=KtVz5dCUmFkN)
- Download Reedit Fashion conversations - https://www.reddit.com/r/femalefashionadvice/ and https://www.reddit.com/r/malefashionadvice/ use the Reedit API https://www.reddit.com/dev/api/
- Download ASOS conversaitons - link here
- Deploy the model on a conversational channel

# AYO-FAQ-replies

Fine-tune a pre-trained BERT model to solve a qa task on our FAQ self serve content.
1. as a first step, learn to map a user question to a faq question entry,
1. then learn to map a user question to a faq reply sub-section,
1. finally, make the solution robust by augmenting the set of training data with synthetic and user conversations data

Data annotation: create an env to collect data from a user interacting with a baseline version of the bot
                 the prompt will ask confirmation of the correct classification to the user, given a choice of 
                 the top 3 highest ranked responses

Start with annotating a set of 100 user questions to train a baseline method,
then collect use the interactive prompt to scale up the training set to ~1K user queries.

Experiment with synthetic data generation algos/methods to improve the final accuracy,
share an early demo to collect real examples of user inputs.



