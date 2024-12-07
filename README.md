# STATS507_FinalProject
In this project, we seek to assess the performance of the Transformer-based Optical Character Recognition model in the presence of varying amounts of noise. This will give insight into how the state-of-the-art character recognition models perform when the document digitalization process has been corrupted.

# The Dataset
The dataset are pulled from the IAM Handwriting Database. In this repository, there are three directories of primary importance: sentences, words, and ascii. Of these, words and ascii are the most important. Words contains handwritten words from the IAM database. Note that there is a comprehensive folder hierarchy in this directory. For this project, we flatten this folder using the following entered into the command line:

find /Users/chandle/Desktop/STATS507/Data_Project/FinalProject_chandle/STATS507_FinalProject/words  -type f -exec cp {} /Users/chandle/Desktop/STATS507/Data_Project/FinalProject_chandle/STATS507_FinalProject/words_flatten \;

**NOTE** IT WILL TAKE A *long* time for this code to run. You are compressing the entire words dataset into a flattened directory.

# The code

The code is found in FinalProject.ipynb. This will describe, step by step, how to use the model on a handwritten text from the IAM dataset and a bit of handwritten text of my own. This jupyter notebook requires the following libraries: transformers, PIL, requests, pandas, numpy, cv2, random, and os. With the exception of the installation of these packages, this jupyter notebook should work out-of-the-box; moreover, you should be able to reproduce all of the results in the project writeup using this jupyter notebook.

# The Writeup

Finally, the writeup to this project is provided in the file STATS507_FinalProject_chandle.pdf. This contains details regarding the model, the dataset, our method, our results, and our conclusions.
