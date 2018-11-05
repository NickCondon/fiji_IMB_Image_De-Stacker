# fiji_IMB_Image_De-Stacker
This is a FIJI/ImageJ script that batch takes 3D/4D images and de-stacks them into lower dimensional files.

IMB_Image_De-stacker<br>
Developed by Dr Nicholas Condon <br>
[ACRF:Cancer Biology Imaging Facility](https://imb.uq.edu.au/microscopy) <br>
Institute for Molecular Biosciences, The University of Queensland
Brisbane, Australia 2018

This script is written in the ImageJ1 Macro Language.


Background
-----
This script is designed to reduce the dimensionality of image data-sets, providing .tif output files of either individual channels, slices, and/or frames.<br>

This script can work on multiple files within a single directory and as long as the format is Bio-formats compatible,  it should run fine. (TIP: Go windowless for the format which you plan to use. See “Preventing Bio-formats Importer window.rtf” file to do this.)<br>


Running the script
-----
The first dialog box to appear explains the script, acknowledges the creator and the ACRF:Cancer Biology Imaging Facility. <br>

￼The second dialog to open will warn the user to select the working directory of your files and to take note of the file extension that they wish to process.<br>

The script then asks you to select the directory you wish to process. <br>

The script will prompt you for the for the parameters you wish to include in your processing.<br>

The options for reducing the original imaging file can be stacked. You can tick, 1, 2 or all three options. <br>

Subfolders option places each image file into a new subfolder. <br>

The final dialog box is an alert to the user that the batch is completed. <br>

Output files
-----
Files are put into a results directory called “filename_extracted" within the chosen working directory. Files will be saved as either a .tif or .txt for the log file. Original filenames are kept and have tags appended to them based upon the chosen parameters. <br>

A text file called log_Image De-Stacker.txt is included which has the chosen parameters and date and time of the run.

Preventing Bio-Formats Importer Window
-----
To prevent Bio-formats Importer window from displaying for each file in your batch complete the following:
1. Open FIJI
2. Navigate to Plugins > Bio-Formats > Bio-Formats Plugins Configuration
3. Select Formats
4. Select your desired file format (e.g. “Zeiss CZI”) and select “Windowless”
5. Close the Bio-Formats Plugins Configuration window

Now the importer window won’t open for this file-type. To restore this, simply follow the steps above and untick ‘Windowless”

￼
