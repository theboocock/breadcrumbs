# Breadcrumbs 

## Motivation.

This project works to reconcile the disconnect between reproducibility and the pressure to publish.

A simple tool for command-line based programs basic starting commands are.

The tool adds no overhead to the workflow of a competent command-line user, but rather by using machine-leaning 
approaches to remove pointless commands run on the path of the directory you are breadcrumbing in. For instance,
excessive habitual use of the ls commands and other random commands cd's etc. Basically, stuff that is irrelevant to 
the project by working this out, you end up with a clear audit trail that tracks the analysis, couple this with git and
you can reproduce the entire workflow.  


## Prototyping commands
Start a new breadcrumbs project
```bash
    breadcrumbs start --folder <folder> <name>
```
Stop a new breadcrumbs project 
```bash
    breadcrumbs stop <name> 
```

