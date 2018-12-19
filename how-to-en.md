

############################################## 

01 ------------------------------------------- 

  donwload the IntelliJ-IDEA-$VERSION.tar.gz file on official site

02--------------------------------------------

  open a terminal (or press ctrl+Alt+T) and go to /opt/:

    $ cd /opt/

03-------------------------------------------- 

  extract the file:

    $ sudo tar -xvzf ~/Downloads/idea-$VERSION_BUILD.tar.gz

    // replace "idea-$VERSION_BUILD.tar.gz" with your correct file name

04-------------------------------------------- 

// this step you decide how to create the need file: manual, or using terminal

04.1------------------ manual -------------

  open your home and create a new text file named "intellij-idea.desktop"

04.1.1--------------------------------------- 

then paste the text and save it

    [Desktop Entry]
    Name=IntelliJ IDEA
    Type=Application
    Exec=/opt/idea-Ic-183.4886.37/bin/idea.sh
    Terminal=false
    Icon=/opt/idea-Ic.183.4886.37/bin/idea.png
    Comment=Integrated Development Environment
    NoDisplay=false
    Categories=Development;IDE;
    Name[en]=IntelliJ IDEA
    Name[en_US]=IntelliJ IDEA
    Name[pt-BR]=IntelliJ IDEA

(replace "idea-Ic.183.4886.37" with your correct folder name) 

// run these codes to check it 
    {$ cd /opt/}
    {$ ls }

04.1.2-------------------------------------------------

04.2- via terminal (ignore if you followed manual steps) -----

open a new terminal (or press ctrl+Alt+T), and type the text:

    $ nano intellij-idea.desktop

then type the text below, replacing "idea-ic-183.4886.37"
with your correct folder name (//check step 04.1.1//)


  [Desktop Entry]
  Name=IntelliJ IDEA
  Type=Application
  Exec=/opt/idea-Ic-183.4886.37/bin/idea.sh
  Terminal=false
  Icon=/opt/idea-Ic.183.4886.37/bin/idea.png
  Comment=Integrated Development Environment
  NoDisplay=false
  Categories=Development;IDE;
  Name[en]=IntelliJ IDEA
  Name[en_US]=IntelliJ IDEA
  Name[pt-BR]=IntelliJ IDEA

04.2.2-------------------------------------------------- 

press ctrl+x to exit;

press s and then confirm to save.

05.------------------------------------------------------

type the text below to install

      ~$ sudo desktop-file-install intellij-idea.desktop
      
############################################################

that it's all.

so, these step could be applied to Android Studio too.

next time you initialize IntelliJ IDEA, or Android Studio, just click on IDE icon ;)
