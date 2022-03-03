# EE-435-Deep-Learning-course-project
Final course project - Face Verification as zero shot learning


Created a data loader to generate positive and negative examples by concatenating two images of the same person and two images of different people, respectively
Modified the pre-trained ResNet-18 model to train on concatenated examples to distinguish if two faces are of the same person or not
Established a baseline accuracy of ~90% on validation examples with previously unseen people. Working on improving accuracy by modifying model architectures and hyperparameters
