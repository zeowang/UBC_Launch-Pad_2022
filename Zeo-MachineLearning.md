# Zeo Wang's submission of UBC LaunchPad 2022 - Technical Challenge.

## Machine Learning
`All your friends have been asking you, what is Machine Learning? Some people think it is the solution to world hunger, while others think it is just a stupid fad. You want to show your friends that machine learning is powerful for certain circumstances, using examples that they can easily understand. Explain techniques and challenges with ML with respect to your example, and convince us that Machine Learning is not just a buzzword.`

Many people think Machine Learning is a tool that can solve every problem and idealized it too much. I would say ML is indeed powerfull but still has many limitations.

#### Concept(I understood)
Let us start with the concept: Machine Learning is a method of developing some algorithms that can automatically "learn," by the word "learn" here it really means make statistical analysis and adjust itself accordingly, so that it may predict some pattern of how the data changes.

Think about the example of random walk in linear algebra. What the machine is "learning" is the position of individual steps of walks, namely the positions, and what is generating inside the machine is this transformation matrix. With a large input of discrete positions, the machine should be able to compute the state transformation matrix and make prediction by matrix multiplications. In this idealized simple example, the machine is learning this covariance between different states.

In real world, there would not be "definite states" given any system, that is where the probability theory and statistical analysis comes in. The data be given will with a lot of "noise," which needed to be filtered out some way. This is where we need to introduce some limitations.

#### Limitations
First, just like teaching a kid, you need to carefully select a range of "trusted" data so that the machine can have a proper initial state. If one starts by feeding meaningless data or data leans towards a whole opposite direction, you would either, if you are lucky, spend A LOT of time to correct that or more commonly, failed. By the word "fail" here I am really talking about the transformation matrix the system figured out will never fit the predicted data. It is a time-consuming job to categorizing and process these data manually or create an algorithm.

Then, you need to get it "learning." In some areas, there is just not enough data to collect from, and ML is easy to apply in such topics. Some other topics have database that are not easily accessed. In principle, you can write a WebCrawler and run it, but it might violate the website restrictions, and cause very serious consequences. (Like your ID being blocked or get penalty from UBC)

Finally, it comes down to interpreting the data. Some of these matrices involving multivariable and environment-dependent parameters can be totally not intelligible. Human might not be able to understand how the machine comes down to, even with the expected result. An example is Google Alpha Go.


#### Techniques
The most widely used technique in science is regression, especially linear regression. There are many kinds of regressions, involving single variable and multivariable, and each type has Linear and Non-Linear. In linear regression, it is like find the best-fit-line given a hole bunch of data. The input type can be multi-dimensional vectors, single data and so on. Another technique is classification model. It is a method of Supervised Learning, which it can conclude from observed values as one or more outcomes in a categorical form. There are many algorithms in building such models, such as building the decision tree. With a classified dataset, we should be able to cluster them into same group if there are some similarities. Finally, you should have some algorithm that can identify and categorize unexpected data and classify them. Then we can say you have a robust model for some system.
