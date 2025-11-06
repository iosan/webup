# GitHub Workflows - Issue Fixed ✅

## Problem Solved

**Issue:** GitHub Actions was failing with `./configure: No such file or directory`

**Root Cause:** A default `makefile.yml` workflow template (for C/C++ autotools projects) was trying to run `./configure`, which doesn't exist in this static HTML/CSS website.

**Solution:** Removed incorrect workflow and created proper static site workflows.

---

## Current Workflows

### `deploy.yml` - GitHub Pages Deployment
Automatically deploys the `html/` directory to GitHub Pages when code is pushed to `master` or `main` branches.

**Setup Required:**
1. Go to repository Settings → Pages
2. Set Source to "GitHub Actions"
3. Push to trigger deployment

**Triggers:**
- Push to `master` or `main` branch
- Manual workflow dispatch

### `build.yml` - Build and Validation
Builds documentation (diagrams and PDFs) and optionally validates HTML/CSS.

**Triggers:**
- Push to `master` or `main` branch
- Pull requests to `master` or `main` branch

**Artifacts:**
- Generated PDFs (docs/*.pdf)
- Generated diagrams (docs/images/*.png)

---

## Important Note

⚠️ **This is a static HTML/CSS website** - there is NO compilation step, no `./configure` script, and no C/C++ build process. The workflows directly deploy the `html/` directory or build documentation using the project's Makefile.
