# ETDE:Exponential and Trigonometric Functions Inspired Single Image Detail Enhancement Algorithm
This is the source code of paper named "Exponential and Trigonometric Functions Inspired Single Image Detail Enhancement Algorithm". 
## Project Introduction
This repository contains the MATLAB implementation of the FLIDE(Exponential and Trigonometric Functions Inspired Single Image Detail Enhancement Algorithm) algorithm proposed in the paper.

Existing residual learning-based methods often adopt greedy search strategies, leading to premature convergence to local optima.
To solve this problem,ETDE transforms the image block matching problem into a two-dimensional location optimization problem.
The candidate matching area is iteratively optimized within the set boundary, and the algorithm can dynamically balance the global search and local optimization through the nested combination of exponx-trigonometric functions to avoid falling into local optimum and improve the performance of the system.

## File Structure
```
├── ETDE.p           # [Core Algorithm] Specific optimization and image processing functions
├── main.m           # [Main Program] Running this program will result in the enhanced image
├── data/            # [Input Folder] Stores the .png images to be processed
├── results/         # [Output Folder] Stores the enhanced images,you need to add folders by yourself.
├── Requirements.txt # Environment dependency instructions
```
## System Requirements
The code has been tested and verified on the following platform:

* **MATLAB Version:** R2023a or later
* **Operating System:** Windows 10/11, Linux, or macOS

### Required Toolboxes
To run the code successfully, the following MATLAB toolboxes are required:

* **Image Processing Toolbox** (Required for image I/O, resizing, and metric calculation)
* **Parallel Computing Toolbox** (Required for the `parpool` acceleration used in the core algorithm)


## Parameter Description (can be modified in main.m)
factor :
Enhancement intensity coefficient

Recommended range: 2.0 - 5.0

'.\data': Input image path 

'.\results': Output result save path 

## Usage
Step 1: Download or clone this project to your local machine

Step 2: Place the image that needs to be enhanced into the "data" folder (The image format should be in PNG format).

Step 3:Type main in the Command Window and press Enter, or simply click the "Run" button in the Editor.

Step 4:Through the above steps, the enhanced image will be saved in the "results" folder.
