# projLaunch

* I wrote this for a very specific use-case.

* I have all my projects in either a folder called GitHub or a folder called Git. 

* Essentially all my projects, use three programs: LyX, OneNote and VS Code.

* This essentially allows me to launch all the relevant files using one command. 

NB: Since I am on MacOS, this is only designed to work there. 

## Setup

1. Fork the repository (sorry, haven't had the time to homebrew it), and clone it. Forking allows you to keep things in sync if you plan to use it on different machines.

2. 
    Edit the `config.conf` file (that by default contains the following, you can customise as needed)
    ```
    DIR_projLaunch="/Users/incompetence/Documents/GitHub/projLaunch"
    DIR_Git="/Users/incompetence/Documents/Git"
    DIR_GitHub="/Users/incompetence/Documents/GitHub"
    ```
    and then copy it as shown
    
    ```mkdir ~/.config/projLaunch && cp config.conf ~/.config/projLaunch/config.conf```
    
    In the `config.conf` file, the first entry specifies where all your project launching scripts are (see the examples folder for inspiration)

    The last two entries are optional---I use them in my own scripts. You can add your own. 

    Separating the paths is helpful if you have the same projects but on different machines.

3. 
    Add it to the environment so you don't have to cd your way into projLaunch. 
    For instance, something like the following
    ```sudo ln -s /location/to/where/you/cloned/projLaunch/projLaunch /usr/local/bin/projLaunch```
## Usage

You should now be able to launch

```projLaunch```

from the terminal and select which project you want to open. It should open all the files associated with it.