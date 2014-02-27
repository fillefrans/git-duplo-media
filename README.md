##Git setup - Duplo Media


####Basic setup

1. [http://git-scm.com/downloads](Download) and install Git for your platform

  ![default settings](images/git-scm1.png "Use default settings")

  ![use from cmd](images/git-scm2.png "Use git from Command Prompt")

  ![use plink](images/git-scm3.png "Choose PLink as SSH helper")

  ![newline format](images/git-scm3.png "Set format for line endings")



2. [http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html](Download) and install PuTTY, if necessary


3. Run PuTTYgen, and create or import your SSH key

  ![click Generate](images/puttygen1.png "click Generate")
  
  - click **Generate**
  - click **Save private key**, and store your key somewhere safe.
  - select the public key in the text area, and copy to the clipboard
  
  ![copy public key to clipboard](images/puttygen3.png "select the public key in the text area, and copy to the clipboard")


4. Add the SSH key to your Springloops account
  
  - log into [Springloops](https://duplo.springloops.io) and open your profile page
  - click "edit" (top right of the page)
  - click "Profile details" in the top left menu
  - scroll down to SSH Public Key, and click "Manage"
  - click "Add a new SSH key"
  - paste in your key, and click "Create this new key"

*Optional* [Download](https://code.google.com/p/tortoisegit/wiki/Download) and install TortoiseGIT (Optional)
  - This is the easiest way to configure SSH

Mac OS X : [Atlassian Sourcetree]() and [Tower Git](http://www.git-tower.com/) both have built-in support for Git-flow


####Links

* [Getting started with git-flow](http://yakiloo.com/getting-started-git-flow/)




####Git-flow setup (Windows)

1. Open a command prompt, and clone the git-flow repo.
  - You can clone it into any directory, but keep in mind that this is the permanent home of the script files you need to use git-flow. It is not a temporary directory.

  ```
  git clone --recursive https://github.com/nvie/gitflow.git
  ```

2. download [libiconv2.dll, libintl3.dll and getopt.exe]() from the linux-ng package, and place them all in the Git bin folder (typically "C:\Program Files (x86)\Git\bin")






####Clone the easyad2 repo from Springloops:
  - This is the main repo for EasyAd

  ```
  git clone ssh://sls@slsapp.com:1234/duplo/easyad2.git
  ```


