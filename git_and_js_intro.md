## GIT

### What is Git?

Git is a Version control System that runs locally on your PC. Bacically it keeps track of changes to your files in versions after each commit so you can rollback, etc. It has other powerful features like branches, ability to view diffs, merging, rebasing etc. It saves you the effort of having to keep track of your code changes manually by duplicating folders/entire projects and versioning them yourself.

- Check if git is installed on your PC. Run `git -v`. If there are no errors. It's installed else visit [git website](https://git-scm.com/downloads) and follow the instructons to download it for your operating system.

## Basic GIT commands

- `git init`: This initializes git in a folder.

- `git add <directory to monitor within folder>`: This tells git what directory to monitor within the folder.

- `git commit -m <commit message>`: This tells git to create a new version for the changes you just made.

- `git remote add <remote name> <remote url>`: This tells git to add a remote which you can push changes to subsequently alongside the versions (Basically copies your folder alongside the versions that git has on tyour local machine and keeps them online so you can use later haowever you like).

- `git log`: See all your versions.
