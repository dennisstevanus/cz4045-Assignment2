# CZ4045 Assignment 2
In this github repository there are 2 different subtasks:
1.  FNN Neural Language Model
2.  Named Entity Recognition (NER)


Installation
------------
Below are step by step guide to clone this repository and install the required library used.
1.  Make sure you've installed git in your computer. (Note: Skip to step 4 if you already have the code from the submission zip and just open a terminal in the source code directory instead.)
2.  Clone this specific repository. 
    1. If you have the Github Desktop, just find the "Clone Repository" in the File menu and enter this "https://github.com/dennisstevanus/cz4045-Assignment2.git".
    2. If you are using Github from terminal, you can just enter this code `git clone https://github.com/dennisstevanus/cz4045-Assignment2.git`.
3.  Go to the the repository directory. For example, after running the step 2.2 above, you can use `cd cz4045-Assignment2` from the terminal. This will be referred as `project root directory`. 
4.  Setup an virtual environment (optional). 
    The following are the tutorial on how to setup venv on Unix machine. For windows or more information, see this [link](https://docs.python.org/3/tutorial/venv.html)
    1. Making the the virtual environment:
        run this on terminal `python3 -m venv venv`
    2. Activate the Virtual environment `source venv/bin/activate`
5.  Install the required library by running this in terminal `pip install -r requirements.txt`
6.  Setup the `PYTHONPATH` to include `project root directory` in the the `PYTHONPATH`. Tutorial on how to set this up is on this [link](https://bic-berkeley.github.io/psych-214-fall-2016/using_pythonpath.html). 
    Otherwise, it can also be done by using `PyCharm IDE` and then using the IDE's [code run assistance](https://www.jetbrains.com/help/pycharm/code-running-assistance-tutorial.html) which by default add `project root directory` to the `PYTHONPATH`. 

Note: You may need to install a specific version of [Pytroch](https://pytorch.org/) based on your Computer environment(GPU availability, CUDA version, etc.).
Therefore, please head directly to the [installation guide](https://pytorch.org/get-started/locally/) from the website to install it based on your environment. 


Content information
------------
The following is the general folder structure of this project: 
*   `question_1`: Contains all the source codes, resources, and user guide for the first question in the assignment, 
which is regarding FNN Neural Language Model
*   `question_2`: Contains all the source codes, resources, and user guide for the second question in the assigment, 
which is regarding Named Entity Recognition (NER). 

Please head directly to each folder and read the `README.md` provided listed above for further guide on how to run the applications. 

Error troubleshooting
------------
*   If you encountered `ImportError` messages, most likely you have missed Installation step 5. Please do the instructions described in step 5.
*   If you encountered `ModuleNotFoundError` messages like this: 
    ```
    ModuleNotFoundError: No module named 'data'
    ```
    most likely you have not done the Installation step 6. Please do the instructions described in step 6.
