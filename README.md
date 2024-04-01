Assignment 2 : git branches


git init
touch feature1.txt feature2.txt
git checkout -b develop
git checkout -b feature1
git checkout -b feature2

git checkout develop
touch develop.txt
git stash develop.txt -m "Stashed file"

git checkout feature1

touch new.txt
git add new.txt
git commit -m "new.txt file"
git push origin feature1

git checkout develop
git stash pop
git commit -m "Added develop.txt file"
git push origin develop



