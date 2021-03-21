- [[Ch 4 Questions]]
    1. How is a [[grayscale]] image represented on a computer? How about a color image?
        - **A grayscale image is represented by numbers between 0 and 255 for each individual pixel, denominating what shade that is between white (0) and black (255).**
    2. How are the files and folders in the[[ MNIST_SAMPLE]] dataset structured? Why?
        - **There are separate folders for training and validation sets. It's common practice and helps keep that data separate.**
    3. Explain how the "pixel similarity" approach to classifying digits works.
        - **This approach would take all the grayscale values of each individual pixel in a given picture, and find the average value of the entire "number" or image. Then, you would have a baseline to compare to other numbers and see if they are near each other.**
    4. What is a [[list comprehension]]? Create one now that selects odd numbers from a list and doubles them.
        - **[[List comprehension]] is a feature of [[Python]] that isn't in all programming languages. It's a simple and intuitive way to create common loops for manipulating variables.
doubled_odds = [x * 2 for x in list(nums) if x % 2 !=0]**
    5. What is a "rank-3 [[tensor]]"?
        - **A three dimensional [[tensor]].**
    6. What is the difference between [[tensor]] rank and shape? How do you get the rank from the shape?
        - **The shape of a [[tensor]] is the length of each axis. The rank of a tensor is the length of it's shape.**
    7. What are [[RMSE]] and [[L1 norm]]?
        - **[[L1 norm]] is the [[mean absolute difference]] and [[RMSE]] is the root mean squared error, or [[L2 norm]].**
    8. How can you apply a calculation on thousands of numbers at once, many thousands of times faster than a [[Python]] loop?
        - **You convert the data to [[array]]s or [[tensor]]s.**
    9. Create a 3×3 tensor or array containing the numbers from 1 to 9. Double it. Select the bottom-right four numbers.
        - **Practiced code in notebook.**
    10. What is [[broadcasting]]?
        - **The act of automatically expanding the [[tensor]] of a smaller rank to have the same size as the larger rank [[tensor]] in an operation between the two.**
    11. Are metrics generally calculated using the [[training set]], or the [[validation set]]? Why?
        - **Using the [[validation set]]. So that there is no [[leakage]], among other things.**
    12. What is [[SGD]]?
        - **It stands for [[Stochastic Gradient Descent]]. Stochastic means random. Gradient means slope, or rise/run, and descent means to lower or approach from above. Putting those all together in a machine learning sense: start with random point, calculate slope or derivative and incorporate that into a loop where the function can see if its getting better or worse at predictions, and approach the best possible accuracy for predictions using trial and error.**
    13. Why does [[SGD]] use mini-batches?
        - **It tries to find the middle ground between calculating all the dataset, which would take a long time, and only doing one point, which would not be very informative.**
    14. What are the seven steps in [[SGD]] for [[Machine Learning]]?
        - The seven steps are: 
            - **Init** 
            - **Predict** 
            - **Loss**
            - **Gradient**
            - **Step**
            - **Repeat**
            - **Stop **
    15. How do we initialize the weights in a model?
        - **They are initialized to random values.**
    16. What is "loss"?
        - **Loss is a conventional way to calculate the effectiveness of the current weight. By convention big loss is bad, small loss is better.**
    17. Why can't we always use a high learning rate?
        - **It will go too far and overshoot the target, or could bounce between being too high and too low over and over.**
    18. What is a "gradient"?
        - **A slope, or a derivative.**
    19. Do you need to know how to calculate gradients yourself?
        - **Not necessarily no, things like PyTorch do it for you.**
    20. Why can't we use accuracy as a loss function?
        - **It would translate as a gradient of near zero almost everywhere, which is not useful.**
    21. Draw the sigmoid function. What is special about its shape?
        - **It looks like a stretched out letter 's'. It's special in that it will return a positive or negative gradient depending on if the loss is good or bad.**
    22. What is the difference between a loss function and a metric?
        - **A metric (like accuracy) helps to drive human understanding, while a loss function is better for automated learning (through machines).**
    23. What is the function to calculate new weights using a learning rate?
        - **w -= gradient(w) * lr**
    24. What does the [[DataLoader]] class do?
        - **It takes a dataset and can create batches to be processed.**
    25. Write [[pseudocode]] showing the basic steps taken in each epoch for [[SGD]].
        - Done in notebook
    26. Create a function that, if passed two arguments [1,2,3,4] and 'abcd', returns [(1, 'a'), (2, 'b'), (3, 'c'), (4, 'd')]. What is special about that output data structure?
        - This is known as a tuple. It has two different kinds of variables.
    27. What does view do in [[PyTorch]]?
        - **It changes the shape of a [[tensor]] without changing the contents.**
    28. What are the "bias" parameters in a neural network? Why do we need them?
        - It is needed because the weights when the value is equal to 0 is 0, it is needed as a constant in the equation to prevent this.
    29. What does the @ operator do in [[Python]]?
        - It does matrix multiplication aka [[matmul]].
    30. What does the backward method do?
        - It signifies [[backpropogation]], which calculates the derivative at each layer (which is how the [[SGD]] model learns over time) 
    31. Why do we have to zero the gradients?
        - [[Pytorch]] loss.backward() function adds gradients to those already existing, so they must be zeroed out if you want just the current values.
    32. What information do we have to pass to [[Learner]]?
        - **You need to pass in all the elements: the data (through [[DataLoaders]]), the model, the [[optimization function]], the [[loss function]], and any metrics you want to print out.**
    33. Show [[Python]] or [[pseudocode]] for the basic steps of a training loop.
        - **Done in notebook.**
    34. What is "[[ReLU]]"? Draw a plot of it for values from -2 to +2.
        - **A different optimization function, like sigmoid. Starts near 0 and ramps up rapidly for activation.**
    35. What is an "[[activation function]]"?
        - A function that can return as either on or off (1 or 0) that is used in neural networks. They are also called [[nonlinearities]].
    36. What's the difference between F.[[ReLU]]and nn.[[ReLU]]?
        - **F.[[ReLU]] is a function and in [[PyTorch]] nn.[[ReLU]] is a module. You need to instantiate it, but it is largely similar.**
    37. The universal approximation theorem shows that any function can be approximated as closely as needed using just one nonlinearity. So why do we normally use more?
        - **There is a performance tradeoff. With more layers, you don't need as many parameters, and thus you can use smaller matrices with more layers instead of larger matrices and fewer layers.**
