This is a very simple project to automate the process of organizing files in the download folder in MacOS. This project has script written in python. 

## Automation & Python
### Organizing files in Download Folder

This project is a very simple project which just contains a puthon script to automate the process of moving downloaded files to different folders according to the file type. 
Eg. If you have demo.jpg image downloaded in the Downloads folder this script will auomatically move that to Downloads/images folder and in the same way it moves other file type to there respective folders like .docx/.pdf/.txt files to Downloads/documents folder and so on. 

#### Technical Details:
This script uses two python modules named os and shutil
- OS module provides functions to interact with operating system and provides a portable way of using os dependent functionalities. Interacting with file system is an example.
- Shutil is again a python module which offers number of high level operations on files and collection of files. It provides us functions which supports copying, moving and removal of files. 

#### How to run:
To run the program first make sure you have following things done
- Python3 installed
- Your automation.py should be in the Downloads folder
- Five folders created in Downloads folder named as images, documents, softwares, others, and Log(It will just contain a single file named log.txt which will be the output of the script)

Now, to run the script, go to the Downloads folder and execute the following command in the terminal 
`python3 automation.py >>~/Downloads/Log/log.txt`

Now, to make this script a cronjob and run it automatically after a certain interval of time follow the instructions either in cronjob.md file or in this article:
https://medium.com/swlh/automation-python-organizing-files-5d2b6b933402?source=friends_link&sk=da95bd01abb41776dd9230a72ba8f193

