# Template directory for Kicad 7+ PCB project

Note: For instructions on how to use libraries, see the [readme.md](https://github.com/eduardobehr/Kicad_PCB_Project_Template/tree/main/libs#libraries) in the `libs` directory

## Requirements

* Git (e.g. TortoiseGit)
* Kicad 7+

## Usage

Note: all commands below assume the use of a Unix shell (bash, zsh, etc).

1. Navigate to the desired directory to create your project

```sh
# define new folder name
PROJECTS_DIR=Kicad_Projects

# create new folder with the name given above
mkdir -p $PROJECTS_DIR

# navigate to new folder
cd $PROJECTS_DIR
```

2. Clone this template repository:

```sh
git clone --recursive https://github.com/eduardobehr/Kicad_PCB_Project_Template.git
cd Kicad_PCB_Project_Template
```
3. Delete the hidden `.git` folder
This action will unlink the directory from the template repository

```sh
rm -rf .git
```

4. Rename the kicad files and the main folder, if necessary:
    * `Kicad_PCB_Project_Template`
        * `Kicad_PCB_Project_Template.kicad_pro`
        * `Kicad_PCB_Project_Template.kicad_sch`
        * `Kicad_PCB_Project_Template.kicad_pcb`
        * `Kicad_PCB_Project_Template.kicad_prl`

5. Create a new repository to track changes to the new project

```sh
git init
```

This will create a new `.git` folder to allow Git to track the project

## Git basics

List current state:

```sh
git status
```

Add files to the staging area (prepare to commit them):

```sh
git add <file>
# to add all, use 'git add --all'
```

Commit (save) changes to repository:

```sh
git commit --message "Changed X and Y"
```

Upload changes to remote repository

```sh
git push
```

Download changes from remote repository

```sh
git pull
```

See history of commits:

```sh
git log --all --oneline --graph
```


