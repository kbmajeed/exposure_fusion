========================================================

EXPOSURE FUSION

README

Kabir Abdulmajeed


========================================================
This folder contains the following:

(1) Main.py 
#(this is the main file to generate the results)

(2) exposureFusion.py 
#(this is the supporting library of functions used by Main.py)

To run the code and generate the results:




========================================================
Dependencies:
========================================================
spyderIDE == 3.2.8 
numpy==1.14.3
cv2 == 2.4.11
matplotlib==2.2.2



========================================================
Instruction:
========================================================
Step 1: Open exposureFusion.py in the SpyderIDE Editor

Step 2: Run exposureFusion.py to load modules

Step 3: Open Main.py in the SpyderIDE Editor

Step 4: Insert / Modify filepath for the folder containing Multi-exposure 
images in section "Load Input Images and Setup Dirs" 

eg:
	path = r"C:\Desktop\Images1"

Step 5: Run Main.py
By default, Main.py would create a new directory "results" in C:\Desktop 
containing the output (Exposure fusion using Multiresolution blending).

If all sections uncommented, and save=True,
then expected outputs in results folder include:
(1) img_BilateralFusion
(2) img_BlurFusion
(3) img_CenterOriginal
(4) img_MeanImage
(5) img_MultiresolutionFusion
(6) img_NaiveFusion
for image(i) in stack:
(7) img_contrast(i)
(8) img_exposedness(i)
(9) img_saturation(i)

Step 5: Un/Comment the desired section
** commenting unwated sections speeds up execution **
Sections include:
(1) Original Image
(2) Naive Exposure Fusion
(3) Blurred Exposure Fusion
(4) Bilateral Exposure Fusion
(5) Multiresolution Exposure Fusion
(6) Display Intermediate Steps and Save
(7) Compute Mean of Image Stack



========================================================
Notes:
========================================================
cv2.imwrite would save files to disk




Code is also available here:
https://drive.google.com/open?id=13ldBQgm0_c6JTF8qzNK4j8rBou2OWIv6

Relevant files can be found here:
https://drive.google.com/open?id=189wcU2gh6iFDWsO6nsplm55QUrcmYI2I


