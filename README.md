# ensf619project

## Setup

#### Clone the repository

    git clone https://github.com/madhuselvarajj/ensf619project.git
#### Navigate to the project directory:

    cd ensf619project

#### Create folder for the data:

    mkdir SignaTR6k
#### Transfer the image data (zip file) to this folder:
This folder is ignored in commits and will only be local

*Example only* (replace `firstname` and `lastname` and `path.from`: 
`rsync --verbose --progress --stats {path.from} {firstname}.{lastname}@talc.ucalgary.ca:/home/{firstname}.{lastname}/ensf619project`

#### Unzip image data into `SignaTR6k` folder

    unzip SignaTR6K.zip -d SignaTR6k

#### Create a virtual environment (if already created, skip to activating it):

    python -m venv venv


#### Activate the virtual environment:

    source venv/bin/activate


#### Install dependencies from requirements.txt:

    pip install -r requirements.txt

(This will install all the required libraries listed in the requirements.txt file)

#### Run the project:

    python eda.py



## Making Commits

#### Create a New Branch:

   Before making any changes, create a **new branch** for your work. Do not make changes in the local main branch.  Name the branch with your name .

       git checkout -b your-branch-name
   For example:

       git checkout -b firstname-eda

#### Make Your Changes, then commit them:

       git add .

       git commit -m "Your commit message"

#### Push Your Branch:

       git push origin your-branch-name

#### Create a Pull Request (PR):

   - Go to repository on GitHub.
   - Click on "Compare & pull request" for your branch.

## Updating local repo
Update Your Local Branch with Changes from Remote:

If there are new changes in the remote branch, you can fetch and merge them:

    git fetch origin 
    git merge origin/main

