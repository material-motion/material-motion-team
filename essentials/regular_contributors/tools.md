# Tools

As a regular contributor you may work with a variety of tools.

Here's a list of tools we currently use as a team:

- [GitBook](https://www.gitbook.com/) for document authoring (like this one!)
- GitHub for code authoring ([material-motion](https://github.com/material-motion) is our org)
- git for all version tracking
- [Phabricator Differential](https://www.phacility.com/phabricator/differential/) for code-review
- The [GitBook mac editor](https://www.gitbook.com/editor/osx) allows you to edit books offline
- [draw.io](https://www.draw.io) for SVG and flow-chart editing

## Installing our tools

We have a team command line tool that installs the different commands.

    git clone git@github.com:material-motion/material-motion-team.git
    cd material-motion-team
    echo "export PATH=$(dirname $(find $(pwd) -regex '.*bin/mdm')):\$PATH"
    
This output should be added to your `~/.bashrc` or `~/.bash_profile`.
    
    # edit ~/.bash_profile
    source ~/.bash_profile
    mdm tools install

### GitHub

- [Add SSH keys to your GitHub account](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)
- [Hello world](https://guides.github.com/activities/hello-world/) GitHub guide.

### Android

Versions of software we use:

- Android Studio 2.2 Preview 4

### appleOS

Versions of software we use:

- Objective-C: 
  - Xcode 7.3.1.
- Swift 3.0: 
  - Xcode 8 beta
- Cocoapods 1.0.1
- psych 2.1.0

  We use version 2.1.0 of the `psych` gem. This version of `psych` adds quotes to the Podfile.lock after a `pod install`. Older versions removed the quotes.

  View your version:

      gem list | grep psych

  Update your version:

      sudo gem update psych