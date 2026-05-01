# projLaunch

* I wrote this for a very specific use-case.

* I have all my projects in either a folder called GitHub or a folder called Git. 

* Essentially all my projects, use three programs: LyX, OneNote and VS Code.

* This essentially allows me to launch all the relevant files using one command. 

NB: Since I am on MacOS, this is only designed to work there. 

## Setup

1. Fork the repository (sorry, haven't had the time to homebrew it), and clone it. Forking allows you to keep things in sync if you plan to use it on different machines.

2. 
    Wherever you cloned it, make sure you have a file called 
    ```config```
    in the home directory and specify the following (customise as needed)
    ```
    DIR_projLaunch="/Users/incompetence/Documents/GitHub/projLaunch"
    DIR_Git="/Users/incompetence/Documents/Git"
    DIR_GitHub="/Users/incompetence/Documents/GitHub"
    ```
    The first entry specifies where all your project launching scripts are (see the examples folder for inspiration)

    The last two entries are optional---I use them in my own scripts. You can add your own. 

    Separating the paths is helpful if you have the same projects but on different machines.


## Usage

You should now be able to launch

```projLaunch```

from the terminal and select which project you want to open. It should open all the files associated with it.