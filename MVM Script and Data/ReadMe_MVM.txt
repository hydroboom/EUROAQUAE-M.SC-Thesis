This script is written as a Multiple Variable Method for obtaining Representative Years.
The following main parts of the script are described briefly:


1. Normalizing the files: After you get the representative year outputs from the SVM script, you can 
use those to combine and normalize the data for the first phase of the MVM method. Depending on the 
number of your variables and the weight, as well as the mode you followed (CY, 12M) in the SVM method, 
you may have to modify the code. You have to ensure you have the folder(s) you want from SVM method in 
the folder of the MVM IPYNB. This code is written in a way to be able to access the folders and 
read/normalize those files and save it in a new folder 'Normalized'. 

2. Composite Representative Year: Based on the normalized file you choose (depending on the method
you want to proceed this with, e.g JSD) you will have to input the filenames in the script. You also
have to ensure that the files are containing your variables' names in the dataframe. You have the 
freedom to input weights on the variables or you can keep them equallt weighted. This snippet will
give you a balanced representative year which is useable for any of the variables in the combination 
you enter (in the script for example, the RY for THETAO and SO combination is shown).