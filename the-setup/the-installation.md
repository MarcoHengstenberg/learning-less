# The Installation

1. First you will have to install Ruby on your machine! No, you don't – Ruby is preinstalled on all Mac Computers. Marvelous. You skipped the first step.
2. Open the Terminal app (cmd + Space, Type *"Terminal"*, hit Enter)
3. Watch the Commmand Prompt and stroke your geek-beard (you will grow one, woman or not, don't mind it)
4. Copy and paste the following command into Terminal `ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"` and hit enter. Wait while Homebrew is installing.
5. Download XCode from the App Store, install its "Command Line Tools" from inside XCode afterwards. Fancy a [guide](http://osxdaily.com/2014/02/12/install-command-line-tools-mac-os-x/)? If you want the Command Line Tools without XCode, [try that one here](http://osxdaily.com/2012/07/06/install-gcc-without-xcode-in-mac-os-x/).
6. Now you can install node.js globally. Again, copypasta the command and hit enter: `brew install node.js` Again some waiting is needed.
7. Install Grunt.js globally. This way you won't have to install Grunt each and every time you create a new project: `npm install -g grunt-cli`. **Optional:** When executing that command, open your mouth, take a deep breath and then exhale through your nose and mouth at the same time while pretending to gargle some water after having brushed your teeth. This is called *"Grunting"*.

Now, that you have installed homebrew, node.js and grunt you are almost there. You are bytes away from happily starting your automated web development workflow.