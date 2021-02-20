README
BLAKE WASHBURN
The collections of files provided in this GitHub enviornment were written for
homework 1 in Dr. Feng Luo's Deep Learning Course at Clemson University during
the Spring 2021 semester (CPSC 8430). 

The files in this folder and their purpose are listed below. A description of 
the funtionality of each file can be found at the top of that file:
assignment_prompt.pdf - Directions for Assignment, written by Dr. Luo
Part1_SimulateAFuntion.ipynb - source code for Part1.1 Simulate a Function
Part1_TrainOnActualTask.ipynb - source code for Part1.2 Train on an Actual Task
Part2_VisualizeOptimization.ipynb - source code for Part2.1 Visualize the Optimization Process
Part2_ObserveGradientNorm.ipynb - source code for Part2.2 Observe Gradient Norm during Training
Part3_RandomLabels.ipynb - source code for Part3.1 Can Network fit Random Labels?
Part3_ParamGener - source code for Part3.2 Number of Parameters VS.Generalization
Part2_FlatGenerPart1 - source code for Part3.3.2 Flatness VS. Generalization
hw1_report_bwashbu.pdf - Assignment report with analysis of code and results

To run these files, the following libraries are required:
python 3.8
Pytorch 1.7
Tensorflow 2.4
Matplotlib 3.2.2
Numpy 1.19

The dataset required to run the source code is the MNIST dataset from the
torchvision datasets library in pytorch. Once the dataset is downloaded to this 
pathfile, it can be used by every other file and is the only file you will
need to download. In every file that requires the MNIST dataset, there is a
line of code that grabs the dataset. It is provided below:
trainingSet = datasets.MNIST('', train=True, download=False, ...)
To download the dataset, change the download option to True. This is done 
for you in the first source code file (Part1_TrainOnActualTask.ipynb). 
You will need internet connect to download the dataset.

To run the following .ipynb files, open juyper notbooks in an enviornment with
the above packages installed and run the cells in the file from top to bottom. 

Part2.3 "What Happens when Gradient is Almost Zero" and Part3.3.1 "Flatness
VS. Generalization Part1" of the assignment were not completed. For the former,
I struggled with finding a way to calculate the Hessian matrix in Pytorch. 
Regarding the latter, I could not figure out how to calculate the interpolation 
ratio. The equation was provided, but I did not know how to implement it 
in a real world network. 
