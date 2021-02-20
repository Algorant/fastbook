- [[Ch 2 Questions]]
    1. Provide an example of where the bear [[classification]] model might work
 poorly in production, due to structural or style differences in the 
[[training data]].
        - **I could not find this exact answer in the notebook.**
    2. Where do text models currently have a major deficiency?
        - **They currently cannot give correct answers to questions.**
    3. What are possible negative societal implications of text generation models?
        - **They can be deployed at scale to spread false or misleading information, even unintentionally.**
    4. In situations where a model might make mistakes, and those mistakes 
could be harmful, what is a good alternative to automating a process?
        - **Instead its better to do a symbiotic approach in which a model and a human interact closely with feedback.**
    5. What kind of [[tabular data]] is [[deep learning]] particularly good at?
        - **They are really good at recommendation systems.**
    6. What's a key downside of directly using a [[deep learning]] model for [[recommendation]] systems?
        - **It tends to recommend what a user might like, rather than what would be helpful or interesting. The best ML approaches to this take all into account not just like.**
    7. What are the steps of the [[Drivetrain Approach]]?
        - **Defined Objective**
        - **Levers**
        - **Data**
        - **Model**
    8. How do the steps of the [[Drivetrain Approach ]]map to a recommendation system?
        - **Objective: drive additional sales by appealing to user.**
        - **Lever: the ranking of the recommendations**
        - **Data: Collect a wide range of recommendations for a wide range of customers.**
        - **Model: Build two models for purchase probabilities, conditional on seeing or not seeing a recommendation.**
    9. Create an image recognition model using data you curate, and deploy it on the web.
        - **Working on it!**
    10. What is [[DataLoaders]]?
        - A class in fastai that stores whatever you pass to it.
    11. What four things do we need to tell fastai to create [[DataLoaders]]?
        - **What kind of data**
        - **How to get list of items**
        - **How to label the items**
        - **How to create the validation set**
    12. What does the splitter parameter to [[DataBlock]] do?
        - **It splits the training and validation sets for testing.**
    13. How do we ensure a random split always gives the same validation set?
        - **Use a seed, by convention usually 42 to start.**
    14. What letters are often used to signify the independent and dependent variables?
        - **X and Y**
    15. What's the difference between the crop, pad, and squish resize approaches? When might you choose one over the others?
        - **Crop: cuts off images at a set length and width.**
        - **Pad: creates empty space (zeroes, black) around images.**
        - **Squish: makes the image fit a set length and width.**
    16. What is data augmentation? Why is it needed?
        - [[Data Augmentation ]]is the process of creating random variations of input data. It is needed to increase model accuracy to different situations. The image may look slightly different, but the meaning (label, answer, truth value) is the same.
    17. What is the difference between [[item_tfms]] and [[batch_tfms]]?
        - **Generally, [[item_tfms]] are performed by CPU, and [[batch_tfms]] are performed by GPU.**
    18. What is a [[confusion matrix]]?
        - **A confusion matrix is a visual way of quickly and accurately representing various aspects of a given model's performance.**
    19. What does export save?
        - **export in [[fastai]] saves a model so that you can later copy it to show others or to a server to use in production.**
    20. What is it called when we use a [[model]] for getting predictions, instead of training?
        - **When you use a [[model]] for predictions instead of training, it is called an [[inference]].**
    21. What are [[IPython]] [[widgets]]?
        - **They are small agile [[JavaScript]] and [[Python]] objects used to quickly and easily make [[GUI]] components in a web browser.**
    22. When might you want to use CPU for deployment? When might GPU be better?
        - **GPU is better for when you want to do a lot of identical work in parallel. In most other cases, such as when you are doing one thing at a time, CPU is probably better.**
    23. What are the downsides of deploying your app to a server, instead of to a client (or edge) device such as a phone or PC?
        - **The application needs a network connection, there's latency to take into account, etc.**
    24. What are three examples of problems that could occur when rolling out a bear warning system in practice?
        - **Video instead of static images**
        - **Night time images or low res images**
        - **Ensuring results are returned fast enough to be useful in practice.**
    25. What is "out-of-domain data"?
        - **Data that a model sees in production that is very different to what it saw in training.**
    26. What is "domain shift"?
        - **When the type of data a model sees changes over time.**
    27. What are the three steps in the deployment process?
        - **Manual Process: run model in parallel, human checks all predictions**
        - **Limited Scope Development: Careful human supervision, time or geographically limited**
        - **Gradual Expansion: Good reporting or logging systems, taking into account things that could go wrong.**
