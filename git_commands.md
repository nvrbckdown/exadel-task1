git clone git@github.com:nvrbckdown/exadel-task1.git

cd exadel-task1
mkdir Task1
echo "HELLO WORLD TO EXADEL" > Task1/README.md

git add . && git commit -m "initial commit" && git push origin master

git branch -c dev
git checkout dev
echo "HELLO FROM Dev branch" > test.txt

git branch -c abdulkodir-new_feature
git checkout abdulkodir-new_feature
echo "HELLO FROM abdulkodir-new_feature branch" > README.md

git status
touch .gitignore
echo ".gitignore" > .gitignore
git add . && git commit -m "initial commit for abdulkodir-new_feature branch" && git push origin abdulkodir-new_feature

echo "Change commit from abdulkodir-new_feature branch" > README.md
git add . && git commit -m "README.md file edited"

git revert HEAD
git log > log.txt

git branch -D abdulkodir-new_feature
git push origin --delete abdulkodir-new_feature

vim git_commands.md
git add . && git commit -m "add git_commands.md file" && git push origin dev
