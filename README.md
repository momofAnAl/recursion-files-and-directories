# Recursive Data
Classroom activity to accompany the CS Fundamentals: Recursion topic.

## One-Time Activity Setup

Follow these directions once, at the beginning of the activity:


1. Navigate to the folder where you wish to save activities. This could be your `projects` folder, or you may want to create a new folder for all of your activities.

   If you followed Ada's recommended file system structure from the Intro to Dev Environment lesson in Learn, you can navigate to your projects folder with the following command:

   ```bash
   $ cd ~/Developer/projects
   ```

   Or, if you want to create a new folder for all of your activities:

   ```bash
   $ cd ~/Developer
   $ mkdir activities
   $ cd activities
   ```

   If you've already created an activities directory, you can navigate to it with the following command:

   ```bash
   $ cd ~/Developer/activities
   ```

2. In Github click on the "Fork" button to fork the repository to your Github account.  This will make a copy of the activity in your Github account. 

3. "Clone" the activity into your working folder. This command makes a new folder named for the activity repository, and then puts the activity into this new folder.

   ```bash
   $ git clone <clone_url_for_the_activity>
   ```

   The `<>` syntax indicates a placeholder. You should replace `<clone_url_for_the_activity>` with the actual URL you'd use to clone this repository. If you click the green "Code" button on the GitHub page for this repository, you'll see a URL that you can copy to your clipboard.
 
   Use `ls` to confirm there's a new activity folder

4. Move your location into this activity folder

   ```bash
   $ cd <repository_directory>
   ```

   The `<repository_directory>` placeholder should be replaced with the name of the activity folder. If you're not sure what the folder is named, remember that you can use `ls` to list the contents of your current location.

5. Create a virtual environment named `venv` for this activity:

   ```bash
   $ python3 -m venv venv
   ```

6. Activate this environment:

   ```bash
   $ source venv/bin/activate
   ```

   Verify that you're in a python3 virtual environment by running:
   
   - `$ python --version` should output a Python 3 version
   - `$ pip --version` should output that it is working with Python 3

7. Install dependencies once at the beginning of this activity with

   ```bash
   # Must be in activated virtual environment
   $ pip install -r requirements.txt
   ```

   Not all activities will have dependencies, but there will still be an included `requirements.txt` file.

Summary of one-time activity setup:
- [ ] Fork the activity repository
- [ ] `cd` into your working folder, such as your `projects` or `activities` folder
- [ ] Clone the activity onto your machine
- [ ] `cd` into the folder for the activity
- [ ] Create the virtual environment `venv`
- [ ] Activate the virtual environment `venv`
- [ ] Install the dependencies with `pip`

## Activity Development Workflow

1. When working on this activity, always ensure that your virtual environment is activated:

   ```bash
   $ source venv/bin/activate
   ```

2. If you want to work on another project from the same terminal window, you should deactivate the virtual environment when you are done working on the activity:

   ```bash
   $ deactivate
   ```

## Activity Directions

In this activity, we will be working with recursive functions. We will implement a few functions that will help build our understanding of recursion.

Recursion is often useful in cases where the underlying data structure is recursive. Directory structures are a good example of this. A directory can contain files and other directories. Each of those directories can contain files and other directories, and so on. This is a recursive data structure.

Since the data structure is recursive, it makes sense to use recursion to traverse it. In this activity, we will be working with a simple directory structure. We will implement a few functions that will help us traverse this structure.

`main.py` defines a small directory structure, `my_dir`. This directory structure is passed to a few functions that we will implement.

Introductory functions:

`print_files`: This function should print the names of all files in the directory structure. It should not print the names of directories.

`print_dirs`: This function should print the names of all directories in the directory structure. It should not print the names of files.

Challenging function:

`print_indented`: This function should print the names of all files and directories in the directory structure. It should print the names of directories indented by a number of spaces proportional to the depth of the directory in the structure.

Ultra bonus function:

`print_tree`: This function should print the names of all files and directories in the directory structure. It should print the names of directories indented by a number of spaces proportional to the depth of the directory in the structure. It should also print a tree-like structure to represent the directory structure.

Super duper challenge function:

`dirtree`: This function is the real deal. Given an actual path, it should use recursion to print the names of all files and directories in the directory structure. It should print the names of directories indented by a number of spaces proportional to the depth of the directory in the structure. It should also print a tree-like structure to represent the directory structure.

Refer to the comments in `main.py` for more information on each function.