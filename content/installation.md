# Installation

## General computing requirements

There are a few computing requirements for the course that are absolutely necessary (beyond the few software packages we would like you to install, described below):

1. You must have administrator access to your computer (i.e., you must be able to install things yourself without requesting IT approval).
2. If you are using Windows you must be using Windows 10; Windows 7 and 8 will not be sufficient for this course.

```{admonition} Disc space
You might want to have 40 GB of free disk space on your computer to install all the software and data required in the workshop.
```

If you foresee any of these being a problem please reach out on the Discord server for what steps you can take to ensure you are ready for when the course starts.

## Required software

To get the most out of our course, we ask you to install the following software:

  - A command-line shell: Bash
  - A version control system: Git
  - A text editor for coding: VSCode
  - Python 3 via Miniconda

:::{note}
Miniconda and VSCode are not strictly required, if you already have python and prefer to use pip, or if you already have a favorite text editor for programming, feel free to use that instead.
:::

If you already have all of the above software tools/packages installed, or are confident you’ll be able to install them by the time the course starts, you can jump straight to checking your install. The rest of this page provides more detail on installation procedures for each of the above elements, with separate instructions for each of the three major operating systems (Windows, Mac OS, and Linux).

## OS-specific installation instructions

Select the tab that corresponds to your operating system and follow the instructions therein.

Note: If the instructions below aren't working and you have spent more than 15-20 minutes troubleshooting on your own, reach out on the #installation-and-set-up channel on the Discord server with the exact problems you're having.


### Bash shell

````{tab-set}
```{tab-item} Windows

**Windows Subsystem for Linux (WSL)**

1. Search for `Windows Powershell` in your applications; right click and select `Run as administrator`. Select Yes on the prompt that appears asking if you want to allow the app to make changes to your device.

2. Type the following into the `Powershell` and then press `Enter`:

    `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

3. Press `Enter` again when prompted to reboot your computer.

4. Once your computer has rebooted, open the Microsoft Store and search for “Ubuntu.” Install the program labelled “Ubuntu 18.04” (not “Ubuntu 16.04” or “Ubuntu”) by clicking the tile, pressing `Get`, and then `Install`.

5. Search for and open `Ubuntu` from your applications. There will be a slight delay (of a few minutes) while it finishes installing.

6. You will be prompted to enter new UNIX username. You can use any combination of alphanumeric characters here for your username, but a good choice is `<first_initial><last_name>` (e.g., `jsmith` for John Smith). You will then be prompted to enter a new password. (Choose something easy to remember as you will find yourself using it frequently.)

7. Right click on the top bar of the Ubuntu application and select `Properties`. Under the `Options` tab, under the `Edit Options` heading, make sure the box reading `Use Ctrl+Shift+C/V as Copy/Paste` is checked. Under the `Terminal` tab, under the `Cursor Shape` heading, make sure the box reading `Vertical Bar` is checked. Press `Okay` to save these settings and then exit the application.

From this point on whenever the instructions specify to `open a terminal` please assume you are supposed to open the Ubuntu application.
```

```{tab-item} Mac OS
You already have it! Depending on which version of Mac OS you’re running you may need to type `bash` inside the terminal to access it. To check whether this is necessary, follow these steps:

- Open a terminal and type `echo $SHELL`. If it reads `/bin/bash` then you are all set!

Note that if you are using Mac Catalina (10.15.X) then it is possible your default shell is NOT CORRECT. To set the default to `bash`, type `chsh -s /bin/bash` in the terminal, enter your password when prompted, and then close + re-open the terminal.
```

```{tab-item} Linux
You already have it! Depending on which version of Linux you’re running you may need to type bash inside the terminal to access it. To check whether this is necessary, follow these steps:

- Open a terminal and type `echo $SHELL`. If it reads `/bin/bash` then you are all set!
- If not, whenever the instructions read “open a terminal,” please assume you are to open a terminal, type `bash`, and the proceed with the instructions as specified.
```
````

### Git

````{tab-set}
```{tab-item} Windows
You already have it, now that you’ve installed the WSL!
```

```{tab-item} Mac OS
You may already have it! Try opening a terminal and typing `git --version`. If you do not see something like `git version X.XX.X` printed out, then follow these steps:

1. Follow this link to automatically download an installer.

2. Double click the downloaded file (`git-2.23.0-intel-universal-mavericks.dmg`) and then double click the `git-2.23.0-intel-universal-mavericks.pkg` icon inside the dmg that is opened.

3. Follow the on-screen instructions to install the package
```

```{tab-item} Linux
You may already have it; try typing `sudo apt-get install git` (Ubuntu, Debian) or `sudo yum install git` (Fedora) inside the terminal.

If you are prompted to install it follow the instructions on-screen to do so.
```
````

### VSCode
There are many options to edit code. Below are instructions to install VSCode. If you do not already have a text editor for coding and looking for options, this could be a good choice.
````{tab-set}
```{tab-item} Windows
1. Go to https://code.visualstudio.com/ and click the download button, then run the `.exe` file.
2. Leave all the defaults during the installation with the following exception:
Please make sure the box labelled “Register Code as an editor for supported file types” is selected
```

```{tab-item} Mac OS
1. Go to https://code.visualstudio.com/ and click the download button.
2. Unzip the downloaded file (e.g., VSCode-darwin-stable.zip) and moving the resulting Visual Studio Code file to your Applications directory
```

```{tab-item} Linux
1. Go to https://code.visualstudio.com/ and click the download button for either the `.deb` (Ubuntu, Debian) or the `.rpm` (Fedora, CentOS) file.
2. Double-click the downloaded file to install VSCode. (You may be prompted to type your administrator password during the install).
```
````

#### VSCode extensions

````{tab-set}
```{tab-item} Windows
1. Open the Ubuntu application.
2. Type code . into the terminal and press Enter. You should see a message reading “Installing VS Code Server” and then a new windows will open up.
3. Press Ctrl+Shift+P in the new window that opens and type “Extensions: Install extensions” into the search bar that appears at the top of the screen. Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads “Extensions: Install extensions”).
4. A new panel should appear on the left-hand side of the screen with a search bar. Search for each of the following extensions and press Install for the first entry that appears. (The author listed for all of these extensions should be “Microsoft”.)
    - Python (n.b., you will need to reload VSCode after installing this)
    - Docker
    - Remote - WSL
```
```{tab-item} Mac OS

1. Open the Visual Studio Code application
2. Type Cmd+Shift+P and then enter “Shell command: Install ‘code’ command in PATH” into the search bar that appears at the top of the screen. Select the highlighted entry. A notification box should appear in the bottom-right corner indicating that the command was installed successfully.
3. Type Cmd+Shift+P again and then enter “Extensions: Install extensions” into the search bar. Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads “Extensions: Install extensions”).
4. A new panel should appear on the left-hand side of the screen with a search bar. Search for each of the following extensions and press Install for the first entry that appears. (The author listed for all of these extensions should be “Microsoft”.)
    - Python (n.b., you will need to reload VSCode after installing this)
    - Docker
```
```{tab-item} Linux
1. Open the Visual Studio Code application.
2. Press Ctrl+Shift+P in the new window that opens and type “Extensions: Install extensions” into the search bar that appears at the top of the screen. Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads “Extensions: Install extensions”).
3. A new panel should appear on the left-hand side of the screen with a search bar. Search for each of the following extensions and press Install for the first entry that appears. (The author listed for all of these extensions should be “Microsoft”.)
    - Python (n.b., you will need to reload VSCode after installing this)
    - Docker
```
````

### Python
All the hands-on components of the training use Python.
````{tab-set}
```{tab-item} Windows

1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

    ```
    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    bash Miniconda3-latest-Linux-x86_64.sh
    ```

2. A license agreement will be displayed and the bottom of the terminal will read `--More--`. Press `Enter` or the space bar until you are prompted with `Do you accept the license terms? [yes|no].` Type `yes` and then press `Enter`

3. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`). Leave this default and press `Enter`.

4. When you are asked `Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no],` type `yes` and press `Enter`. Exit the terminal once the installation has finished.

5. Re-open the Ubuntu application. Type which python into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).
    :::{tip}
    If you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step.
    If your issue is still not resolved skip the following step and contact an instructor.
    :::

6. Type the following to remove the installation script that was downloaded:

    ```
    rm ./Miniconda3-latest-Linux-x86_64.sh
    ```
```

```{tab-item} Mac OS
1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:
    ```
    curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
    bash Miniconda3-latest-MacOSX-x86_64.sh
    ```
2. A license agreement will be displayed and the bottom of the terminal will read `--More--`. Press `Enter` or the space bar until you are prompted with `Do you accept the license terms? [yes|no].` Type `yes` and then press `Enter`

3. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`). Leave this default and press `Enter`.

4. When you are asked `Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no],` type `yes` and press `Enter`. Exit the terminal once the installation has finished.

5. Re-open a terminal. Type which python into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).

    :::{tip}
    If you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step.
    If your issue is still not resolved skip the following step and contact an instructor.
    :::

6. Type the following to remove the installation script that was downloaded:
    ```
    rm ./Miniconda3-latest-MacOSX-x86_64.sh
    ```
```

```{tab-item} Linux
1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:
    ```
    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    bash Miniconda3-latest-Linux-x86_64.sh
    ```
2. A license agreement will be displayed and the bottom of the terminal will read `--More--`. Press `Enter` or the space bar until you are prompted with `Do you accept the license terms? [yes|no]`. Type `yes` and then press `Enter`

3. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`). Leave this default and press `Enter`.

4. When you are asked `Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no],` type `yes` and press `Enter`. Exit the terminal once the installation has finished.

5. Re-open a new terminal. Type which python into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`). Tip: if you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step. If your issue is still not resolved skip the following step and contact an instructor.

6. Type the following to remove the installation script that was downloaded:
    ```
    rm ./Miniconda3-latest-Linux-x86_64.sh
    ```
```
````

#### Python packages

````{tab-set}
```{tab-item} Windows

Open a terminal and type the following commands:

    conda config --append channels conda-forge
    conda config --set channel_priority strict
    conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn tensorflow keras pytorch torchvision torchaudio cpuonly -c pytorch
```
```{tab-item} Mac OS
Open a terminal and type the following commands:

    conda config --append channels conda-forge
    conda config --set channel_priority strict
    conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn tensorflow keras pytorch torchvision torchaudio -c pytorch
```
```{tab-item} Linux
Open a terminal and type the following commands:

    conda config --append channels conda-forge
    conda config --set channel_priority strict
    conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn tensorflow keras pytorch torchvision torchaudio cpuonly -c pytorch
```
````

## Checking your install

Now that you've installed everything it's time to check that everything works as expected! Type the following into your terminal:

```bash
bash <( curl -s https://raw.githubusercontent.com/main-educational/main-educational.github.io/main/content/main_educational_check_install.sh )
```

If you installed everything correctly you should see a message informing you as such. If any problems were detected you should receive some brief instructions on what is wrong with potential suggestions on how to remedy it. If you followed these instructions step-by-step and cannot resolve the issue please contact one of the course instructors for more help.
