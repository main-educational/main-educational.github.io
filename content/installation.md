# Installation

> Instructions to install and setup all the tools required for the MAIN 2021 educational.

## General computing requirements

There are a few computing requirements for the course that are absolutely necessary (beyond the few software packages we would like you to install, described below):

1. You must have administrator access to your computer (i.e., you must be able to install things yourself without requesting IT approval).
2. You must have at least 40 GB of free disk space on your computer (but we would recommend more, to be safe).
3. If you are using Windows you must be using Windows 10; Windows 7 and 8 will not be sufficient for this course.

If you foresee any of these being a problem please reach out to one of the instructors for what steps you can take to ensure you are ready for the course start on November 25th.

## Required software

To get the most out of our course, we ask you to install the following software:

  - A command-line shell: Bash
  - A version control system: Git
  - A remote-capable text editor: VSCode
  - Python 3 via Miniconda
  - A virtualization system: Docker
  - A GitHub account
  - A modern browser

:::{note}
Miniconda and VSCode are not strictly required, if you already have python and prefer to use pip, or if you already have a favorite text editor for programming, feel free to use that instead.
:::

If you already have all of the above software tools/packages installed, or are confident you’ll be able to install them by the time the course starts, you can jump straight to checking your install. The rest of this page provides more detail on installation procedures for each of the above elements, with separate instructions for each of the three major operating systems (Windows, Mac OS, and Linux).

## OS-specific installation instructions

Select the tab that corresponds to your operating system and follow the instructions therein.

Note: If the instructions below aren't working and you have spent more than 15-20 minutes troubleshooting on your own, reach out on the #help-installation channel on the BHS Discord with the exact problems you're having.


### Bash shell
```{tabbed} Windows

**Windows Subsystem for Linux (WSL)**

1. Search for `Windows Powershell` in your applications; right click and select `Run as administrator`. Select Yes on the prompt that appears asking if you want to allow the app to make changes to your device.

2. Type the following into the `Powershell` and then press `Enter`:

    `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

3. Press `Enter` again when prompted to reboot your computer.

4. Once your computer has rebooted, open the Microsoft Store and search for “Ubuntu.” Install the program labelled “Ubuntu 18.04” (not “Ubuntu 16.04” or “Ubuntu”) by clicking the tile, pressing `Get`, and then `Install`.

5. Search for and open `Ubuntu` from your applications. There will be a slight delay (of a few minutes) while it finishes installing.

6. You will be prompted to enter new UNIX username. You can use any combination of alphanumeric characters here for your username, but a good choice is `<first_initial><last_name>` (e.g., `jsmith` for John Smith). You will then be prompted to enter a new password. (Choose something easy to remember as you will find yourself using it frequently.)

7. Right click on the top bar of the Ubuntu application and select `Properties`. Under the `Options` tab, under the `Edit Options` heading, make sure the box reading `Use Ctrl+Shift+C/V as Copy/Paste` is checked. Under the `Terminal` tab, under the `Cursor Shape` heading, make sure the box reading `Vertical Bar` is checked. Press `Okay` to save these settings and then exit the application.

(The above step-by-step WSL instructions are distilled from here and here. If you have questions during the installation procedure those resources may have answers!)

From this point on whenever the instructions specify to `open a terminal` please assume you are supposed to open the Ubuntu application.
```
```{tabbed} Mac OS
You already have it! Depending on which version of Mac OS you’re running you may need to type bash inside the terminal to access it. To check whether this is necessary, follow these steps:

- Open a terminal and type `echo $SHELL`. If it reads `/bin/bash` then you are all set!

Note: If you are using Mac Catalina (10.15.X) then it is possible your default shell is NOT CORRECT. To set the default to `bash`, type `chsh -s /bin/bash` in the terminal, enter your password when prompted, and then close + re-open the terminal.
```
```{tabbed} Linux
You already have it! Depending on which version of Linux you’re running you may need to type bash inside the terminal to access it. To check whether this is necessary, follow these steps:

- Open a terminal and type `echo $SHELL`. If it reads `/bin/bash` then you are all set! 
- If not, whenever the instructions read “open a terminal,” please assume you are to open a terminal, type `bash`, and the proceed with the instructions as specified.
```

### Git

```{tabbed} Windows
You already have it, now that you’ve installed the WSL!
```

```{tabbed} Mac OS
You may already have it! Try opening a terminal and typing `git --version`. If you do not see something like `git version X.XX.X` printed out, then follow these steps:

Follow this link to automatically download an installer.

Double click the downloaded file (`git-2.23.0-intel-universal-mavericks.dmg`) and then double click the `git-2.23.0-intel-universal-mavericks.pkg` icon inside the dmg that is opened.

Follow the on-screen instructions to install the package
```

```{tabbed} Linux
You may already have it; try typing `sudo apt-get install git` (Ubuntu, Debian) or `sudo yum install git` (Fedora) inside the terminal. 

If you are prompted to install it follow the instructions on-screen to do so.
```

### VSCode

```{tabbed} Windows
1. Go to https://code.visualstudio.com/ and click the download button, then run the `.exe` file.
2. Leave all the defaults during the installation with the following exception:
Please make sure the box labelled “Register Code as an editor for supported file types” is selected
```

```{tabbed} Mac OS
1. Go to https://code.visualstudio.com/ and click the download button.
2. Unzip the downloaded file (e.g., VSCode-darwin-stable.zip) and moving the resulting Visual Studio Code file to your Applications directory
```

```{tabbed} Linux
1. Go to https://code.visualstudio.com/ and click the download button for either the `.deb` (Ubuntu, Debian) or the `.rpm` (Fedora, CentOS) file. 
2. Double-click the downloaded file to install VSCode. (You may be prompted to type your administrator password during the install).
```

#### VSCode extensions

```{tabbed} Windows
1. Open the Ubuntu application.
2. Type code . into the terminal and press Enter. You should see a message reading “Installing VS Code Server” and then a new windows will open up.
3. Press Ctrl+Shift+P in the new window that opens and type “Extensions: Install extensions” into the search bar that appears at the top of the screen. Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads “Extensions: Install extensions”).
4. A new panel should appear on the left-hand side of the screen with a search bar. Search for each of the following extensions and press Install for the first entry that appears. (The author listed for all of these extensions should be “Microsoft”.)
    - Python (n.b., you will need to reload VSCode after installing this)
    - Docker
    - Remote - WSL
```
```{tabbed} Mac OS

1. Open the Visual Studio Code application
2. Type Cmd+Shift+P and then enter “Shell command: Install ‘code’ command in PATH” into the search bar that appears at the top of the screen. Select the highlighted entry. A notification box should appear in the bottom-right corner indicating that the command was installed successfully.
3. Type Cmd+Shift+P again and then enter “Extensions: Install extensions” into the search bar. Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads “Extensions: Install extensions”).
4. A new panel should appear on the left-hand side of the screen with a search bar. Search for each of the following extensions and press Install for the first entry that appears. (The author listed for all of these extensions should be “Microsoft”.)
    - Python (n.b., you will need to reload VSCode after installing this)
    - Docker
```
```{tabbed} Linux
1. Open the Visual Studio Code application.
2. Press Ctrl+Shift+P in the new window that opens and type “Extensions: Install extensions” into the search bar that appears at the top of the screen. Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads “Extensions: Install extensions”).
3. A new panel should appear on the left-hand side of the screen with a search bar. Search for each of the following extensions and press Install for the first entry that appears. (The author listed for all of these extensions should be “Microsoft”.)
    - Python (n.b., you will need to reload VSCode after installing this)
    - Docker
```

### Python

```{tabbed} Windows

Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    bash Miniconda3-latest-Linux-x86_64.sh

A license agreement will be displayed and the bottom of the terminal will read `--More--`. Press `Enter` or the space bar until you are prompted with `Do you accept the license terms? [yes|no].` Type `yes` and then press `Enter`

The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`). Leave this default and press `Enter`.

When you are asked `Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no],` type `yes` and press `Enter`. Exit the terminal once the installation has finished.

Re-open the Ubuntu application. Type which python into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).
 - If you do not see a path like this then please try typing conda init, closing your terminal, and repeating this step. If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel on the BHS Slack.

Type the following to remove the installation script that was downloaded:

    rm ./Miniconda3-latest-Linux-x86_64.sh

```

```{tabbed} Mac OS
Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

    curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
    bash Miniconda3-latest-MacOSX-x86_64.sh

A license agreement will be displayed and the bottom of the terminal will read --More--. Press `Enter` or the space bar until you are prompted with “Do you accept the license terms? [yes|no].” Type yes and then press Enter

The installation script will inform you that it is going to install into a default directory (e.g., /home/$USER/miniconda3). Leave this default and press Enter.

When you are asked “Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no],” type yes and press Enter. Exit the terminal once the installation has finished.

Re-open a terminal. Type which python into the terminal and it should return a path (e.g., /home/$USER/miniconda3/bin/python).
 - If you do not see a path like this then please try typing conda init, closing your terminal, and repeating this step. If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel of the BHS Slack.

Type the following to remove the installation script that was downloaded:

    rm ./Miniconda3-latest-MacOSX-x86_64.sh

```

```{tabbed} Linux
Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    bash Miniconda3-latest-Linux-x86_64.sh

A license agreement will be displayed and the bottom of the terminal will read --More--. Press `Enter` or the space bar until you are prompted with “Do you accept the license terms? [yes|no].” Type yes and then press Enter

The installation script will inform you that it is going to install into a default directory (e.g., /home/$USER/miniconda3). Leave this default and press Enter.

When you are asked “Do you wish the installer to initialize Miniconda3 by running conda init? [yes|no],” type yes and press Enter. Exit the terminal once the installation has finished.

Re-open a new terminal. Type which python into the terminal and it should return a path (e.g., /home/$USER/miniconda3/bin/python). 
 - If you do not see a path like this then please try typing conda init, closing your terminal, and repeating this step. If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel of the BHS Slack.

Type the following to remove the installation script that was downloaded:

    rm ./Miniconda3-latest-Linux-x86_64.sh

```


#### Python packages

```{tabbed} Windows

Open a terminal and type the following commands:

    conda config --append channels conda-forge
    conda config --set channel_priority strict
    conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn
```
```{tabbed} Mac OS
Open a terminal and type the following commands:

    conda config --append channels conda-forge
    conda config --set channel_priority strict
    conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn
```
```{tabbed} Linux
Open a terminal and type the following commands:

    conda config --append channels conda-forge
    conda config --set channel_priority strict
    conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn
```

### Docker
```{tabbed} Windows

Unfortunately, Docker for Windows is a bit of a mess. The recommended version of Docker to install varies dramatically depending not only on which version of Windows you have installed (e.g., Windows 10 Home versus Professional/Enterprise/Education), but also which build of Windows you have. As such, developing a comprehensive set of instructions for installing Docker is rather difficult.

For this course, you will need to install either Docker Toolbox for Windows or Docker for Windows Desktop. Which you install will depend on your OS. PLEASE NOTE that installing Docker for Windows Desktop will disable VirtualBox on your computer. If you actively use VirtualBox we recommend you install Docker Toolbox.

(Note: the below instructions assume you are installing Docker Toolbox. Because there are fewer requirements for Docker Toolbox, it is likely that you will be able to install this more easily.)

Download the latest Docker Toolbox installer (note: that link will automatically download the file)

Run the downloaded .exe file and leave all the defaults during the installation procedure. Click Yeson the prompt that appears asking if the application can make changes to your computer.

Search for and open the newly-installed “Docker Quickstart” application. Again, click Yeson the prompt that appears asking if the application can make changes to your computer. The application will do a number of things to finish installing and setting up Docker.

Once you see a $ prompt type docker run hello-world. A brief introductory message should be printed to the screen.

Close the “Docker Quickstart” application and open a terminal (i.e., the Ubuntu application).

Copy-paste the following commands. You will be prompted to enter your password once.

    # Update the apt package list.
    sudo apt-get update -y
    # Install Docker's package dependencies.
    sudo apt-get install -y \
        apt-transport-https \
        ca-certificates \
        curl \
        software-properties-common

    # Download and add Docker's official public PGP key.
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

    # Verify the fingerprint.
    sudo apt-key fingerprint 0EBFCD88

    # Add the stable channel's Docker upstream repository.

    sudo add-apt-repository \
        "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
        $(lsb_release -cs) \
        stable"

    # Update the apt package list (for the new apt repo).
    sudo apt-get update -y

    # Install the latest version of Docker CE.
    sudo apt-get install -y docker-ce

    # Allow your user to access the Docker CLI without needing root access.
    sudo usermod -aG docker $USER


Close and re-open the terminal.

Type `pip install docker-compose`.

Type powershell.exe "docker-machine config". You should get output similar to the following:

    --tlsverify
    --tlscacert="C:\\Users\\<YOUR_USERNAME>\\.docker\\machine\\machines\\default\\ca.pem"
    --tlscert="C:\\Users\\<YOUR_USERNAME>\\.docker\\machine\\machines\\default\\cert.pem"
    --tlskey="C:\\Users\\<YOUR_USERNAME>\\.docker\\machine\\machines\\default\\key.pem"
    -H=tcp://xxx.xxx.xx.xxx:xxxx

where `<YOUR_USERNAME>` will have an actual value (likely your Windows username), and `tcp=xxx.xxx.xx.xxx:xxx` will be a series of numbers. If you don't get this output then something has gone wrong. Please make sure you were able to run the docker run hello-world command, above. If you were and you still don't receive this output, please contact one of the instructors on the #help-installation channel on the BHS Slack.

You will use the the outputs of the above command to modify the commands below before running them in the terminal. First, take the numbers printed in place of the xs on the output of the line `-H=tcp://xxx.xxx.xx.xxx:xxxx` from above and replace the placeholder `xxx.xxx.xx.xxx:xxxx` on the first command below (export `DOCKER_HOST`). Second, take whatever value is printed in place of `<YOUR_USERNAME>` above and replace the `<YOUR_USERNAME> `placeholder on the second command below (export `DOCKER_CERT_PATH`). Once you have updated the commands appropriately, copy and paste them into the terminal:

    echo "export DOCKER_HOST=tcp://xxx.xxx.xx.xxx:xxxx" >> $HOME/.bashrc
    echo "export DOCKER_CERT_PATH=/mnt/c/Users/<YOUR_USERNAME>/.docker/machine/certs" >> $HOME/.bashrc
    echo "export DOCKER_TLS_VERIFY=1" >> $HOME/.bashrc

Close and re-open a terminal (i.e., the Ubuntu application). Type docker run hello-world. The same brief introductory message you saw before should be printed to the screen.

*Note: *If you restart your computer (or somehow otherwise shut down the Docker VM) you will need to re-open the “Docker Quickstart” application and wait until you see the $ prompt again before your docker commands will work again! If you are having problems running docker commands in the terminal, try re-opening the “Docker Quickstart” application.

(The above step-by-step instructions are distilled from here and here. If you have questions during the installation procedure please check those links for potential answers!)
```
```{tabbed} Mac OS
1. Go to https://hub.docker.com/editions/community/docker-ce-desktop-mac/ and press “Get Docker”.
2. Open the “Docker.dmg” file that is downloaded and drag and drop the icon to the Applications folder
3. Open the Docker application and enter your password. An icon will appear in the status bar in the top-left of the screen. Wait until it reads “Docker Desktop is now up and running!”
4. Open a new terminal and type docker run hello-world. A brief introductory message should be printed to the screen.

(The above step-by-step Docker instructions are distilled from here. If you have questions during the installation procedure please check that link for potential answers!)
```

```{tabbed} Linux
You will be following different instructions depending on your distro (Ubuntu, Debian, Fedora, CentOS). Make sure to follow the “Install using the repository” method!
Once you’ve installed Docker make sure to follow the post-install instructions as well. You only need to do the “Manage Docker as a non-root user” and “Configure Docker to start on boot” steps.
Open a new terminal and type docker run hello-world. A brief introductory message should be printed to the screen.
```

## GitHub account

Go to https://github.com/join/ and follow the on-screen instructions to create an account. It is a good idea to associate this with your university e-mail (if you have one) as this will entitle you to sign up for the GitHub Student Developer Pack which comes with some nice free bonuses.

## Modern web browser

Install Firefox or Chrome. (Safari will also work.) Microsoft Edge is not modern, despite what Microsoft might try and otherwise tell you.

## Checking your install

Now that you've installed everything it's time to check that everything works as expected! Type the following into your terminal:

```bash
bash <( curl -s https://raw.githubusercontent.com/BrainhackMTL/psy6983_2021/master/content/en/modules/installation/nds_check_install.sh )
```

If you installed everything correctly you should see a message informing you as such. If any problems were detected you should receive some brief instructions on what is wrong with potential suggestions on how to remedy it. If you followed these instructions step-by-step and cannot resolve the issue please contact one of the course instructors for more help.