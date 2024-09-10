### TODO List:
##### Training on GPT2 
- [ ] in progress
###### GPT2, being one of the first transformer architectures to be trained for text generation, it is simple, small, yet effective for basic level experimentations before using a larger model for more accurate results.
##### Using various different Bible Versions
- [ ] in progress
###### By first starting with word for word translations, we establish words’ relationship with other words in the Bible in GPT2.
###### Then, by moving more to thought for thought, we introduce new vocabulary and introduce the idea of thought, while including the earlier versions as a validation dataset.
###### However, we do not use Paraphrase, since paraphrase means to state the text with one’s own words. Therefore, paraphrased Bibles are not really the “word” of God.

*Image to insert*

##### (BETA) Try using Isopsephy
- [ ] in progress
###### Isopsephy is giving each Ancient Greek/Hebrew letter a number (as denoted in the picture)

*Image1 to insert*

###### If given a text and up all the words in the text, and find another text with the same sum, it means that the two texts are similar or have a similar aspect or overall meaning.

*Image2 to insert*

###### Still researching on this topic. Will write a research topic that explores “Can Isopsephy enhance AI understanding of context?”
##### RAG
- [ ] in progress
###### Using added context to further improve the performance and accuracy of the model.
##### Using Q&A Datasets
- [ ] in progress
###### By using Q&A Theology Books and files, we can fine-tune the model to answer our questions.
###### For example, the Q&A book can be like:
```
Q: What is God?

 A: …

 Q: Who is Jesus?

 A:…

 …
```
###### Where <|endoftext|> states that GPT2 has finished his answer.
###### If we want to ask: What is God’s relationship with human? We input the following prompt to GPT2.

```
Q: What is God’s relationship with human?

A:
```

###### GPT2, standing for Generative Pretrained Transformers will try to generate the next word according to the context its give (in this case, it is:

```
Q: What is God’s relationship with human?

A:
```
###### ), and update it to the context (the context after a update will be:

```
Q: What is God’s relationship with human?
A: God’s)
```

###### GPT2 then proceed to generate one more word on the updated context and add it to the new updated context, and then continue again until a special token (e.g. <|endoftext|>) is generated, meaning that GPT2 has finished generating.

