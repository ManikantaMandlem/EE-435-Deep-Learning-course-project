# EE-435-Deep-Learning-course-project
Final course project - Face Verification as zero shot learning


Created a data loader to generate positive and negative examples by concatenating two images of the same person and two images of different people, respectively
Modified the pre-trained ResNet-18 model to train on concatenated examples to distinguish if two faces are of the same person or not
Established a baseline accuracy of ~90% on validation examples with previously unseen people. Working on improving accuracy by modifying model architectures and hyperparameters
 Project master: This is the base code which is implemented using ResNet18 as base architecture
 
 Project2_experiment1: For Resnet18, with final FC layers as [1024, 512, 256, 2]. Here, no of trainable parameters are: 12,362,050
 
 Project2_experiment2: For Resnet18 by ignoring the last average pooling layer and flattening and connecting to the fc [x,1024, 512,256,2]. Here no of trainable parameters are: 148,158,786

Project2_experiment3: Experiment1 with more legitimate data augmentation techniques. There seems to be some bias in the model or data and I think the flip vertical augmentation technique could be introducing some bias. So remove flip vertical and add more legitimate augmentation techniques

Project2_experiment4: Using efficientnet b2 network as base architecture, rest all things are same as master. No of trainable parameters are 8,555,780
