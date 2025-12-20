# EnterInSync

## 🚀 Quick Setup

### Conda Environment (Local to Project)

This project uses a **local conda environment** stored in `.conda/` folder.

#### Creating the Local Environment (First Time)

```bash
# Create a local conda environment in the project directory
conda create -p "e:\CODING\06_Personal Builds\15_EnterInSync\.conda" python=3.11 -y
```

#### Local vs Named Environments

**Local Environment (What we're using):**
- ✅ Created with `-p` (prefix) flag
- ✅ Stored in project directory: `.conda/`
- ✅ Project-specific and self-contained
- ✅ Easy to delete/recreate (just delete the folder)
- ✅ Better for version control (add to `.gitignore`)
- ❌ Path-dependent (must use full path)

**Named Environment (Default conda):**
- Created with `-n` (name) flag: `conda create -n myenv python=3.11`
- Stored centrally: `C:\Users\Rahul\anaconda3\envs\myenv`
- Shared across all projects
- Activated by name: `conda activate myenv`
- Can cause conflicts between projects

```bash
# Activate the environment
conda activate "e:\CODING\06_Personal Builds\15_EnterInSync\.conda"

# Install new packages
conda install -p "e:\CODING\06_Personal Builds\15_EnterInSync\.conda" <package-name> -y

# Install ipykernel (for Jupyter notebooks)
conda install -p "e:\CODING\06_Personal Builds\15_EnterInSync\.conda" ipykernel --update-deps --force-reinstall -y
```

**Note**: The `.conda` folder is gitignored and can be several GB in size.

---

