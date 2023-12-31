# Data Manipulation using notebooks in colab [![Test](https://github.com/nogibjj/DukeIDS706_ds655_Week09/actions/workflows/04_Test.yml/badge.svg)](https://github.com/nogibjj/DukeIDS706_ds655_Week09/actions/workflows/04_Test.yml)


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nogibjj/DukeIDS706_ds655_Week09/blob/main/Codes/Data_Manipulation.ipynb)

Performing basic data manipulations such as data merging in Python. 


There are several reasons to use Colab for Python projects:

**Free and cloud-based:** Colab is a free, cloud-based platform that allows you to run Python code without having to install any software on the local machine.

**Easy to use:** Colab has a user-friendly interface that makes it easy to write, run, and share Python code.

**Integrated with Google Drive:** Colab is integrated with Google Drive, which means you can easily save and share your notebooks with others.

**Access to powerful hardware:** Colab provides access to powerful hardware, including GPUs and TPUs, which can significantly speed up the execution of your code.

**Support for popular libraries:** Colab comes pre-installed with many popular Python libraries, including NumPy, Pandas, and Matplotlib, making it easy to get started with data analysis and machine learning.

**Collaboration:** Colab allows you to collaborate with others in real-time, making it a great tool for team projects.

Overall, Colab is a great platform for anyone who wants to write and run Python code without having to worry about setting up a local development environment.





Files in this repository include:


## 1. Readme
  The `README.md` file is a markdown file that contains basic information about the repository, what files it contains, and how to consume them


## 2. Requirements
  The `requirements.txt` file has a list of packages to be installed for any required project. Currently, my requirements file contains some basic python packages.


## 3. Codes
  This folder contains all the code files used in this repository - the files named "Test_" will be used for testing and the remaining will define certain functions
  `Data_Manipulation.ipynb` is the main file that contains the code for data manipulation using pandas and numpy


## 4. Resources
  -  This folder contains any other files relevant to this project. Currently, I have added -


## 5. CI/CD Automation Files


  ### 5(a). Makefile
  The `Makefile` contains instructions for installing packages (specified in `requirements.txt`), formatting the code (using black formatting), testing the code (running all the sample python code files starting with the term *'Check...'* ), and linting the code using pylint


  ### 5(b). Github Actions
  Github Actions uses the `main.yml` file to call the functions defined in the Makefile based on triggers such as push or pull. Currently, every time a change is pushed onto the repository, it runs the install packages, formatting the code, linting the code, and then testing the code functions


  ### 5(c). Devcontainer
  
  The `.devcontainer` folder mainly contains two files - 
  * `Dockerfile` defines the environment variables - essentially it ensures that all collaborators using the repository are working on the same environment to avoid conflicts and version mismatch issues
  * `devcontainer.json` is a json file that specifies the environment variables including the installed extensions in the virtual environment
