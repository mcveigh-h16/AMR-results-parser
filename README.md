# AMR-results-parser

upyter notebook to import the output of AMRFinder https://github.com/ncbi/amr/wiki/Running-AMRFinder and parse it into a format that is usable by genome workbench. Gene and allele names are verified by a curated list.

Jupyter notebook installation requires the installation of https://docs.anaconda.com/anaconda/navigator/ on your PC. Once you launch Anaconda Navigator your select "jupyter notebook" to launch the application. The code is attached in AMRparser.ipynb, download this and save it in the directory on your PC where you want to work. 

Note python dependencies for this script are pandas and numpy which may need to be installed in your set up of Anaconda Navigator (see Environments). 

In the second cell of the script edit this line file_name_string = (r'C:\Users\mcveigh\Documents\PythonPC\AMRresults.txt') to point it to your path. All files should be saved and written to this same directory.

To execute the script you need to hit "shift" > "enter" in each block of code. Be sure to do this in order. 

Note writing the final file will overwrite any existing file with the same name. This behavior can be changed by simply changing the output file name in the final line of code here AMRresults.to_csv(r'AMRtable', sep ='\t', index = True). The script will fail to write the output if you have an existing file open with the same name. 

