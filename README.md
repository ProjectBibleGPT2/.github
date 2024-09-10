1. Why? Why won’t we just fine-tune ChatGPT?
   a) Because fine-tuning is just fine-TUNING, tuning is only a fine (or relatively small) change in parameters. For example, if tuning GPT2 on Spanish, one can still make it speak English by tricking it, since the base parameters trained on English is still present in the parameters.
   b) By training from scratch GPT2, we can create strong base parameters around the Bible, then we can finetune it for Q&A using Theology Q&A files or books.

2. The step and meaning of the step used to create the project?
   a) Training on GPT2
      i. GPT2, being one of the first transformer architectures to be trained for text generation, it is simple, small, yet effective for basic level experimentations before using a larger model for more accurate results.
   b) Using various different Bible Versions
      i. By first starting with word for word translations, we establish words’ relationship with other words in the Bible in GPT2.
      ii. Then, by moving more to thought for thought, we introduce new vocabulary and introduce the idea of thought, while including the earlier versions as a validation dataset.
      iii. However, we do not use Paraphrase, since paraphrase means to state the text with one’s own words. Therefore, paraphrased Bibles are not really the “word” of God.
      
      *Image to insert*

   c) (BETA) Try using Isopsephy
      i. Isopsephy is giving each Ancient Greek/Hebrew letter a number (as denoted in the picture)
      
      *Image1 to insert*
      
      ii. If given a text and up all the words in the text, and find another text with the same sum, it means that the two texts are similar or have a similar aspect or overall meaning.
      
      *Image2 to insert*
      
      iii. Still researching on this topic. Will write a research topic that explores “Can Isopsephy enhance AI understanding of context?”
   d) RAG
      i. Using added context to further improve the performance and accuracy of the model.
   e) Using Q&A Datasets
      i. By using Q&A Theology Books and files, we can fine-tune the model to answer our questions.
      ii. For example, the Q&A book can be like:
         Q: What is God?
         A: …
