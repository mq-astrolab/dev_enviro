# dev_enviro
Development Environment Notes

I. Standardization

So that we're all on the same page. Let us standardize our development environment for the Macquarie teaching spectrograph data reduction project.

First off we will be starting with the Veloce pipeline, and Christoph Bergmann from UNSW has come over to do a mini workshop with the vacation scholarship students to get us started. We will be forking his repository from here:

https://github.com/cmbergmann/mq_spectrograph

The imported repository is here:

https://github.com/mq-astrolab/mq_spectrograph

II. Directory Tree

I suggest we use the following directory tree.

mq-astrolab -- codestore -- mq_spectrogprah
            |--datastore
            
            
for example:  c:\users\blaise\documents\mq-astrolab\codestore\mq_spectrograph
              c:\users\blaise\documents\mq-astrolab\datastore
              
              
III. Cloud storage

I created this directory for cloud store for sharing fits and other large files:

https://cloudstor.aarnet.edu.au/plus/s/0y8pRpeXIVgb05J

I'll post the password to access the link in slack.

For convenience I can add your cloudstor usernamed to the share directory and the desktop sync clients can used to mount the share directory on your laptops.

The desktop clients are here:
https://cloudstor.aarnet.edu.au/client-download/

IV. Python and Integrated Development Environment

For python download Anaconda from here, which is available for Windows, Linux and OS X

https://www.anaconda.com/download/

Download version for Python 3.

When going through the installer, choose to also install Visual Studio Code.

a. As far a IDE, Christoph uses PyCharm, which is also cross platform.

I propose using Visual Studio Code since it already install along with Anaconda.

Both are free. PyCharm's bigger brother IntelliJ IDEA is also free for students.

b. As an addition step if you plan to use git via ssh, create a public key in your home directory. It will be in somewhere like c:\users\blaise\.ssh

Copy and paste that key to github.com under keys. Now you should be able to use git to automatically fetch and push changes to the repository.

V. Importing the repository into Visual Studio Code.

Now that everything is setup. Start up Visual Studio Code. Go to "File" and "New Window" to start fresh.

Use the shortcut, Ctrl+Shift+P, then type "Git: Clone" and enter

It will prompt you to enter a URL and type or paste in:

git@github.com:mq-astrolab/mq_spectrograph.git

https://github.com/mq-astrolab/mq_spectrograph.git

depending on whether you use http or ssh

Select the folder "codestore" the mq_spectrograph repo and directory will be created there.

A popup asking to open the repository will appear. Click "open repository"

Open a script and start working!

Your IDE should look like this:

![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/img.png)
