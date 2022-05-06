# Monocular Depth Estimation using Deep Learning

### Project Author
	1. Gopal Krishna
	2. Gourav Beura

### Project Presentation and Demo Link
The Project Presentation and Video Link is added in the Google spreadsheet.
https://youtu.be/WBAdfvj9xlQ

### Project Description:
	Monocular Depth Estimation - We propose to solve monocular depth estimation into a supervised learning problem. 
		The setup is simple: we convert an input image into per-pixel distance estimates (a depth map) using deep learning-based computer vision 
		techniques. We use RGB images and corresponding ground truth depth maps to supervise the learning of neural network weights via standard 
		backpropagation of prediction errors.
		
### Check-ins
	1. Checkin 1 -
		In our initial approach, we are adopting transfer learning for the task starting with a baseline architecture composed of “DenseNet-169” trained on the ImageNet database as a feature encoder and a decoder for estimation of depth from the encoded features. 
		We are trying to reproduce the methodology from: https://arxiv.org/abs/1812.11941 and set up experiments using the NYU-Depth-V2 
		and KITTI dataset which consists of indoor and outdoor scenes respectively.
	
	2. The progress so far-
		1.	We have studied the NYU-Depth-V2 and KITTI dataset.
		2.	Implementing the end-to-end pipeline for the project. That includes:
				a.	scaling downing the image to lower size( 320x320)
				b.	generating the dataset and data loader of the mat files
				c.	implementing the Deep Learning Model
				d.	designing the training and test functions
				e.	Finally, perform hyper-parameter tuning for improve results (if time permits).
 
### Operation System
Windows 11

### IDE
Jupyter Notebook

### Instructions for running the python files
	1. Make sure to install pytorch, ,h5py and sk-learn on your machine
	2. Before executing the code make sure that the dataset is present the directory structure: 
		<root_dir>
		|_./dataset
			|_nyu_depth_v2_labeled.mat
			|_splits.mat
	3. Open the .ipynb files in Jupyter Notebook and run each cell.
	
### Project Repo:
	https://github.com/gourav10/Monocular_Depth_Estimation
	
### References
	1. https://github.com/ialhashim/DenseDepth
