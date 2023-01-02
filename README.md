## Python Word counting in 2022 Whatsapp Chat 2️⃣0️⃣2️⃣2️⃣
2022 has finished and as a way of summarizing the best moments with my friends I developed something to get some laughs. My best friend and I are used to chat a lot since classes at College are given online. And this year isn't an exception.

### Downloading data and creating dataframe
____________________________________________
First, I want to clarify that I am using this information with the permission of my best friend. Okay, let's see how I downloaded it. We are going to need out phone and a group called "me" (or any chat, it doesn't matter). To download chat data I had to follow the next steps: Settings > Chats > Chats Record > Export chat > Select the chat you want to export.

Then, with all the data, a for loop was ran so all the words were saved into an empty dictionary. Then the dictionary was converted to a pandas dataframe using pd.Dataframe(words.keys()). 

### Cleaning 🧹🧹
__________________
Now, we have to prepare the data. When the file is open, you will see that each message is composed by date and hour data. This is useful data, but not in this case since we just want messages(it would be useful to identify trends throughout the year 📶). 
#### How to clean it
There are multiple ways, in this case I used simple regular expressions and re.search or re.fullmatch method. You can see it in the code file within the repository. I had to clean a lot of words like prepositions or symbols like -. 

### Plotting 〽️🔄️
___________________
Using seaborn and sorting the top 15 words we used, I just plotted frecuency vs words. This was the result: 
![BarChart_Whatsapp Chat](https://user-images.githubusercontent.com/101015892/210257588-3f90e54c-81bc-46bc-a80a-767ea0333761.png)
_Note: this words are in spanish since that is our native language_.

As you see, but is our preferred word, classes are our daily bread and we laugh a lot (JAJA). Now let's see the emojis. In this case, seaborn does not recognize emojis in the x axis so I had to do a little table with all the emojis. I had to add an extra clean step so the words would be removed. 

![image](https://user-images.githubusercontent.com/101015892/210258264-2be3b724-9699-4ce3-897e-d2b69a5e3b8f.png)

As we see, here are the top 10 emojis of 2022 with my best friend. We were so surprised to see that 🤡 was mentioned just 26 times this year. We thought we used it like a thousand times. 

_____________________________________________________________
That is how you make a wrap up of you and your friend's year.
_____________________________________________________________
