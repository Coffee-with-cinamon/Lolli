# Lolli
git init
git checkout -b main
echo "Initial content" > file.txt
git add file.txt
git commit -m "Add initial file"
rename file.txt file.md
git add file.md
git commit -m "Change file type to markdown"
git checkout -b dev
echo "Initial function content" > func.py
git add func.py
git commit -m "Add func.py"
echo "def new_function():\n    return 'Hello World'" > func.py
git add func.py
git commit -m "Modify func.py"
git checkout main
git merge dev -m "Merge dev into main with new func.py changes"
