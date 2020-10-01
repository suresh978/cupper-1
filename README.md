# Cupper
Introduction--
The meaning of Cupper's name is be better than common user passwords profiler (cupp). At the time of V1.0, I was determined to make this tool the best social work password generator in China. Until now, there is no independent latest tool for generating social work passwords in China. After half a year, the V2.0 version is finally completed. Compared with the first version, the functions of this version have been greatly improved. This tool will continue to be updated in the future. Hope this tool can play a positive role in your study and penetration testing.

Cupper allows for the update of services that are created using cookiecutter. When run, it creates a new branch that contains the latest cookiecuttered code, using a JSON file with context that matches the existing service. This file can be created through cookiecutter with the following contents:

`{{ cookiecutter | jsonify }}`

The script takes two arguments: a JSON file containing configuration for cookiecutter, and the name of the branch to create.

`cupper .cookiecutter.json template`

You can then merge these changes into your existing code:

`git merge template`

This code is heavily based on https://github.com/aroig/cookiecutter-latex-paper/blob/master/make/cookiecutter-update.py, with a few very small changes. 

Note that you will need a recent version of git for this to work (it needs --no-checkout on git worktree)
