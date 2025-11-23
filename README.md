# GitHub Collaboration Guide

## Overview

This guide explains how to collaborate on your capstone project using GitHub. You'll learn how to fork a repository, work together, and merge your contributions. This guide applies to all groups (Group 1, Group 2, Group 3, and Group 4).

## Step 1: Create the Main Repository

**One person in your group** should:

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right → "New repository"
3. Name it: `capstone-groupX` (replace X with your group number, or your preferred name)
4. Make it **Public** (so everyone can access it)
5. Add a README.md file
6. Click "Create repository"

## Step 2: Add Collaborators

**The repository owner** should:

1. Go to your repository
2. Click "Settings" → "Collaborators"
3. Click "Add people"
4. Add all group members by their GitHub usernames
5. Everyone accepts the invitation

## Step 3: Fork the Repository (Alternative Method)

If you prefer individual forks:

1. Each member goes to the main repository
2. Click "Fork" button (top right)
3. This creates your own copy of the repository
4. Work on your fork, then create Pull Requests to merge back

## Step 4: Clone the Repository

**Everyone** should:

1. Go to the main repository (or your fork)
2. Click the green "Code" button
3. Copy the repository URL
4. Open terminal/command prompt
5. Run:
   ```bash
   git clone https://github.com/username/capstone-groupX.git
   cd capstone-groupX
   ```

## Step 5: Create a Branch for Your Work

**Before making changes**, create a branch:

```bash
git checkout -b your-name-work
# Example: git checkout -b john-notebook-section
# Example: git checkout -b sarah-data-collection
```

This keeps your work separate from others.

## Step 6: Make Your Changes

1. Work on your notebook or files
2. Save your changes
3. Test that everything works

## Step 7: Commit Your Changes

When you're ready to save your work:

```bash
# Add your changes
git add .

# Or add specific files
git add capstone_notebook.ipynb
git add README.md

# Commit with a message
git commit -m "Added data collection section to notebook"
```

**Good commit messages**:
- "Added model training section"
- "Updated README with setup instructions"
- "Fixed preprocessing code"
- "Added design thinking summary"
- "Improved model accuracy with fine-tuning"

## Step 8: Push Your Changes

Push your branch to GitHub:

```bash
git push origin your-name-work
```

## Step 9: Create a Pull Request (If Using Forks)

If you're using forks:

1. Go to your fork on GitHub
2. Click "Contribute" → "Open pull request"
3. Write a description of your changes
4. Click "Create pull request"
5. Wait for review and merge

## Step 10: Merge Changes (If Using Branches)

**The repository owner or a collaborator** can merge:

1. Go to the repository on GitHub
2. Click "Pull requests" tab
3. Review the changes
4. Click "Merge pull request"
5. Confirm the merge

## Step 11: Update Your Local Copy

**After someone merges changes**, update your local copy:

```bash
git checkout main
git pull origin main
```

This gets the latest changes from others.

## Collaboration Best Practices

### ✅ Do's

- **Communicate**: Tell your group what you're working on
- **Pull before push**: Always pull latest changes before pushing
- **Use branches**: Don't work directly on main branch
- **Commit often**: Save your work regularly
- **Write clear messages**: Explain what you changed
- **Test before commit**: Make sure your code works

### ❌ Don'ts

- **Don't commit API keys**: Use environment variables
- **Don't delete others' work**: Be careful with git commands
- **Don't work on same file simultaneously**: Coordinate with your group
- **Don't force push**: Can overwrite others' work
- **Don't commit large files**: Use Git LFS if needed

## Resolving Conflicts

If you get a **merge conflict**:

1. Don't panic! This is normal when multiple people edit the same file
2. Git will mark the conflicts in the file
3. Open the file and look for conflict markers:
   ```
   <<<<<<< HEAD
   Your changes
   =======
   Their changes
   >>>>>>> branch-name
   ```
4. Decide which version to keep (or combine both)
5. Remove the conflict markers
6. Save the file
7. Commit the resolved file:
   ```bash
   git add filename
   git commit -m "Resolved merge conflict"
   ```

## Common Git Commands

```bash
# Check status
git status

# See what changed
git diff

# See commit history
git log

# Switch branches
git checkout branch-name

# Create new branch
git checkout -b new-branch-name

# Discard local changes (be careful!)
git checkout -- filename

# See all branches
git branch

# Delete a branch (after merging)
git branch -d branch-name
```

## Getting Help

If you're stuck:

1. **GitHub Help**: https://docs.github.com
2. **Git Tutorial**: https://git-scm.com/docs
3. **Ask your group**: Someone might know the answer
4. **Ask instructor**: During mentoring session or class

## Final Submission Checklist

Before Session 10, make sure:

- [ ] All notebook sections are complete
- [ ] README.md is complete with setup instructions
- [ ] All code is committed and pushed
- [ ] Repository is public and accessible
- [ ] No API keys are in the code
- [ ] All group members have contributed
- [ ] Repository link is ready for presentation

## Quick Reference

**Daily workflow**:
```bash
git pull origin main          # Get latest changes
git checkout -b my-work       # Create branch for your work
# ... make changes ...
git add .
git commit -m "Description"
git push origin my-work       # Push your branch
# Create pull request on GitHub
```

**Good luck with your collaboration! 🚀**

