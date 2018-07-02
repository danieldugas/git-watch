# git-watch
A super simple python-based command-line tool to keep track of your git repositories.

[![Demo git-watch](https://raw.githubusercontent.com/danieldugas/git-watch/master/demo.gif)]()

## Install

```
sudo apt install python-git
cd ~
git clone https://github.com/danieldugas/git-watch.git
echo "export PATH=\"\$HOME/git-watch:\$PATH\"" >> ~/.bashrc
source ~/.bashrc
```
That's it.

### Try it
```
git-watch --no-fetch
```

#### git_repos_to_watch.txt
Add the paths to your favorite repositories in the file git_repos_to_watch.txt, and git-watch will keep track of them too.  
git-watch looks for git_repos_to_watch.txt in your home folder, and will create it if it doesn't exist.

#### --no-fetch
Without this option, git-watch udpates the upstream information for your repositories, which can take a few seconds. You might be in a hurry, and a few seconds are worth sparing, sometimes.

#### --add-this-repo
You're in your new favorite git repository, and want to quickly add it to the git_repos_to_watch.txt file? No hassle, let git-watch do it for you: ```git-watch --add-this-repo```.

## Uninstall

It's okay, git-watch understands and loves you anyways. To remove it from your computer, delete ~/git_repos_to_watch.txt, remove the ```export PATH="$HOME/git-watch:$PATH"``` line in ~/.bashrc, and delete the ~/git-watch folder. 

## License

Do-whatever-the-heck-you-want, but be nice about it.
