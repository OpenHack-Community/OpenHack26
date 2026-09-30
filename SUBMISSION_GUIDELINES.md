<div align="center">

<img src="assets/logo.png" alt="OpenHack'26" width="200"/>

# 📦 Project Submission Guide

### Think. Build. **Push.**

![Repos](https://img.shields.io/badge/REPOSITORIES-2-bd00ff?style=for-the-badge&labelColor=0b0b0f)
![Steps](https://img.shields.io/badge/STEPS-22-9dff00?style=for-the-badge&labelColor=0b0b0f)
![Parts](https://img.shields.io/badge/PARTS-A_→_E-bd00ff?style=for-the-badge&labelColor=0b0b0f)
![Level](https://img.shields.io/badge/BEGINNER-FRIENDLY-9dff00?style=for-the-badge&labelColor=0b0b0f)

[🏠 Home](README.md) · [📜 Rules](RULES.md) · [📋 Problems](PROBLEMS.md) · [⚖️ Judging](JUDGING.md) · [🧑‍💻 GitHub Guide](GITHUB_GUIDE.md)

</div>

<img src="assets/divider.png" width="100%" height="4" alt=""/>

Welcome, Hackers! 🚀

This guide takes you through the **complete submission process from zero**, even if you are new to Git and GitHub.

## 🧭 Table of Contents

| Part | Section | Steps |
| :-: | :-- | :-: |
| ⚠️ | [Understand the Two Repositories](#two-repos) | — |
| 🔥 | [Complete Submission Flow](#flow) | — |
| 🟢 **A** | [Your Own Project Repository](#part-a) | 1–10 |
| 🟢 | [During the Hackathon](#during) | — |
| 🔵 **B** | [Submit to the Official OpenHack26 Repository](#part-b) | 11–18 |
| 🔴 **C** | [Create the Pull Request](#part-c) | 19–22 |
| 🟡 **D** | [Organizer Review](#part-d) | — |
| 🟣 **E** | [Official Submission Form](#part-e) | — |
| 📁 | [Final Repository Structure](#final-structure) | — |
| ✅ | [Final Checklist](#checklist) | — |

<img src="assets/divider.png" width="100%" height="4" alt=""/>

<a id="two-repos"></a>
## ⚠️ First: Understand the Two Repositories

For OpenHack'26, **every team will work with TWO GitHub repositories**.

<table>
<tr>
<td width="50%" valign="top">

### 🧑‍💻 1. Your Own Project Repository

Your team's **main project repository**. Your complete project is stored here, and you do your **actual development, commits, and project work here**.

Example:

```text
https://github.com/YourUsername/AI-Waste-Classifier
```

</td>
<td width="50%" valign="top">

### 🏛️ 2. Official OpenHack'26 Repository

Used for the **hackathon submission and permanent event record**. Your team will create:

```text
submissions/
└── YourTeamName/
    └── README.md
```

This README will contain your:

* Team name
* Team members
* Selected problem
* Category
* Solution
* Technologies
* Challenges
* AI/Open-source usage
* **Link to your own project repository**

</td>
</tr>
</table>

> [!IMPORTANT]
> **Do not confuse these two repositories.** Your complete project stays in **your own repository**. The OpenHack26 repository contains your **official submission record**.

<img src="assets/divider.png" width="100%" height="4" alt=""/>

<a id="flow"></a>



<img src="assets/divider.png" width="100%" height="4" alt=""/>

<a id="part-a"></a>
## 🟢 Part A — Your Own Project Repository (Steps 1–10)
 
**Step 1 — Create a GitHub repository.** Go to GitHub and create a new repo, e.g. `AI-Waste-Classifier`. Its URL will look like `https://github.com/YourUsername/AI-Waste-Classifier`. This is your **main project repository**.
 
**Step 2 — Open your project in VS Code.** Open your project folder (e.g. `AI-Waste-Classifier/`), then open the terminal: **Terminal → New Terminal**.
 
**Steps 3–10 — Run in the terminal, inside your project folder:**
 
```bash
# Step 3: Check Git installation (expect something like: git version 2.x.x)
git --version
 
# Step 4: Configure Git (first-time users only), then verify
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
git config --global --list
 
# Step 5: Initialize, turns your project folder into a Git repository
git init
 
# Step 6: Check files, shows untracked or modified files
git status
 
# Step 7: Add all files in the current project ("." = everything)
git add .
git status                  # files should now appear as staged
 
# Step 8: First commit, saves a version of your project in Git history
git commit -m "Initial project setup"
 
# Step 9: Connect to GitHub (use your repo URL), then verify it appears
git remote add origin https://github.com/YourUsername/AI-Waste-Classifier.git
git remote -v
 
# Step 10: Push (if your repo uses main)
git branch -M main
git push -u origin main
```
 
> 🎉 **Your main project repository is ready!** Your complete project should now appear on GitHub.
 
**During the hackathon**, keep working in your own repository and regularly save your work:
 
```bash
git status
git add .
git commit -m "Add user authentication"
git push
```
 
Your complete development history stays in your own GitHub repository.

<img src="assets/divider.png" width="100%" height="4" alt=""/>

 
## 🔵 Part B — Official OpenHack26 Repository (Steps 11–18)
 
> [!WARNING]
> **Never edit the official repo directly.** Fork it first.
 
1. Open the official OpenHack26 repo → **Fork → Create Fork**.
2. Clone **your fork** and add your team folder:
```bash
git clone https://github.com/YourUsername/Hackathon.git
cd Hackathon
mkdir submissions/CodeWarriors        # use your registered team name
# create submissions/CodeWarriors/README.md (template below)
 
git add .
git commit -m "Add CodeWarriors submission"
git push origin main
```
 
**Submission `README.md` template:**
 
```markdown
# Project Name
 
## Team Name
CodeWarriors
 
## Team Members
- Alice — @alicehub
- Bob — @bobdev
 
## Problem Statement
Problem 07 — [Problem Title]
 
## Category
AgriTech & Food
 
## Solution
Briefly explain your solution.
 
## Tech Stack
- React
- Node.js
- MongoDB
 
## Challenges Faced
Briefly explain your challenges.
 
## Learnings
What did your team learn?
 
## AI / Open-Source Usage
Mention AI tools, models, APIs, and open-source resources used.
 
## Project Repository
https://github.com/YourUsername/AI-Waste-Classifier
```
 
> [!IMPORTANT]
> `Project Repository` must link to **your own** project repo.

<img src="assets/divider.png" width="100%" height="4" alt=""/>

 
## 🔴 Part C — Pull Request (Steps 19–22)
 
On your fork's GitHub page click **Contribute → Open Pull Request**, and check the direction is
**`YourUsername/Hackathon` → `OpenHack-26/Hackathon`** (not the reverse).
 
**Title format:**
 
```text
[SUBMISSION] TeamName - ProjectName - Category
```
 
Example: `[SUBMISSION] CodeWarriors - AI Waste Classifier - AgriTech & Food`
 
**Description:**
 
```markdown
## Team Information
 
- **Team Name:** CodeWarriors
- **Project Name:** AI Waste Classifier
- **Problem:** Problem 07
- **Category:** AgriTech & Food
- **Team Members:** @alicehub, @bobdev
 
## Project Repository
 
https://github.com/YourUsername/AI-Waste-Classifier
 
## Submission Checklist
 
- [x] Team folder created
- [x] Submission README included
- [x] Problem identified
- [x] Project repository linked
- [x] AI/Open-source usage disclosed
```
 
Click **Create Pull Request**.


<img src="assets/divider.png" width="100%" height="4" alt=""/>

# 🟡 PART D — Organizer Review

The OpenHack26 organizing team will review your Pull Request.

If everything is correct, your submission will be merged.

If organizers request changes:

```bash
git add .
git commit -m "Update submission"
git push
```

Your existing Pull Request will automatically update.

<img src="assets/divider.png" width="100%" height="4" alt=""/>

<a id="part-e"></a>
# 🟣 PART E — Official Submission Form

After creating your Pull Request, complete the official OpenHack26 submission form.

The form will collect:

| | | |
| :-- | :-- | :-- |
| Team name | Project name | Selected problem |
| Team members | **Your own GitHub project repository URL** | OpenHack26 Pull Request URL |
| Demo video | Screenshots | Live deployment URL |
| Presentation / PPT | Other required information | |

### Example

**Your Project Repository:**

```text
https://github.com/YourUsername/AI-Waste-Classifier
```

**OpenHack26 Pull Request:**

```text
https://github.com/OpenHack-26/Hackathon/pull/123
```

<img src="assets/divider.png" width="100%" height="4" alt=""/>

<a id="final-structure"></a>
# 📁 Final Repository Structure

At the end, there will be **two separate repositories**.

### 🧑‍💻 Your Project Repository

```text
AI-Waste-Classifier/
├── README.md
├── src/
├── model/
├── requirements.txt
├── main.py
└── ...
```

### 🏛️ OpenHack26 Repository

```text
Hackathon/
└── submissions/
    ├── Team-Alpha/
    │   └── README.md
    ├── Team-Beta/
    │   └── README.md
    └── CodeWarriors/
        └── README.md
```

<img src="assets/divider.png" width="100%" height="4" alt=""/>

<a id="checklist"></a>
# ✅ Final Checklist

### 🧑‍💻 Your Own GitHub Repository

* [ ] GitHub repository created
* [ ] Project initialized with Git
* [ ] `git add` completed
* [ ] Initial commit created
* [ ] Remote repository connected
* [ ] Project pushed
* [ ] Development work committed regularly
* [ ] Final project pushed

### 🏛️ OpenHack26 Repository

* [ ] Official repository forked
* [ ] Fork cloned
* [ ] `submissions/` opened
* [ ] Team folder created
* [ ] Submission README created
* [ ] Own project repository linked
* [ ] Changes committed
* [ ] Changes pushed
* [ ] Pull Request created
* [ ] Pull Request submitted for review

### 📝 Official Form

* [ ] Team information completed
* [ ] Own GitHub repository URL provided
* [ ] Pull Request URL provided
* [ ] Demo video provided if required
* [ ] Screenshots provided if required
* [ ] Deployment URL provided if available
* [ ] Form submitted

<img src="assets/divider.png" width="100%" height="4" alt=""/>

# ⚠️ Important

* Use your registered team name.
* Do not modify another team's submission.
* Do not submit another team's project.
* External people must not develop the project for your team.
* AI tools and open-source technologies are allowed according to the hackathon rules.
* Make sure all submitted links are accessible.
* Submit before the official deadline.

<img src="assets/divider.png" width="100%" height="4" alt=""/>

<div align="center">

### 🚀 Build → Commit → Push → Submit → Demo

**Think. Build. Push.**

**OpenHack'26 — Build. Solve. Demonstrate. ❤️**

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0b0b0f,100:bd00ff&height=100&section=footer" width="100%" alt="footer"/>