# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Replace the default profile README with a playful developer card for Tacoo.

**Architecture:** This is a Markdown-only profile README. The README uses centered HTML blocks where GitHub Markdown benefits from alignment, remote badge/stat SVGs for visual polish, and plain Markdown lists for readable content.

**Tech Stack:** GitHub Markdown, Shields.io badges, Readme Typing SVG, GitHub Readme Stats, GitHub Streak Stats.

---

## File Structure

- Modify: `README.md`
  - Owns the public GitHub profile content shown on `takotaks/takotaks`.
  - Contains the header, typing banner, stack badges, AI toolkit, current focus, stats, and closing line.

## Tasks

### Task 1: Replace Default README

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Replace the default template with the profile README**

Write this complete content to `README.md`:

```markdown
<div align="center">

# Hi, I'm Tacoo

### Python tinkerer, React explorer, and Node.js builder

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=36BCF7&center=true&vCenter=true&width=520&lines=Python+tinkerer;React+explorer;Node.js+builder;Linux+learner;Web+project+maker" alt="Typing SVG" />

</div>

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

**Tools and Platform**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Hostinger](https://img.shields.io/badge/Hostinger-673DE6?style=for-the-badge&logo=hostinger&logoColor=white)

**AI Toolkit**

![ChatGPT](https://img.shields.io/badge/ChatGPT-00A67E?style=for-the-badge&logo=openai&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-000000?style=for-the-badge&logo=githubcopilot&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor-000000?style=for-the-badge&logo=cursor&logoColor=white)
![Codex](https://img.shields.io/badge/Codex-111111?style=for-the-badge&logo=openai&logoColor=white)

---

## Current Focus

- Building web projects that are useful, clean, and fun to use
- Practicing React and Node.js one feature at a time
- Improving my Linux workflow and developer setup
- Experimenting with hosting, deployment, and AI-assisted coding

---

## GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=takotaks&show_icons=true&theme=tokyonight&hide_border=true" alt="Tacoo's GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=takotaks&layout=compact&theme=tokyonight&hide_border=true" alt="Tacoo's top languages" />

<br />

<img src="https://streak-stats.demolab.com?user=takotaks&theme=tokyonight&hide_border=true" alt="Tacoo's GitHub streak" />

</div>

---

<div align="center">

Thanks for stopping by. Check out my projects and follow along while I keep building.

</div>
```

- [ ] **Step 2: Verify every approved stack item appears**

Run:

```powershell
Select-String -Path 'README.md' -Pattern 'Python|JavaScript|React|HTML5|CSS3|Node.js|Git|VS Code|Linux|Hostinger|ChatGPT|Claude|GitHub Copilot|Cursor|Codex'
```

Expected: output includes matches for every approved tech and AI tool.

- [ ] **Step 3: Verify stats use the correct username**

Run:

```powershell
Select-String -Path 'README.md' -Pattern 'username=takotaks|user=takotaks'
```

Expected: output includes both GitHub Readme Stats URLs and the streak stats URL.

- [ ] **Step 4: Review final README content**

Run:

```powershell
Get-Content -LiteralPath 'README.md'
```

Expected: README shows the playful Tacoo profile and no longer contains the default GitHub template comment.

- [ ] **Step 5: Commit implementation**

Run:

```powershell
git add README.md docs\superpowers\plans\2026-05-21-github-profile-readme.md
git commit -m "Update profile README"
```

Expected: commit succeeds with the README and plan changes.
