# There are 3 levels of git config; local, global and system.

# local: Local configs are only available for the current project and stored in .git/config in the project's directory.
# global: Global configs are available for all projects for the current user and stored in ~/.gitconfig.
# system: System configs are available for all the users/projects and stored in /etc/gitconfig.

# Create a local specific config, you have to execute this under the project's directory.
$ git config user.name "John Doe"

# Create a global config
$ git config --global user.name "John Doe"

# Create a system config
$ git config --system user.name "John Doe"

# Your identity

# Git configuration of user name and email adddress is important. Because each git commit uses this information. Following command used for this purpose:

$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com

# In specific project, if you want to overwrite user name and email address, you must config without global config. Because, global configuration affects entire project in your working repository in a computer.

# You can check user name and email address by following commands:

$ git config user.name

# Result for this command is:

John Doe

$ git config user.email

# Result for this command is:

johndoe@example.com

# You can view all your settings and where they come from with the following command:

$ git config --list --show-origin

# If you run above command, you can get:

file:/home/John/.gitconfig   user.email=johndoe@example.com
file:/home/John/.gitconfig   user.name=John Doe
file:/home/John/.gitconfig   core.editor=emacs
file:/home/John/.gitconfig   core.editor=vs
file:/home/John/.gitconfig   credential.helper=wincerd
file:.git/config        core.repositoryformatversion=0
file:.git/config        core.filemode=true
file:.git/config        core.bare=false
file:.git/config        core.logallrefupdates=true

# You can check your settings without file directory by following command:

$ git config --list

# If you run above command, you can get:

user.email=johndoe@example.com
user.name=John Doe
core.editor=emacs
core.editor=vs
credential.helper=wincerd
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true

# If you want to use other editor like emacs, you can do the following command:

# In Linux system,

$ git config --global core.editor emacs

# In Windows system,

$ git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"

# Otherwise your computer use default text editor
