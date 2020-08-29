# ICPose
"I see pose" is a complete machine learning package containing both the models and full architecture for my masters project.
The package uses depth-images as input to estimate pose from a mixed bottom-up model, where it first finds evidence for joints, and then estimates the poses for each detected person instance. The project is inspired by [OpenPose][1], and is trained on the [Panoptic Studio dataset][2].

The goals for this project is both speed and accuracy, and should work on relatively limited hardware like the [Jetson TX2][3], and is implemented in [pytorch][4].


[1]: https://github.com/CMU-Perceptual-Computing-Lab/openpose
[2]: http://domedb.perception.cs.cmu.edu/
[3]: https://developer.nvidia.com/embedded/jetson-tx2
[4]: https://pytorch.org/
