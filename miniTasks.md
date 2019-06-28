---
layout: page
title: Mini Tasks
nav_order: 3
---

# Mini Tasks

---

<h3><a href="https://github.com/INoLiao/NCTU_2019SpringPP" target="_blank">Parallel Programming</a></h3>
- <h4>Pthread - Estimate π by Monte Carlo Method</h4>
	<div align="justify">Toss darts randomly at a square dartboard, whose sides are two feet in length. Suppose that there is a circle inscribed in the square dartboard. The radius of the circle is one foot, so its area is π square feet. If the points that are hit by the darts are uniformly distributed, then the number of darts that hit inside the circle divided by the total number of tosses should approximately equal to π/4. Pthread is applied to parallelize the program through evenly distributing the total number of tosses by the number of cores. For 100M iterations, multiprocessing with 4 cores reaches 3.48 times speedup.</div>
- <h4>OpenMP - Parallelize Conjugate Gradient Method</h4>
	<div align="justify">Insert proper OpenMP pragma to parallelize the program. To find the appropriate pragma insertion point, profiling the serial version is adopted to find the bottleneck of the program execution. Meanwhile, analyze the trade-off between program speedup and overhead brought by parallel programming. The performance of multiprocessing with 4 cores reaches 2.00 times speedup.</div>
- <h4>MPI (Message Passing Interface) - Parallelize 2D Heat Conduction</h4>
	<div align="justify">Adopt MPI to parallelize 2D heat conduction problem by evenly distributing the workload of each iteration. The 2D plate is represented by a 2D array and each computing node is responsible for a portion of array elements. The performance of multiprocessing with 4 computing nodes reaches 1.67 times speedup. The speedup is limited due to the significant message passing overhead via the internet.</div>
- <h4>CUDA - Parallelize Concurrent Wave Propagation Equation</h4>
	<div align="justify">Design a CUDA kernel to realize the parallelism on GPU. NVIDIA GeForce GTX 1060 GPU is equipped to accelerate the concurrent wave propagation problem. The parallelism is accomplished by assigning total points of the concurrent wave to each GPU processing element. For 100K points and 100K iterations, CUDA achieves 169 times speedup compared with the serial version.</div>
- <h4>OpenCL - Parallelize the Generation of Histogram from Images</h4>
	<div align="justify">Design an OpenCL kernel to parallelize the histogram generation from images. NVIDIA GeForce GTX 1060 GPU is used in this task. The program is capable of processing multiple images efficiently by keeping the kernel activated until all images are processed. 6 images with an average size of 5K by 3K pixels are tested and the OpenCL achieves 1.46 times speedup.</div>

---

<h3><a href="https://github.com/INoLiao/NTHU_2019SpringOS" target="_blank">Operating Systems</a></h3>
- <h4>Linux Kernel - Load/Remove Kernel Modules</h4>
	<div align="justify">Construct a linked list and load the list to the kernel. The list contains nodes recording student ID and birthday. When the kernel is initiated, the linked list with five student nodes is created. The student ID, birthday, and the memory address of each node are printed on the kernel log buffer. When the kernel is terminated, the linked list is removed and its memory space is released back to the system to prevent a memory leak.</div>
- <h4>Traverse Linux System Kernel Tasks</h4>
	<div align="justify">Design kernel modules that traverse all tasks in the Linux system. Firstly, traverse system tasks in a linear manner and the expected list of tasks are ordered by pid. In addition, design the DFS algorithm to traverse system tasks in a parent-children manner and the expected list of tasks are ordered according to the relationship of inheritance.</div>
- <h4>Merge Sort Parallelism by Pthread</h4>
	<div align="justify">Exploit Pthread to implement multithreading program on merge sort. The main thread creates an additional two threads which are responsible for sorting half of the array. After sorting is completed, the main thread will merge two sorted arrays.</div>
- <h4>The Dining Philosophers Problem</h4>
	<div align="justify">Implement the famous Dining Philosophers Problem using Pthreads. There are 5 philosophers and 5 forks. All philosophers are initialized to the state of THINKING. The THINKING time is randomly generated from one to three seconds. After THINKING, the state changes to HUNGRY, implying that the philosopher wants to eat. Therefore, the philosopher will try EATING. If the philosopher can acquire left and right forks, she can start EATING. The EATING time is randomly assigned from one to three seconds. Note that the fork is a metaphor of computer resource and left and right forks are available if left and right philosophers are not EATING. After finishing the meal, the philosopher will return the forks and start THINKING again. Right after the philosopher returns the forks, she will test if left and right philosophers would like to eat. Such an action is to wake up others to continue their job when the resource is available. </div>
	
---

<h3><a href="https://github.com/INoLiao/NCTU_2018SpringDM" target="_blank">Data Mining</a></h3>
- <h4>Association Rules - Interpretations of Weather Data and Power Plant Data of Taiwan</h4>
	<div align="justify">For both applications, the FP-Growth algorithm is applied for mining the association rules among interesting parameters. For weather application, the association rules among temperature, humidity, wind speed, pressure, and time are analyzed. For power plant data, the relationship of net electricity usage of northern, central, southern, and eastern Taiwan is dug out. Interesting interpretations and insights are provided in this task.</div>
- <h4>Clustering - Analysis of PM2.5 in Taiwan</h4>
	<div align="justify">Analyze the PM2.5 data in Taiwan using clustering algorithms. Both K-Means and DBSCAN (Density-Based Spatial Clustering of Applications with Noise) are adopted so that proper comparisons between these two algorithms can be analyzed.</div>
- <h4>Classification - NBA Game Winning Prediction</h4>
	<div align="justify">The task is the prototype of the comprehensive <a href="https://inoliao.github.io/nbaWebsite/" target="_blank">NBA Game Prediction System</a>. Thorough data mining design flow from problem definition, data preprocessing, feature extraction, machine learning model training, to model prediction are covered. Classification algorithms such as Logistic Regression, XGBoost, Random Forest, and AdaBoost are applied for NBA game-winning prediction.</div>