# There are two ways to get git repository:

# * Turn not version controled local directory into Git repository
# * Clone a existing repository from anywhere

# * Turn not version controled local directory into Git repository:

# Step 1:

# To access project directory is different for different operating system:

# for Linux:

$ cd /home/user/my_project

# for macOS:

$ cd /Users/user/my_project

# for Windows:

$ cd C:/Users/user/my_project

# Step 2:

# Initialize git repository using following command:

$ git init

# Result for this command creates a new subdirectory named '.git' which contains all the necessary repository files. It can be used to convert an existing, unversioned project to a Git repository or initialize a new, empty repository.

# Step 3:

$ git add *.c
$ git add LICENSE

# This command adds corresponding file

# Step 4:

$ git commit -m 'Initial project version'

# This is a job to specify commit message when you are making commit 

# Git cloning:

# Clone a repository with "git clone <url>"

# Example01:

# If you want to clone libgit2, you can use following command:

$ git clone https://github.com/libgit2/libgit2

# It makes an exact copy of the entire repository on your local machine's 'libgit2' directory.

# Example02:

# If you want to clone libgit2, but not in same directory name.For that case you can use following command: 

$ git clone https://github.com/libgit2/libgit2 <new_directory_name>

# It makes an exact copy of the entire repository on your local machine's 'new' directory.

# There are differnt transfer protocols are available, you can use anyone of following this:

# * `https: //`

# * `git: //`

# * `user@server:path/to/repo.git`
