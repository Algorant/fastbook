- [[Ch 1 Questions]]
    1. Do you need these for deep learning?
        1. Lots of math T / F | **False!**
        2. Lots of data T / F | **False!**
        3. Lots of expensive computers T / F | **False**!
        4. A PhD T / F | **False**
    2. Name five areas where deep learning is now the best in the world.
        - **[[NLP]], [[Self-Driving Cars]], [[Computer Vision]], Medicine/Biology, Image Generation**
    3. What was the name of the first device that was based on the principle of the artificial [[neuron]]?
        - **The Perceptron**
    4. Based on the book of the same name, what are the requirements for parallel distributed processing (PDP)?
        - **Processing Units**
        - **Activation**
        - **[[Output Function]]**
        - **Pattern of Connectivity**
        - **[[Propogation Rule]]**
        - **[[Activation Rule]]**
        - **Learning Rule**
        - **Environment**
    5. What were the two theoretical misunderstandings that held back the field of neural networks?
        - ** The thought was that it was unable to solve a [[XOR]] Gate.
        - ** Did not add extra layers**
    6. What is a GPU?
        - A Graphical Processing Unit. A video card. [[AMD]]/[[Nvidia]] are the two main manufacturers.
    7. Open a notebook and execute a cell containing: 1+1. What happens?
        - **It returns "2".**
    8. Follow
 through each cell of the stripped version of the notebook for this 
chapter. Before executing each cell, guess what will happen.
        - **Ok**
    9. Complete the [[[[Jupyter]] Notebook ]]online appendix.
        - **Not needed.**
    10. Why is it hard to use a traditional computer program to recognize images in a photo?
        - **It's difficult to tell a computer every step in the process and make it code.**
    11. What did Samuel mean by "weight assignment"?
        - **He basically meant a particular choice of values for variables.**
    12. What term do we normally use in deep learning for what Samuel called "weights"?
        - **Parameters is a better word.**
    13. Draw a picture that summarizes Samuel's view of a machine learning model.
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FIncertophile%2FumMYaB1JhZ.svg?alt=media&token=519a61f5-e500-451e-b5ee-b83fd1e142b5)
    14. Why is it hard to understand why a deep learning model makes a particular prediction?
        - **It's a little bit of a black box. The computer doesn't tell you how its doing it explicitly.**
    15. What is the name of the theorem that shows that a neural network can solve any mathematical problem to any level of accuracy?
        - **The [[Universal Approximation Theorem]]**
    16. What do you need in order to train a model?
        - **Data!**
    17. How could a feedback loop impact the rollout of a predictive policing model?
        - **It could end up predicting arrests, not crimes. Which gets into the issue of proxies.**
    18. Do we always have to use 224×224-pixel images with the cat recognition model?
        - **No, its a legacy thing. You can use basically anything now.**
    19. What is the difference between [[Classification]] and [[Regression]]?
        - **[[Classification]] deals with predicting a class or category. [[Regression]] deals with numeric quantities, such as temperature of a location.**
    20. What is a [[validation set]]? What is a [[test set]]? Why do we need them?
        - A [[validation set]] is a subset of data on which the model is tested for accuracy, which is held out of the [[training set]]. A [[test set]] is a data even further removed. It cannot be used in the model at all and is only for verification purposes.
    21. What will [[fast.ai]] do if you don't provide a validation set?
        - **[[fast.ai]] will create one for you!**
    22. Can we always use a random sample for a validation set? Why or why not?
        - **You can but you may not want to. It may not be an accurate representation of reality.**
    23. What is [[overfitting]]? Provide an example.
        - **A model that is getting reduced accuracy due to being too focused on predicting the training set, and not tuned to be able to predict new data.**
    24. What is a [[metric]]? How does it differ from "loss"?
        - **Metric is a function that measure the quality of the model's predictions using the validation set. Common ones are things like [[Error Rate]] and [[Accuracy]]. Loss is one metric you might use, but not necessarily.**
    25. How can pretrained models help?
        - **A pretrained model allows models to be more accurate, more quickly, with less data, and less time and money spent.**
    26. What is the "head" of a model?
        - **The part of a model that is newly added to be specific to the new dataset.**
    27. What kinds of features do the early layers of a [[CNN]] find? How about the later layers?
        - **Early on it can find diagonal, horizontal, and vertical edges. Later it can find higher level semantic components, such as car wheels, text, and flower petals.**
    28. Are image models only useful for photos?
        - **No! Can work for all kinds of stuff that you can translate into photos (visual component)**
    29. What is an "architecture"?
        - **The functional form of a model.**
    30. What is segmentation?
        - **A model that can recognize the content of every individual pixel of an image.**
    31. What is y_range used for? When do we need it?
        - It lets the model predict the target within a certain range, as the prediction is a continuous number.
    32. What are "hyperparameters"?
        - High level choices that determine the meaning of weights. That is, parameters for a parameter.
    33. What's the best way to avoid failures when using AI in an organization?
        - **Ensure that you know what the test and validation sets are and why they are important.**
    34. ### [Further Research](https://console.paperspace.com/te1hfdivi/notebook/r69qx4wp8j2xv4?file=01_intro.ipynb#further-research-1)
        - Each chapter also has a "Further Research" section that poses questions that aren't fully answered in the text, or gives more advanced assignments. 
Answers to these questions aren't on the book's website; you'll need to 
do your own research!
            - Why is a GPU useful for deep learning? How is a CPU different, and why is it less effective for deep learning?
            - Try to think of three areas where feedback loops might impact the use of 
machine learning. See if you can find documented examples of that 
happening in practice.
