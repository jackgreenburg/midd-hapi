# Project Proposal

## Abstract

This project aims to prevent hospital acquired pressure injuries by searching for a model that can help predict when they will occur. This problem involves overcoming the challenges presented by making use of a highly imbalanced timestamped data set with heavy missingness. To accomplish our goals, we must extensively read the existing literature in order to come up with various vectorization, imputation, and training techniques that we can test for effectiveness. Success in this project will result in a report on the efficacy of a wide range of training pipelines, and hopefully a highly accurate predictor.


## Motivation and Question

The motivation for my project is to help prevent pressure injuries, which are very dangerous to the health of patients with low mobility during extended hospital stays. A sufficiently accurate model could warn nurses of patients likely to develop a pressure injury before it occurs. Additionally, the complex nature of the dataset that we are using presents a good opportunity to learn about machine learning techniques that we can implement in other places in the field of pathology.

## Planned Deliverables

At the conclusion of this project I will have a brief report comparing the effectiveness of a number of vectorization techniques as well as a few models. 

Full success: I am able to implement and then compare all of the imputation methods I have found in my study of the literature. I test at least LSTM and GRU models (with variations). I also would like to try out some more creative methods that I have come across. At the end, I have a well tuned model that matches or exceeds ones previously developed.

Partial success: I am only able to implement some of the vectorization techniques. I am only able to test out a few models. I do not train any models that can match up to others that have been developed. At the very least, I have significantly advanced my knowledge of everything that I have implemented.

## Written Deliverables
I will also write a blog post on my project; I will not discuss this post in my proposal though.

## Resources Required

Through a lab at the Dartmouth Department of Pathology I have a large dataset and access to multiple compute nodes for training.

## What You Will Learn

### Theory

In this project I will need to learn about many advanced machine learning methods. In trying to identify an optimal model, I will need to test both data preparation methods and machine learning models. In order to discern which ones may be better for my task, I will need to have an understanding of how they work. At the very least, I expect to gain significant knowledge of imputation techniques and a few select recurrent neural network models.

### Technical methods

Due to the size of my dataset (around 100,000 patients), I will need to take advantage of GPUs for training. In order to do this, I will need to learn more about how to actually take advantage of GPU support. I will also need to learn more about running jobs on Slurm.

## Risk Statement

There is definitely a risk that timestamped EHR data does not significantly contribute to a more accurate predictor of hospital acquired pressure injuries. There is also a risk that our dataset is not large or diverse enough to offset how imbalanced it is. 
Additionally, there is a small risk that the nodes on the Dartmouth HPC system that I have access to go down at a critical time (it would not be particularly surprising).

## Ethics Statement

### Who has the potential to benefit?

This project has the potential to help prevent hospital acquired pressure injuries from occurring, so, if it is effective, it could be quite beneficial for patients with low mobility who have extended hospital stays. Hospitals also stand to benefit because pressure injuries are difficult and expensive to treat.

### Who might be harmed?

For starters, there is always going to be the potential problem of over reliance on automated systems. Another significant issue that could arise from models trained on this dataset is that the data comes from the Dartmouth Hospital in New Hampshire where a very high percentage of the patients are white. This is especially problematic considering how imbalanced the dataset is. Among other possible problems, our model could become optimized for white patients, with other races receiving less proactive care. This risk also exists for other possible identifiers, not just race.

### Will the world become a better place? 

Advancing the research towards better health outcomes would definitely make the world a better place. This assumes that I formulate my research into a paper that is published and then is actually utilized later. It also assumes that whoever ends up implementing my model or one descendent from my research is careful with its implementation. They must make sure to continue to trust the nurses who are primarily responsible for preventing pressure injuries from occurring.

## Tentative Timeline

#### Week 3

- Review most recent literature
- Implement some fun imputation methods
- Some RNN model trained

#### Week 6

- Implement some serious imputation methods
- Show some results comparing RNNs

#### Week 9

- Implement some serious imputation methods
- Show some results comparing RNNs
- Fix the issues that came up before week 6 that likely prevented me from doing the really fun stuff...

