# 🧠 Git Basics: A Personal Cheatsheet by Prapti

## 🔧 Git Configuration

```bash
git --version
git config --global user.name "Prapti"
git config --global user.email "flyingprapti99@gmail.com"

##📁 Create a New Git Project		← H2
mkdir gitdemo
cd gitdemo
git init

##📂 Checking Status and Branch	**
git status
git branch

##📝 Adding Files and Making Commits	← H2
vi one.txt              # or any text editor
git add one.txt         # stage file
git add .               # stage all files
git commit -m "this is my first commit"

##🔁 Second Commit (after editing a file)	← H2
vi one.txt
git status
git add one.txt
git commit -m "this is my 2nd commit"

##🔍 View Git History			← H2
git log
git log --stat

##🌱 Create and Switch Branches		 ← H2
git branch branch1
git checkout branch1
git branch

##📤 Push Code to GitHub           	 ← H2
mkdir githubdemo
cd githubdemo
git init

vi one1.txt
vi two2.txt
git add .
git commit -m "1st commit"

git remote add origin https://github.com/penguin1599/githubdemo.git
git branch -M main        # rename master → main
git push -u origin main   # first push



##📥 Pull Updates from Remote		← H2
git pull          # fetch + merge the current branch from origin
# OR, if you renamed the remote or want explicit control:
git pull origin main

# Quick check for what’s new before merging:
git fetch origin           # download changes, don’t merge
git log HEAD..origin/main  # view commits you’re about to merge
git merge origin/main      # merge manually (optional)


##✅ After Push / Pull: Check Status	← H2
git status

