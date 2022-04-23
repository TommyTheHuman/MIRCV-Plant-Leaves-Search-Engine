# Plant-Leaves-Search-Engine---MIRCV
Plant Leaves Search Engine is a system that can recognise the species given a leaf image by the user. Our engine can recognise leaves from 14 different plants: Apple, Blueberry, Cherry, Corn, Grape, Orange, Peach, Pepper, Potato, Raspberry, Soy Bean, Squash, Strawberry and Tomato. In order to do that we exploit a fine- tuned version of DenseNet121, and for the retrieval we use a Vantage Point Tree index.

We decided to extract the features using the finetuned model, to obtain the correct result we deleted the classification layers at the end of the neural network. We exploit these feature to build the VPT index, thanks to the features we retrieved the k nearest neighbours using a distance measure. We compared the query time between the usage of a VPT index and a brute force approach. Finally we have evaluated the pretrained model and the finetuned one using the MaP metric.

#link to the entire dataset
https://drive.google.com/file/d/1hVKgDn6qdx_BSuYPxGk6crwF5l7kOAk_/view?usp=sharing
