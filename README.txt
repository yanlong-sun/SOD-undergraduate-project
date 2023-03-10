Step 1.   
(Obtain the dataset): Unzip the 'LFSD.zip' and 'NJU2K.zip' files in the 'Dataset' folder to obtain the dataset.

Step 2. 
(Calculate the depth saliency map): Open the 'acsdSaliency.sln' file in the '1_acsdSaliency' folder, modify the name of the dataset (LFSD or NJU2K) to be processed in 'demo.cpp', and then compile.

Step 3   
(Fuse the depth saliency map): Open the 'Process_org_image.m' file in the '2_Pre-Processing' folder, modify the name of the dataset (LFSD or NJU2K), and then compile.

Step 4   
(Compute the initial saliency map using the multi-task FCN): In the Ubuntu system (with the Caffe environment configured), open the terminal in the '3_deepSaliency' folder, modify the name of the dataset (LFSD or NJU2K) to be processed in the 'demo.py' file, and then run 'python demo.py' in the Caffe environment.

Step 5. 
(Refine the saliency map): Open the 'Runme_forBLsaliencymap.m' file in the '4_Refinement' folder, modify the name of the dataset (LFSD or NJU2K), and then compile. The final saliency map is stored in '../SaliencyMap/LFSD/Ours' and '../SaliencyMap/NJU2K/Ours'.


Step 6.   
(Objective evaluation): Open the 'evaluate_models.m' file in the '../5_Evaluation/tools/' folder, run the program, select the model and dataset to be evaluated, and the results are stored in '../5_Evaluation/Results/'.
