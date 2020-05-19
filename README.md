# Development Environment setup

All you need to write Javascript, HTML, and CSS is TextEdit/Notepad and a Browser, the rest is just for fun:

## Text Editors

You'll need something nice to edit text, choose one of these, or something else!

### [Visual Studio Code](https://code.visualstudio.com/)

Made by microsoft, has all the things, autocompletes your Javascript, integrates with git and has a built-in terminal. If your computer is old, it might run slightly slow. If it asks you to install plugins while opening files, just say yes to everything so it can set itself up.

#### Opening files in VS Code from the command line

If you prefer using a separate terminal app, you can open files from there in VS Code with the  `code` command. If you are on a Mac, it needs to be set up before it will work:

1. Open the Command Palette (⌘⇧P) and type 'shell command' and click 'Shell Command: Install 'code' command in PATH'
2. Open a terminal. Open a file with `code ./some/file/path.html`

### [Sublime Text](https://www.sublimetext.com/)

Another good option. Runs real fast, minimal interface, has nice themes. It costs $70 for a license but you can use it for free if you don't mind an occasional nag popup

### Vim/Nano/...Emacs...

Editors that run in your terminal. These are useful for quickly editing files without opening a full editor session, and are often the easiest way to edit files on remote servers. They can be confusing, but you should be somewhat familiar with them. If you need to use one, I suggest `nano path/to/some/file` since it has nice onscreen instructions. 

#### What happened when I typed `git commit`? Why can't I close this commit message and save my work?

Git typically uses Vim as its default '$EDITOR' for editing commit messages, so running `git commit` without `  -m "Commit message"` actually opens the Vim text editor with a buffer to write your commit message. To finish the commit, you need to save the commit message, which is done in this arcane way:

1. Press the ESC key on your keyboard
2. type `:wq` -- what you type should appear on the bottom line of the window
3. Press Enter to return to commit and your terminal session
4. Ask Ders for help if you get stuck because he loves Vim

## Developer Tools

### Git

#### [Git for Windows](https://gitforwindows.org/)

Windows doesn't come with git by default, so install it from there. All the defaults are fine.

#### Git on Mac

Macs come with git preinstalled, but you can get a more up-to-date version if you'd like from [Homebrew](https://brew.sh/) -- install homebrew by pasting their install command in your terminal. Once it's installed, just run `brew install git`.

Homebrew is great for  downloading and managing all other command-line related software, and is highly recommended regardless of if you use it to install node.

### [NodeJs](https://nodejs.org/en/)

Node.js® is a JavaScript runtime built on Chrome's [V8 JavaScript engine](https://v8.dev/). Download and install the latest LTS version from above. LTS = Long-Term Support = won't change very often.

#### Other option for downloading Node on Mac:

Install [Homebrew](https://brew.sh/) and then run `brew install node@12` to get the latest LTS release.

### [Insomnia](https://insomnia.rest/download/)

Useful REST API client for testing http requests. Download 'Insomnia Core'
