# SKELY:Recognize_Orientation_of_a_3D_Skeleton
Where is the skeleton facing ? The task is to predict the orientation of a 3D model from a single picture.

This problem introduces a non-uniform distribution of samples in the training and the test set. And more importantly, this problem also evaluates out-of-distribution generalization.


## Challenge
For input you will be given a large number of images, for about half of them, we have measured the orientation of the skeleton. But to be able to stitch all those images together, you have to figure out how to predict the orientation of the skeleton for the rest of the images.

## Dataset
The training dataset consists of 9999 images of size 2048x1898 with 4 channels each (for RGBA). The associated label is a single continuous variables :

xRot : Orientation of the Skeleton, in degrees, along an arbitrarily chosen axis (a number between 0 and 360). The axis around which this value is measured, is consitent across the whole of the training and the test set.
The test dataset consists of 10001 images of size 2048x1898 with 4 channels each (for RGBA). The goal of the task is to predict the xRot value of the Skeleton in these test images.

## Evaluation Criteria
During evaluation Mean Squared Error be used to test the overall performance of model

## LeaderBoard
https://www.aicrowd.com/challenges/aicrowd-blitz-2/problems/skely/leaderboards
