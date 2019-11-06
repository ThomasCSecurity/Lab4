# RIT CSEC465 Lab4 (Fall 2019)
[![_License_: 2-clause BSD License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause "2-clause BSD License")
[![Build Status](https://travis-ci.org/2191-CSEC465-Group6/Lab4.svg?branch=master)](https://travis-ci.org/2191-CSEC465-Group6/Lab4)

## Creating a new role using Ansible Molecule
To keep roles consistent, we are using Ansible Molecule to create and test our roles.

First, install Ansible Molecule
```
pip install --user molecule
```

Next, create a new role
```
molecule init role --role-name <your-new-role>
```

Then, remove the `meta/` directory from your new role since we're not submitting our roles to Ansible Galaxy
```
rm -rf roles/<your-new-role>/meta/
```
