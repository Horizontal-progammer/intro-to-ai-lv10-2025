# GitHub Collaboration Guide

## Overview

This guide explains how to collaborate on your capstone project using GitHub. **All groups will work in a single shared repository** to learn collaboration. Each group has their own folder (Group1, Group2, Group3, Group4) where they will place their capstone project files.

**Repository**: https://github.com/Praxis-High-School/intro-to-ai-lv10-2025

## Repository Structure

```
intro-to-ai-lv10-2025/
├── README.md (this file)
├── Group1/     (Group 1's workspace)
├── Group2/     (Group 2's workspace)
├── Group3/     (Group 3's workspace)
└── Group4/     (Group 4's workspace)
```

**Important**: Each group works in their own folder. Don't modify other groups' folders!

## Step 1: Clone the Shared Repository

**Everyone** should:

1. Go to the repository: https://github.com/Praxis-High-School/intro-to-ai-lv10-2025
2. Click the green "Code" button
3. Copy the repository URL
4. Open terminal/command prompt
5. Run:
   ```bash
   git clone https://github.com/Praxis-High-School/intro-to-ai-lv10-2025.git
   cd intro-to-ai-lv10-2025
   ```

**Note**: The repository is already set up. You don't need to create a new one!

## Step 2: Navigate to Your Group Folder

After cloning, navigate to your group's folder:

```bash
# For Group 1
cd Group1

# For Group 2
cd Group2

# For Group 3
cd Group3

# For Group 4
cd Group4
```

**Remember**: Work only in your group's folder. Don't modify other groups' work!

## Step 3: Create a Branch for Your Work

**Before making changes**, create a branch:

```bash
git checkout -b your-name-work
# Example: git checkout -b john-notebook-section
# Example: git checkout -b sarah-data-collection
```

This keeps your work separate from others.

## Step 4: Make Your Changes

1. Work on your notebook or files
2. Save your changes
3. Test that everything works

## Step 5: Commit Your Changes

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

## Step 6: Push Your Changes

Push your branch to GitHub:

```bash
git push origin your-name-work
```

## Step 7: Create a Pull Request

When you're ready to merge your branch:

1. Go to the repository on GitHub: https://github.com/Praxis-High-School/intro-to-ai-lv10-2025
2. You should see a banner suggesting to create a pull request for your branch
3. Click "Compare & pull request"
4. Write a description of your changes (e.g., "Added Group1 capstone notebook")
5. Make sure the base branch is `main` and compare branch is your branch
6. Click "Create pull request"
7. Wait for review (instructor or group member can review)
8. Once approved, click "Merge pull request"

## Step 8: Update Your Local Copy

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

- [ ] All notebook sections are complete in your group folder
- [ ] README.md is in your group folder with setup instructions
- [ ] All code is committed and pushed to the shared repository
- [ ] All changes are merged to main branch via pull request
- [ ] No API keys are in the code
- [ ] All group members have contributed
- [ ] Your group folder contains: `capstone_notebook.ipynb` and `README.md`
- [ ] Repository link is ready for presentation: https://github.com/Praxis-High-School/intro-to-ai-lv10-2025

## Quick Reference

**Daily workflow**:
```bash
cd intro-to-ai-lv10-2025     # Navigate to repository
cd GroupX                     # Go to your group folder (replace X with your group number)
git pull origin main          # Get latest changes
git checkout -b my-work       # Create branch for your work
# ... make changes in your group folder ...
git add GroupX/               # Add your group's changes
git commit -m "Description"
git push origin my-work       # Push your branch
# Create pull request on GitHub
```

**Important Notes**:
- Always work in your group's folder (Group1, Group2, Group3, or Group4)
- Don't modify files outside your group folder
- Pull latest changes before starting work each day
- Create branches for your individual contributions
- Use pull requests to merge your work

**Good luck with your collaboration! 🚀**

