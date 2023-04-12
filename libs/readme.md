# Libraries

Use this directory to store libraries, which will be referenced to the project by relative path (allowing for use in multiple machines)

# Adding Library

### Place the library files

There are two ways to accomplish this:

* Copy the library to this folder
* Add a Git submodule inside this folder

### Link library to Kicad

As an example, for the schematic editor (Eeschema):

1. Go to: Preferences > Manage Symbol Libraries
2. Click on the "Project Specific Libraries"
3. Click on the "+" button to add a library link
4. Enter a nickname
5. Choose the corresponding file placed on the previous step (submodule or local copy)
After doing these steps, your library should be linked at `${KIPRJMOD}/libs/...`, where `${KIPRJMOD}` resolves to the path of the current project

6. Press OK and save the schematic




