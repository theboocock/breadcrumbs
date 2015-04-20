# Breadcrumbs 

## Motivation.

This project works to reconcile the disconnect between reproducibility and the pressure to publish.

A simple tool for command-line based programs basic starting commands are.

The tool adds no overhead to the workflow of a competent command-line user, but rather by using machine-leaning 
approaches to remove pointless commands run on the path of the directory you are breadcrumbing in. For instance,
excessive habitual use of the ls commands and other random commands cd's etc. Basically, stuff that is irrelevant to 
the project by working this out, you end up with a clear audit trail that tracks the analysis, couple this with git and
you can reproduce the entire workflow.  

## First step is to add the tracking function to your shell, in may case ZSH
```
function zshaddhistory() {
    echo "$(date "+%H:%M:%S") # ${PWD} # ${1%%$'\n'}" >> ~/test_history.zsh
}
```

This will date and save all the commands you run in a file test_history.zsh

Need two thngs for this to work.

Need be monitoring the test history, plus need to be monitoring the file system, each breadcrumb will be a process that gets started 
with the when you run breadcrumb start. It set's up file monitoring of the entire subdirectory and adds the new subdirectories when they 
get added.

## Reproducibl research.

As humanities research endevour has transitioned into the 21st century, computer-based projects are taking a larger and larger role. However, the tools associated with 

## Prototyping commands
Start a new breadcrumbs project
```bash
    breadcrumbs start --folder <folder> <name>
```
Stop a new breadcrumbs project 
```bash
    breadcrumbs stop <name> 
```

