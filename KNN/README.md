The Nearest Neighbors method (k Nearest Neighbors, or kNN) is a very popular classification method, also sometimes used in regression problems.  At the level of intuition, the essence of the method is this: look at the neighbors; which ones prevail - so are you. Formally, the basis of the method is the compactness hypothesis: if the distance metric between examples is introduced quite successfully, then similar examples are much more often in the same class than in different ones.

![image](https://github.com/fewHoursLater/ML/assets/84395151/640808d3-6b1c-43b2-b608-1f2721170ec6)


To classify each of the objects of the test sample, the following operations must be performed sequentially:

- Calculate the distance to each of the objects in the training sample
- Select the objects of the training sample, the distance to which is minimal
- The class of the object being classified is the class most commonly found among the k nearest neighbors


We will work with a subsample of data on the type of forest cover from the UCI repository. There are 7 different classes available. Each object is described by 54 features, 40 of which are binary.
