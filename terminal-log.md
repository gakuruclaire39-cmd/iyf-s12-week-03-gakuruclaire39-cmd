# Terminal Log — Week 03 - Claire Wairimu

## Task 5.1: Navigation
pwd
mkdir -p my-project/src/css my-project/src/js
touch my-project/README.md
find my-project

## Task 5.2: File Operations
touch index.html
cp index.html backup.html
mv backup.html my-project/docs/
rm home.html
cp -r src src-backup
mv src-backup archive/
rm -r archive

## Task 5.3: Finding Files
find . -name "*.html" | wc -l
grep -rli "contact" --include="*.html" .
wc -l css/styles.css
history | tail -10

## Task 5.4: Script
chmod +x new-project.sh
bash ./new-project.sh my-awesome-app
find my-awesome-app
