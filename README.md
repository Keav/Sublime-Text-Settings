Initialise a Web Development Environment
============
This is a repo of the Sublime Text 3 `Packages\User` folder; containing all installed Sublime Text packages and settings, including custom Sublime Text User Preferences.

**Windows**
```
C:\Users\UserName\AppData\Roaming\Sublime Text 3\Packages\User
```
**OS X**
```
~/Library/Application Support/Sublime Text 3/Packages/User
```

######The following instructions are not all required simply to get Sublime Text up and running but also include a number of other tools that I use within most of my web projects.

## Typical Global Project Dependencies

- Node.js
- Ruby
- Python
- Git
- GitHub for Windows
- Grunt
- WAMP

## Install These

- Install Node.js - http://nodejs.org/
- Install Ruby (1.9.3 for Grunt compatibility) - http://rubyinstaller.org/
- Install Python - https://www.python.org/downloads/
- Install Git - http://git-scm.com/download/win
- Install GitHub GUI for Windows or OS X
  - https://windows.github.com/
  - https://mac.github.com/
- Install Menlo Regular Font - https://github.com/hbin/top-programming-fonts
- Sugest system restart to ensure packages are registered and PATH variable set.
- Install Sublime Text 3 - http://www.sublimetext.com/3
- Add Package Control to Sublime Text - https://sublime.wbond.net/installation
- Shutdown Sublime Text
- Grunt CLI - `npm install -g grunt-cli`
- Local installs of Grunt itself are handled by having a packages.json file in your project and running `npm install`
* WAMP - http://www.wampserver.com/
* MAMP - https://www.mamp.info/

Also see my localhost configuration instructions here: https://github.com/Keav/localhost-config

## Individual Sublime Text plugin dependancies

- HTML Tidy - http://tidybatchfiles.info/
  Download and extract the zipfile to anywhere you like and ensure the PATH is set in environment variables.
  Update: This is now part of my 'scripts' repo.
- CSS Lint - `npm install -g csslint`
- SCSS Lint - `gem install scss-lint`
- JS Lint - `npm install -g jslint`
- PHP Lint - `npm install -g phplint`

### Clone this repo
 
 Do not use GitHub for Windows (or GitHub for Mac) or the 'Clone to Desktop' option available at GitHub.com. This will always create a folder of the same name as your repo, which is not what we want. Instead, we want all the repo files to go into the `packages/User` folder, regardless of Repo name.
 
Ensure you have run Sublime Text at least once, otherwise the necessary folders won't exist.

In your git shell, navigate to:

**Windows**
```
C:\Users\UserName\AppData\Roaming\Sublime Text 3\Packages\User
```
**Pro Tip**: If you have Git Bash installed in Windows you can use the same command as you would in Linux or OS X:
```
cd ~/appdata/roaming/sublime\ text\ 3/packages/user
```
The `\`'s are required to escape the spaces.

**Mac OS X**
```
~/Library/Application Support/Sublime Text 3/Packages/User
```

Ensure the folder is empty and enter the following:

**Make sure you include the final `.` in the following command**
```
git clone https://github.com/User/YourRepo.git .
```

The `.` means the repo's contents will be cloned into the current location.

If you want this repo in GitHub for Windows, now add this local repo in the usual way, within GitHub for Windows.

Start Sublime Text - Package control should begin to downloading and installing the 'missing' packages.

## Post Install Checks

- CSS3 - Disable default CSS package - possible conflicts with Emmet
- Emmet plugin requires PyV8 which may fail to download to the Packages folder using this method. Using Package Control, remove and re-add Emmet manually.
- WAMP requires MSVC110.dll which may not be present on a fresh Windows build. Download from http://www.microsoft.com/en-us/download/details.aspx?id=30679

##Useful Files and Paths

* Session.sublime_session
```
~/Library/Application Support/Sublime Text 3/Local/Session.sublime_session
```
Usually you don't want to edit this file but scroll to the bottom and you will find your project quick switch list. Occasionally you may need to remove a project from this list or change its location.

* User Preferences
```
/Users/chriskeavey/Library/Application Support/Sublime Text 3/Packages/User/Preferences.sublime-settings
```

## Next

Go ahead and take a look at my instructions for configuring a developer friendly localhost server environment:
- https://github.com/Keav/localhost-config
