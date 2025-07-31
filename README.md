# Task

I will be working with the BERT model.
The goal of this task is to get familiar with the model using a Question Answering example. To do this, you need to:

Install the required packages

Create a file called q&a.py containing your code

Load a pre-trained BERT model

Set a context — a text passage in which the model will search for answers to the user’s questions

Implement a bot that receives a string (the question), sends it to the model, and then prints the answer to the screen

To build such a bot using BERT, we will use the Transformers library from Hugging Face and the Flask framework to create a web application.
This bot will process user queries and respond using the BERT model.

A specific BERT model should be selected based on the task type.
In this case, we will use BertForQuestionAnswering, which includes the necessary architecture and a head suitable for the Question Answering task.

After running the code, the address of the web page will be displayed. By following the link, you should see a working web interface.

As context (paragraph), we will use the book "Alice in Wonderland", which is in English, since the model was trained in that language.

To test the model, you can try the following questions:

"Who did Alice follow down the rabbit hole?"

"What did Alice see as she was falling down the well?"

"How did Alice manage to shrink in size?"


<img width="1443" height="545" alt="изображение" src="https://github.com/user-attachments/assets/0602f2f1-63e5-4ec6-9db7-f8ff1c50736c" />



# Summary:

The code implements a complete Question Answering system based on BERT, allowing users to ask questions about Alice in Wonderland through a simple Gradio web interface.

It includes:

Loading the pre-trained bert-large-uncased model (fine-tuned on SQuAD)

Splitting the text into 400-token chunks (to stay within BERT’s 512-token limit)

Searching for the most likely span containing the answer

Displaying the result to the user through a Gradio web interface
