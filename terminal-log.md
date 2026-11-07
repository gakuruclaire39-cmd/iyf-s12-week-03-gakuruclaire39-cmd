Terminal Log — Week 03 - Claire Wairimu

# Terminal Log — Week 03 - Claire Wairimu

## Task 5.1: Navigation and Directories

| Terminal Command | Explanation |
|---|---|
| `pwd` | Displays the current working directory. |
| `ls -la` | Lists all files and folders, including hidden files. |
| `mkdir -p portfolio/src/css` | Creates a portfolio directory with a CSS subfolder. |
| `cd portfolio` | Moves into the portfolio directory. |
| `cd ..` | Returns to the parent directory. |
| `tree` | Displays files and folders in a tree structure. |

## Task 5.2: File Operations and Editing

| Terminal Command | Explanation |
|---|---|
| `touch index.html` | Creates a new HTML file. |
| `touch about.html contact.html` | Creates two HTML files. |
| `echo "<h1>My Portfolio</h1>" > index.html` | Writes content into a file, replacing existing content. |
| `echo "<p>Welcome to my website.</p>" >> index.html` | Adds content without deleting existing content. |
| `nano index.html` | Opens an existing file for editing. |
| `sed -i 's/My Portfolio/Claire Wairimu Portfolio/g' index.html` | Replaces specific text in the original file. |
| `cp index.html backup.html` | Creates a copy of the HTML file. |
| `mv backup.html old-index.html` | Renames the backup file. |
| `rm old-index.html` | Deletes the backup file. |

## Task 5.3: Finding and Searching Files

| Terminal Command | Explanation |
|---|---|
| `find . -type f` | Finds all files in the current directory and subdirectories. |
| `find . -name "*.html"` | Searches for all HTML files. |
| `find . -name "*.css"` | Searches for all CSS files. |
| `grep -n "Portfolio" index.html` | Searches for Portfolio and displays its line number. |
| `grep -ri "contact" .` | Searches for contact in files and folders. |
| `wc -l index.html` | Counts the lines in the HTML file. |
| `du -sh .` | Displays the total size of the current directory. |
| `history | tail -10` | Displays the last ten terminal commands. |

## Task 5.4: Creating and Running a Shell Script

| Terminal Command | Explanation |
|---|---|
| `touch setup.sh` | Creates a shell script file. |
| `nano setup.sh` | Opens the script for editing. |
| `chmod +x setup.sh` | Gives the script permission to execute. |
| `./setup.sh` | Runs the shell script. |
| `bash setup.sh` | Executes the script using Bash. |

### Shell Script Content

```bash
#!/bin/bash

echo "Creating my portfolio project..."

mkdir -p my-portfolio/css
mkdir -p my-portfolio/js
mkdir -p my-portfolio/images

touch my-portfolio/index.html
touch my-portfolio/README.md

echo "Portfolio created successfully!"
