# Lesson 5.1 Terminal Log - Claire Wairimu
Date: Codespaces Terminal (Linux bash)

## Setup
- mkdir -p ~/terminal-practice - Created safe scratch folder outside repo
- cd ~/terminal-practice - Moved into practice folder

## Exercise 1
- pwd - Printed current working directory
- ls -la - Listed all files including hidden
- cd /tmp - Navigated to /tmp
- cd .. - Went back one level
- cd ~ - Went to home directory

## Exercise 2
- mkdir -p my-project/src/css my-project/src/js my-project/src/images
- mkdir -p my-project/docs my-project/tests
- touch my-project/README.md
- ls -R my-project - Verified structure
- find my-project | sort - Showed tree

## Final Structure:
my-project/
├── src/css/
├── src/js/
├── src/images/
├── docs/
├── tests/
└── README.md

---

## Lesson 5.2: File Operations - Claire Wairimu (Continued)

### Exercise 1: Create and Edit Files

# Create a new file
touch index.html

# Add content
echo "<h1>Hello Portfolio</h1>" > index.html

# View file contents
cat index.html

# Copy a file
cp index.html backup.html

# Move a file
mkdir -p docs
mv backup.html docs/

# Rename a file
mv index.html home.html

# Delete a file
rm home.html

### Exercise 2: Working with Directories

# Create source structure
mkdir -p src/css src/js
touch src/css/style.css src/js/app.js

# Copy a directory
cp -r src/ src-backup/

# Move a directory
mv src-backup/ archive/

# Delete an empty directory
mkdir empty-test
rmdir empty-test

# Delete a directory with contents
rm -r archive/

### Challenge: Reorganize Portfolio Project

# Create new structure
mkdir -p assets/images assets/css docs
mv -n images/* assets/images/ 2>/dev/null || cp -r images/* assets/images/
mv -n styles.css assets/css/ 2>/dev/null || true
ls -R

---

## Lesson 5.3: Useful Terminal Commands - Claire Wairimu (Continued)

### Search and Find:

# Find files by name
find . -name "*.html"

# Search inside files
grep "class" index.html
grep -r "button" ./src/

# Show command history
history

### View and Edit:

# View first/last lines
head -10 assets/css/styles.css
tail -10 assets/css/styles.css

# Count lines, words, characters
wc index.html
wc -l index.html

### Task Answers (using terminal commands only):

# Q1: How many HTML files?
find . -name "*.html" | wc -l

# Q2: Which files contain "contact"?
grep -r -l "contact" . --include="*.html"

# Q3: How many lines is CSS?
wc -l assets/css/styles.css

# Q4: Last 10 commands?
history | tail -10

## Lesson 6.1: Git Basics
git config --list, git init, git status, git add, git commit, git log
3 commits: Style, Fix, Docs - completed

## Lesson 6.1: Git Basics
git config --list, git init, git status, git add, git commit, git log
3 commits: Style, Fix, Docs - completed
