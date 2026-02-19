# alpha

# ============================
# 1. Create local folders
# ============================
mkdir c:\mygit\alpha
mkdir c:\mygit\bravo

# ============================
# 2. Initialize Git (alpha)
# ============================
cd c:\mygit\alpha
git init
git add .
git commit -m "Initial commit"

# ============================
# 3. Initialize Git (bravo)
# ============================
cd c:\mygit\bravo
git init
git add .
git commit -m "Initial commit"

# ============================
# 4. Create GitHub repos
# ============================
# On GitHub (web):
#   Go to https://github.com/PetroAI1492
#   Click "New"
#   Create repo named: alpha   (empty)
#   Create repo named: bravo   (empty)

# ============================
# 5. Connect alpha to GitHub
# ============================
cd c:\mygit\alpha
git remote add origin https://github.com/PetroAI1492/alpha.git
git branch -M main
git push -u origin main

# ============================
# 6. Connect bravo to GitHub
# ============================
cd c:\mygit\bravo
git remote add origin https://github.com/PetroAI1492/bravo.git
git branch -M main
git push -u origin main

# ============================
# 7. Daily workflow
# ============================
# Update alpha
cd c:\mygit\alpha
git add .
git commit -m "update"
git push

# Update bravo
cd c:\mygit\bravo
git add .
git commit -m "update"
git push

