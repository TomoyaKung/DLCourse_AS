# DLCourse_AS
DeepLearning Course Assignments

1. Assignment1: [deadline: 2016/11/04 24:00]
 
 svm.ipynb => softmax.ipynb => two_layer_net.ipynb

2. Assignment2: [deadline: 2016/12/09 24:00]

 FullyConnectedNets.ipynb => BatchNormalization.ipynb => Dropout.ipynb => ConvolutionalNetworks.ipynb


# Introduction

 DeepLearning Course Home Page: [https://speechlab.sjtu.edu.cn/~kyu/node/7](https://speechlab.sjtu.edu.cn/~kyu/node/7)

These assignments are retrieved and modified from the assignments of [CS231n](http://cs231n.github.io/). Some contents are deleted from their assignments and we also extended additional contents according to needs of our DeepLearning Course.

For each assignment, you should complete and hand in completed worksheet (including its outputs and any supporting code outside of the worksheet) with your assignment submission. If you encounter any difficulties, you may refer to the course notes of [CS231n](http://cs231n.github.io/) to get some inspiration.

Required tools: Python 2.7+, Jupyter Notebook.

## Setup your workspace locally.

### Step 1
**[Option 1: Use Anaconda]:** The preferred approach for installing all the assignment dependencies is to use [Anaconda](https://www.continuum.io/downloads), which is a Python distribution that includes many of the most popular Python packages for science, math, engineering and data analysis. Once you install it you can skip all mentions of requirements and you’re ready to go directly to working on the assignment.

**[Option 2: Manual install, virtual environment]:** If you’d like to (instead of Anaconda) go with a more manual and risky installation route you will likely want to create a [virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/) for the project. If you choose not to use a virtual environment, it is up to you to make sure that all dependencies for the code are installed globally on your machine.

Let's take assignment1 for example. To set up a virtual environment, run the following:

```bash
cd assignment1
sudo pip install virtualenv      # This may already be installed
virtualenv .env                  # Create a virtual environment
source .env/bin/activate         # Activate the virtual environment
pip install -r requirements.txt  # Install dependencies
# Work on the assignment for a while ...
deactivate                       # Exit the virtual environment
```

### Step 2
**[Download data]:** Once you have the starter code, you will need to download the CIFAR-10 dataset. Run the following from the `assignment1` directory:

```bash
cd cs231n/datasets
./get_datasets.sh
```

### Step 3
**[Start Jupyter Notebook]:** After you have the CIFAR-10 data, you should start the Jupyter notebook server from the `assignment1` directory. If you are unfamiliar with Jupyter, you can refer to [Installing Jupyter Notebook](http://jupyter.readthedocs.io/en/latest/install.html) and [Running the Notebook](https://jupyter.readthedocs.io/en/latest/running.html#running).

for example, you may begin working on your assignment like this:
```bash
cd assignment1
jupyter notebook --port=5000
# Your browser will open a webpage for you to work on. If not, open 'localhost:5000' by yourselves.
# Click '*.ipynb' in the list displayed in the webpage, remember to keep the outputs of those code cells.
```

**[NOTE]:** If you are working in a virtual environment on OSX, you may encounter errors with matplotlib due to the issues described [here](http://matplotlib.org/faq/virtualenv_faq.html). You can work around this issue by starting the IPython server using the `start_ipython_osx.sh` script from the `assignment1` directory; the script assumes that your virtual environment is named `.env`.


## Submit your work.

Once you are done working run the `collectSubmission.sh` script; this will produce a file called `assignment1.zip`. Rename it to `StudentID-StudentName-AssignmentID.zip`(for example, `12345-小明-as1.zip`). 

Upload your assignments to corresponding folder in `ftp://202.120.38.125`. Public account: `dl2016`/`dl2016`.
