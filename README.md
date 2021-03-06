##Git setup - Windows


####Basic setup

1. <a href="http://git-scm.com/downloads" target="git_dl">Download</a> and install Git for your platform

  ![default settings](images/git-scm1.png "Use default settings")
  - Use default settings

  ![use from cmd](images/git-scm2.png "Use git from Command Prompt")
  - *Run Git from Command Prompt* is preferred

  ![use plink](images/git-scm3.png "Choose PLink as SSH helper")
  - PuTTY's plink integrates better with Windows

  ![newline format](images/git-scm4.png "Set format for line endings")
  - The default setting is fine



2. <a href="http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html" target="git_dl">Download</a> and install PuTTY, if necessary


3. Run PuTTYgen to create or import your SSH key

  ![click Generate](images/puttygen1.png "click Generate")
  
  - click **Generate**
  - click **Save private key**, and store your key somewhere safe.
  
  ![copy public key to clipboard](images/puttygen3.png "select the public key in the text area, and copy to the clipboard")
  - select the public key in the text area, and copy to the clipboard


4. [Add the SSH key to your GitHub account]
  

*Optional* <a href="https://code.google.com/p/tortoisegit/wiki/Download" target="git_dl">Download</a> and install TortoiseGIT (Optional)
  - This is the easiest way to configure SSH


*Alternatively:* <a href="http://sourcetreeapp.com" target="git_dl">Atlassian Sourcetree</a>



####Git-flow setup (Windows)

1. download [libiconv2.dll, libintl3.dll and getopt.exe](https://github.com/fillefrans/git-setup-windows/raw/master/bin/linux-ng.zip) from the util-linux-ng package, and place them all in the Git bin folder (typically "C:\Program Files (x86)\Git\bin")

2. Open a Command Prompt as Administrator (right-click \> *Run as Administrator*), and clone the git-flow repo.
  - You can clone it into any directory, but keep in mind that this is the permanent home of the script files you need to use git-flow. It is not a temporary directory.

  ```
  git clone --recursive https://github.com/nvie/gitflow.git
  ```

3. Install git-flow extension

  ```
  cd gitflow
  contrib\msysgit-install.cmd "C:\Program Files (x86)\Git"

  ```
  *Change "C:\Program Files (x86)\Git" to the folder where you installed Git*



####Start a git-flow repo:
  
  Open a Command Prompt, and navigate to the root of your repo

  Initialize as git-flow repository:

  ```
  cd easyad
  git flow init
  ```
  Hit \<Enter\> at each prompt to accept defaults


  Done!




####Links

* [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)
* [Why aren't you using git-flow?](http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/)
* [Getting started with git-flow](http://yakiloo.com/getting-started-git-flow/)
