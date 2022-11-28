# Welcome to the BBQ!

## What is BBQ?
BBQ is a utility script that provides management of testing scripts and results. It uses Git to manage storage of test files and results.

## Overview

BBQ is intended for Linux system that have Git installed and configured. Before you try to use BBQ, ensure that you can create a Git repository, 
and that you can add files and make commits.

The bbq script should be placed in the path of the user that will be running the testing scripts. A good place to put the script is in the ~/.local/bin directory. 
However, if multiple users on a system will be accesing the script, a centralized location is best.

Directories in which BBQ has been initialized will contain a .bbq directory. This directory is created by Git, and is (mostly) a standard .git diretory 
using a different name. Since BBQ uses the .bbq directory, you can use Git as you normally do on a BBQ directory without any change in functionality. However,
you should be aware of the BBQ context prior to using Git functions, and ensure that the desired file versions are present before adding or making commits.

BBQ also creates a .bbqRegister file in the home directory (this location can be changed in the script). This file contains a listing of all of the directories
where bbq has been initialized, and is used during the result collection and archive BBQ functions.

By default, BBQ creates and uses the ~/bbqArchive directory to store BBQ archives. This can be changed in the script.

## Commands

### Basic
CheckBBQ
snap
init
archive

### Movement
delete
list
load <dir>
main
results
scripts
whereami
tag <name>
listTags
  
### Processing
commands
run
process
first
next
previous
latest
  
### Register
editRegister
listRegister
