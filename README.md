This is the Github repository for Object Recognition Project at Denis Pelli's Lab.

This is a public webpage, so only public information such as tutorials will be put here. This simply servers as a webpage to read stuff; you do not have to be familiar with Github (well, at least, for the time being)

### Installing MATLAB:

  1. Here is how you install MATLAB as a NYU student and activate with NYU license:
   - https://github.com/hyiltiz/ObjectRecognition/blob/master/InstallingMatlab.md
  1. After finishing installation, several tweaks/configurations are necessary:
   - *OS X specific*: The first time you open MATLAB, OS X gives a fatal error saying the developer is not registered.  Instead you should cntrl click the MATLAB app and select open. Then the same error message comes up but with an option to open anyway. If you succeed once then the finder remembers that it's ok. 


   - MATLAB is normally installed in the application folder which is good except that by default it's write only which prevents the user from saving the [path](http://www.mathworks.com/help/matlab/matlab_env/what-is-the-matlab-search-path.html), eg to include Psychtoolbox. This is flagged by a warning when you run `downloadpsychtoolbox`. An easy and straighforward solution is to set the correct permission for the pathdef file. To do so:
     - OS X: Using finder, `Cntrl click` open-package the MATLAB app to get inside the package. Then get info to allow everyone to read and write the pathdef file. You can also follow the method below for GNU/Linux systems if you are comfortable with using Terminal in OS X.
     - GNU/Linux: fire up your terminal, and become root then change file permission:
      ```bash
        su root # become root 
        # sudo -sH  # this also works on some systems
        # insert your password; note: it is invisible

        # use ls command to find out where MATLAB is installed
        # For example, try the following to see the contents of /usr/local folder
        ls /usr/local/

        # Then change the permission
        chmod 666 /usr/local/Mathworkѕ/MATLAB/R2015a/bin/pathdef.m

        # staying as root is dangerous and highly not recommended
        exit
      ```


### Installing Psychtoolbox:

There are several issues that arise in installing psychtoolbox. The first is whether the OS X svn tool is installed to do the installation. it's included in apple's developer software so you can get it that way through the App Store for free. Xcode?

  And you can follow the link below to install Psychtoolbox, which we are mainly using for running our experiments:
   - http://psychtoolbox.org/download/
   - *NOTE*: please follow the instructions in the website above as well as the output of the installer carefully; it is not all automatic. It requires to do certain things before it is all set up. For example, you may need to install additional software such as `svn` which if shipped with Apple's XCode development tools and `Gstreamer` depending on your Operating System; you may also need to restart MATLAB; you may need to create and add new user/group `psychtoolbox` in your system. The documentation is excellent in providing all those details, so you can simply follow their instructions.
   - try running `GratingDemo` to confirm that Psychtoolbox is installed.
   - try running `BasicSoundOutputDemo` to confirm that sound works. If you see problems, see `help PsychPortAudio`.
   - try running `Speak('I love science!');` to confirm that speech synthesis features can work.

Please [submit a new issue](https://github.com/hyiltiz/ObjectRecognition/issues) if you experience any difficulties.
