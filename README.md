# DNA-classification-using-decision-trees

About the script:
-----------------
-The language used to implement the ID3 algorithm here is "python".
-There are two scripts uploaded that contain the code for the decision tree algorithm.
-One of them is a notebook document and the other is a python script and the names are "Decision_Tree.ipynb" and "Decision_Tree.py" respectively.
-The code in the notebook file can be seen as sections for better understanding.
-Both of them are executable under different environments and the instructions for execution are given below.

Instructions for execution:
---------------------------
Requirements:
1. Python 3.7 or above installed (for .py file)
2. Jupyter Notebook (for .ipynb file)
3. Google Colab (for .ipynb file)
4. Or any other IDE that supports python execution.

Steps to execute:
-----------------
1. Load the file into the environment, either .py file or .ipynb file.

2. Changing path for training data
  - In the "importing and processing the training data" section,
  - Change the path for the training data set.
  - Copy the path of the actual file in your system and paste as a parameter in the read_csv(method).
  - If Google colab is used, you can upload the file to the runtime and copy the path from there.

3. For calculating impurities in different methods,
  - In "calculating the information gain" section, the impurity method is called with two parameters.
  - One of them is the method name for the impurity calculation method.
  - For gini index, pass "gini" as the method parameter.
  - For entropy, pass "entropy" as the method parameter.
  - For miss-classification error, pass "mis" as the method parameter.
  - The impurity function is defined for all these methods in the above section.
   
4. For changing the confidence level
  - In "calculating the chi square value" section, 
  - While finding the chi square value from table, the confidence level is passed as an argument to chi2.ppf function.
  - The confidence levels for this project can be 0.0, 0.95, and 0.99.
  - Any one of these three levels can be used for producing better accurate results.

5. For testing the classifier
  - In "testing the classifier section", change the path of testing data.
  - Copy the path of the actual file in your system and paste as a parameter in the read_csv(method).
  - This algorithm generates a final csv file with the classification.
  - Generally, the output file is generated in the same folder in which the script files(.ipynb or .py) are located.
  - If you want the output file to be generated in other folder, copy the path of the folder and paste it in to_csv method
    and append the file name "prediction.csv" at the end of the path.

6. After following all the above steps, run all the cells(for .ipynb file) or run the entire code(for .py file).

7. The output file "prediction.csv" is generated in the specified folder.
