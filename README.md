Initialise Windows Web Development Environment
============
This is a repo of the Sublime Text 3 `C:\Users\UserName\AppData\Roaming\Sublime Text 3\Packages\User` folder; containing all installed Sublime Text packages and settings.

####The following instructions are not all required simply to get Sublime Text up and running but also include a number of other tools that I use within most of my web projects.

## Global Project Dependencies

- Node.js
- Ruby
- Python
- Git
- GitHub for Windows
- Grunt
- WAMP

## Instructions for Windows

- Install Node.js - http://nodejs.org/
- Install Ruby (1.9.3 for Grunt compatibility) - http://rubyinstaller.org/
- Install Python - https://www.python.org/downloads/
- Install Git - http://git-scm.com/download/win
- Install GitHub GUI for Windows or OS X - https://windows.github.com/
- Install Menlo Regular Font - https://github.com/hbin/top-programming-fonts
- Sugest system restart to ensure packages are registered and PATH variable set.
- Install Sublime Text 3 - http://www.sublimetext.com/3
- Add Package Control to Sublime Text - https://sublime.wbond.net/installation
- Shutdown Sublime Text
- Grunt - `npm install grunt`
- Grunt CLI - `npm install -g grunt-cli`
- WAMP - http://www.wampserver.com/en/
- MAMP - https://www.mamp.info/en/
 
- Also see my localhost configuration instructions here: https://github.com/Keav/localhost-config

## Individual plugin dependancies

- HTML Tidy - http://tidybatchfiles.info/
  Download and extract the zipfile to anywhere you like and ensure the PATH is set in environment variables.
  Update: This is now part of my 'scripts' repo.
- CSS Lint - `npm install -g csslint`
- SCSS Lint - `gem install scss-lint`
- JS Lint - `npm install -g jslint`

### Clone this repo
 
 Do not use GitHub for Windows or the 'Clone to Desktop' option. This will always create a folder of the same name as your repo, which is not what we want. Instead, we want all the repo files to go into the `packages/User` folder, regardless of Repo name.
 
 - Ensure you have run Sublime Text at least once, otherwise the necessary folders won't exist.
 - In your git shell, navigate to:
```
C:\Users\UserName\AppData\Roaming\Sublime Text 3\Packages\User
```
- Pro Tip: If you have Git Bash installed in Windows you can use the same command as you would in Linux or OS X:
`\` is required to escape the spaces.
```
cd ~/appdata/roaming/sublime\ text\ 3/packages/user
```

- Ensure the folder is empty and enter the following:

`git clone https://github.com/User/YourRepo.git .`

- The '.' means the repo's contents will be cloned into the current location.

- If you want this repo in GitHub for Windows, now add this local repo in the usual way, within GitHub for Windows.

- Start Sublime Text - Package control should begin to downloading and installing the 'missing' packages. BE PATIENT - on an old laptop this took 15 mins plus during which time Sublime and laptop were unresponsive.

## Post Install Checks

- CSS3 - Disable default CSS package - possible conflicts with Emmet
- Emmet plugin requires PyV8 which may fail to download to the Packages folder using this method. Using Package Control, remove and re-add Emmet manually.
- WAMP requires MSVC110.dll which is unlikely to be present on a fresh Windows build. Download from http://www.microsoft.com/en-us/download/details.aspx?id=30679
