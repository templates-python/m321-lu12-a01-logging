# Python-Template (Version 2023)
## Introduction
This is the python template we use in our programming classes. It contains:
- main.py: Simple script
- main_test.py: A single pytest-case
- .gitignore: Used to exclude PyCharm settings and venv
- requirements.txt: Basic requirements for python and pytest
## Workflows
### classroom.yml
This workflow contains a number of jobs for the automation of classroom assignments.
#### setup
Runs only when the repository is first created by a push of 'classroom bot'.
It triggers a workflow that copies the issues from a source repository into the students repos.
#### grading
Does not run when the repository is first created by 'classroom bot'.
It triggers a workflow for autograding using the tests in /.github/classroom/autograding.json

### copyissues.yml
The workflow to copy the issues with manual trigger.
