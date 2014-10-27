Sublime Text 3 User Settings
============

Sublime Text 3 Packages/User folder

## Dependancies

- Node.js
- Ruby
- Python
- Git
- GitHub for Windows

## Instructions for Windows

- Install Node.js - http://nodejs.org/
- Install Ruby (1.9.3 for Grunt compatibility) - http://rubyinstaller.org/
- Install Python - https://www.python.org/downloads/
- - Install Git - http://git-scm.com/download/win
- Install GitHub for Windows - https://windows.github.com/
- Install Menlo Regular Font - https://github.com/hbin/top-programming-fonts
- Sugest system restart to ensure packages are registered and PATH variable set.
- Install Sublime Text 3 - http://www.sublimetext.com/3
- - Add Package Control to Sublime Text - https://sublime.wbond.net/installation
- Shutdown Sublime Text

## Individual plugin dependancies

- HTML Tidy - http://tidybatchfiles.info/
  Download and extract the zipfile to anywhere you like and ensure the PATH is set in environment variables.
- CSS Lint - You must install CSS Lint on your system first - `npm install -g csslint`
- SCSS Lint - `gem install scss-lint`
- JS Lint - `npm install -g jslint`
- CSS3 - Disable default CSS package - possible conflicts with Emmet
- Emmet plugin requires PyV8 which may fail to download to the Packages folder using this method. Using Package Control, remove and re-add Emmet manually.

### Once all the above is set up:

- Clone this repo to:
 
` C:\Users\UserName\AppData\Roaming\Sublime Text 3\Packages`

- This will overwrite the existing User folder.

- Start Sublime Text - Package control should begin to downloading and installing the 'missing' packages. BE PATIENT - on an old laptop this took 15 mins plus during which time Sublime and laptop were unresponsive.
