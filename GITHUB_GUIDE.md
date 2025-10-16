# Gid pou Mete Pwojè w sou GitHub / Guide to Put Your Project on GitHub

## An Kreyòl Ayisyen

### Etap 1: Prepare Òdinatè w

#### Enstale Git
1. Ale sou [git-scm.com](https://git-scm.com)
2. Telechaje Git pou sistèm operasyon ou (Windows, Mac, oswa Linux)
3. Enstale l epi suiv enstriksyon yo

#### Verifye Git enstale byen
Ouvri yon terminal oswa Command Prompt epi tape:
```bash
git --version
```
Si w wè yon nimewo vèsyon, Git enstale kòrèkteman.

### Etap 2: Konfigure Git

Konfigure non w ak imel ou:
```bash
git config --global user.name "Non Ou"
git config --global user.email "email@example.com"
```

### Etap 3: Kreye Kont GitHub

1. Ale sou [github.com](https://github.com)
2. Klike sou "Sign up"
3. Ranpli enfòmasyon yo:
   - Chwazi yon non itilizatè
   - Mete adrès imel ou
   - Kreye yon modpas solid
4. Verifye imel ou
5. Konplete pwofil ou

### Etap 4: Kreye yon Nouvo Repository

1. Konekte ou sou GitHub
2. Klike sou bouton "+" an wo adwat paj la
3. Chwazi "New repository"
4. Ranpli enfòmasyon yo:
   - **Repository name**: Bay yon non (pa egzanp: "boulanje")
   - **Description**: (opsyonèl) Dekri pwojè a
   - **Public/Private**: Chwazi si moun ka wè repo a oswa non
   - **Initialize with README**: Pa check sa a si w deja gen fichye yo
5. Klike "Create repository"

### Etap 5: Pouse Pwojè w sou GitHub

#### Si se premye fwa w ap itilize Git pou pwojè sa a:

```bash
# 1. Navige nan dosye pwojè w la
cd /chemen/pou/pwojè/ou

# 2. Inisyalize Git
git init

# 3. Ajoute tout fichye yo
git add .

# 4. Fè premye commit ou
git commit -m "Premye commit: Ajoute tout fichye pwojè a"

# 5. Konekte ak repo GitHub ou (ranplase USERNAME ak REPO-NAME)
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# 6. Pouse kòd la sou GitHub
git push -u origin main
```

**Nòt**: Si w gen pwoblèm ak branch "main", eseye ak "master":
```bash
git branch -M main
git push -u origin main
```

#### Si w deja gen yon repo lokal:

```bash
# Ajoute remote GitHub
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# Pouse kòd la
git push -u origin main
```

### Etap 6: Fè Chanjman ak Push

Chak fwa w fè chanjman:

```bash
# 1. Wè ki fichye ki chanje
git status

# 2. Ajoute fichye yo
git add .

# 3. Fè commit ak yon mesaj
git commit -m "Dekri chanjman ou yo"

# 4. Pouse sou GitHub
git push
```

### Etap 7: Mete Sit Wèb la Sou Entènèt (GitHub Pages)

1. Ale nan repo GitHub ou
2. Klike sou "Settings"
3. Klike sou "Pages" nan menu agoch
4. Anba "Source":
   - Chwazi branch "main"
   - Chwazi folder "/" (root)
5. Klike "Save"
6. Tann kèk minit
7. Sit wèb ou ap disponib nan: `https://USERNAME.github.io/REPO-NAME/`

### Kòmand Git ki Enpòtan

| Kòmand | Aksyon |
|--------|--------|
| `git status` | Wè estati fichye yo |
| `git add .` | Ajoute tout fichye yo |
| `git commit -m "mesaj"` | Kreye yon commit |
| `git push` | Voye chanjman yo sou GitHub |
| `git pull` | Resevwa dènye chanjman sou GitHub |
| `git clone URL` | Kopye yon repo GitHub |
| `git log` | Wè istorik commit yo |

### Pwoblèm Komen ak Solisyon

#### Pwoblèm 1: "git: command not found"
**Solisyon**: Git pa enstale. Swiv etap 1 pou enstale Git.

#### Pwoblèm 2: "Permission denied (publickey)"
**Solisyon**: Itilize HTTPS olye SSH, oswa konfigure SSH keys.

#### Pwoblèm 3: "failed to push some refs"
**Solisyon**: 
```bash
git pull origin main --rebase
git push origin main
```

---

## In English

### Step 1: Prepare Your Computer

#### Install Git
1. Go to [git-scm.com](https://git-scm.com)
2. Download Git for your operating system (Windows, Mac, or Linux)
3. Install it and follow the instructions

#### Verify Git is installed
Open a terminal or Command Prompt and type:
```bash
git --version
```
If you see a version number, Git is installed correctly.

### Step 2: Configure Git

Set your name and email:
```bash
git config --global user.name "Your Name"
git config --global user.email "email@example.com"
```

### Step 3: Create a GitHub Account

1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Fill in the information:
   - Choose a username
   - Enter your email address
   - Create a strong password
4. Verify your email
5. Complete your profile

### Step 4: Create a New Repository

1. Log in to GitHub
2. Click the "+" button at the top right
3. Choose "New repository"
4. Fill in the details:
   - **Repository name**: Give it a name (e.g., "boulanje")
   - **Description**: (optional) Describe the project
   - **Public/Private**: Choose if people can see the repo or not
   - **Initialize with README**: Don't check this if you already have files
5. Click "Create repository"

### Step 5: Push Your Project to GitHub

#### If this is your first time using Git for this project:

```bash
# 1. Navigate to your project folder
cd /path/to/your/project

# 2. Initialize Git
git init

# 3. Add all files
git add .

# 4. Make your first commit
git commit -m "First commit: Add all project files"

# 5. Connect to your GitHub repo (replace USERNAME and REPO-NAME)
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# 6. Push the code to GitHub
git push -u origin main
```

**Note**: If you have issues with the "main" branch, try with "master":
```bash
git branch -M main
git push -u origin main
```

#### If you already have a local repo:

```bash
# Add GitHub remote
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# Push the code
git push -u origin main
```

### Step 6: Make Changes and Push

Each time you make changes:

```bash
# 1. See which files changed
git status

# 2. Add the files
git add .

# 3. Commit with a message
git commit -m "Describe your changes"

# 4. Push to GitHub
git push
```

### Step 7: Deploy the Website Online (GitHub Pages)

1. Go to your GitHub repository
2. Click "Settings"
3. Click "Pages" in the left menu
4. Under "Source":
   - Select branch "main"
   - Select folder "/" (root)
5. Click "Save"
6. Wait a few minutes
7. Your website will be available at: `https://USERNAME.github.io/REPO-NAME/`

### Important Git Commands

| Command | Action |
|---------|--------|
| `git status` | Check file status |
| `git add .` | Add all files |
| `git commit -m "message"` | Create a commit |
| `git push` | Send changes to GitHub |
| `git pull` | Get latest changes from GitHub |
| `git clone URL` | Copy a GitHub repo |
| `git log` | View commit history |

### Common Problems and Solutions

#### Problem 1: "git: command not found"
**Solution**: Git is not installed. Follow step 1 to install Git.

#### Problem 2: "Permission denied (publickey)"
**Solution**: Use HTTPS instead of SSH, or configure SSH keys.

#### Problem 3: "failed to push some refs"
**Solution**: 
```bash
git pull origin main --rebase
git push origin main
```

## Resous Siplemantè / Additional Resources

- [GitHub Documentation](https://docs.github.com)
- [Git Tutorial](https://git-scm.com/docs/gittutorial)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Desktop](https://desktop.github.com) - Aplikasyon Desktop pou Git (si w pa renmen liy kòmand)
