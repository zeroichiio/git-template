# git-template
base git template

### pretext

This document expects that you have a working git and github environment. Setting up github settings or ssh-agent, gpg-agent on linux or windows, using git-bash or related components is outside of the scope of this document.

### git clone
```
cd <working space>
git clone https://github.com/zeroichiio/git-template.git
```
result: <working space> **git-timeplace**

- rename the folder *git-template to <project name>

### .git/config additions

For signing github commits and so on (public/private) repositories edit the following file:

**.git/config**

```
[remote "origin"]
	url = https://github.com/zeroichiio/<new name of git repo>.git
[user]
        email = <your github assigned email>
        name = <your github username>
        signingkey = A69E641C4115DFB5 <== your signing key in this form
[commit]
        gpgsign = true <== default to signing commits
```
