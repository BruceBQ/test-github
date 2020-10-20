echo "# test-github" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/BruceBQ/test-github.git
git push -u origin main
git checkout -b main_1
git add .
git commit -m "add file 1.js"
git push origin main_1
git merge main
git checkout main
git add .
git commit -m "add main.js"
git push
git merge main_1
git add .
git commit -m "add comment abc"
git checkout main_1
git push
git add .
git commit -m "add xyz"
git push origin main_1
git add main_2.js
git commit -m "merge"