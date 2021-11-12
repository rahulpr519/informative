# informative

to fix "Head detached from prev commit(master)"

1. git branch temp
2. git checkout temp
3. git log --graph --decorate --pretty=oneline --abbrev-commit master origin/master temp
4. git diff master temp
5. git diff origin/master temp
6. git branch -f master temp
7. git checkout master
8. git branch -d temp
9. git push origin master


to "change author"

git commit --amend --author="Author Name <email@address.com>" --no-edit
