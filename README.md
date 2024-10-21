LLM - Large Language Model. ( this page is under construction :-))

**For whom.**

For some reason you don't want to work with open or commercial LLMs. And you don't want to understand the areas that tell you how to build a LLM yourself. Then this corner of the Internet is for you. It's not that complicated. First, let's look at a ready-made LLM, it is intentionally made very, very, very simple.

**To start**

1. **Copy llm.zip** to the folder you selected on your computer.
2. **Unzip archive.**
3. **LLM training.**
   
We perform LLM training on ready-made data, this is a very important part of your work. The data set for training is in the textbook folder in the form of text files that simulate arithmetic operations from 0 + 0 = 0 to 9 + 9 = 18 in the format of numbers and words. The format of the records can be viewed by opening any file from the textbook folder in your editor. For llm training, go to the builder folder, launch the console in the folder and type in the console: llm.exe -td 1. The data.txt file should appear in the brains folder, which contains the data on the basis of which llm will communicate with you.

A bit of explanation. The -td 1 parameter is an abbreviation for ToDo, and 1 indicates that llm should take files from textbook and create data for itself in the brains folder.

4.**Working with LLM.**
   
While in the same folder, type: llm.exe -td 2, which means for llm that it needs to enter to the conversation mode with the user.

llm gives an invitation to start communication, below is the sample of the dialogue of your communication with llm through the console:

user:->1+1=<**enter**>

llm: typed 1+1

llm: result: =3

user:2+2=<**enter**>

llm:result:4

2+u=<**enter**>

llm:error:word u could not be evaluated

Explanations. Yes, you (under my supervision) made a mistake - it happens. Now we are going to correct it.

user:2+8=<**enter**>

llm:result:10

Now you can test llm's work with words, not just numbers.

user: nil plus nil equals <**enter**>

llm: result nil

user: eight plus eight equals<**enter**>

llm: result:sixteen

5. **Setting up llm operation using the config.json file**
   
You have 2 parameters available:

**evaluator_type** and **chatter_type**.

**evaluator_type** has two options:

⦁	simple - returns the next available word in order.

⦁	random - returns a word chosen randomly from possible ones.

**chatter_type** has two options:

⦁	completer - llm completes the sentence you typed.

⦁	teller - "tries" to maintain a "conversation" with you by choosing the last word of the previous sentence to begin a new one.

6. Well, now you know everything to create data for setting up your own llm. It's up to you. Experiment as you wish. And it's all Free of charge.
    
7. **Memo**. The program is written in Go for Windows 10, there is no multithreading, the data for llm is located all in RAM. There is a plan for its further development.
   
8. If you find any **error** and wish to send me a description, please provide a set of data where possible to reproduce the bug. I will say thank you.
   
9. In case there is a **modification** you need, drop me a message.

