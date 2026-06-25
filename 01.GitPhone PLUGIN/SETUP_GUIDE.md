# 📱 GitPhone Setup Guide – Zero to GitHub on Android
**No laptop, no prior experience needed.**

This guide turns your Android phone into a full Git development machine with Termux, a code editor, and GitHub. Every step is typed by hand — that’s how you learn.

---

## Table of Contents
1. [What You Need](#1-what-you-need)
2. [Install Termux](#2-install-termux)
3. [Termux First‑Run Setup](#3-termux-first‑run-setup)
4. [Install a Code Editor (Acode)](#4-install-a-code-editor-acode)
5. [Create a GitHub Account & Token](#5-create-a-github-account--token)
6. [Configure Git in Termux](#6-configure-git-in-termux)
7. [Clone the GitPhone Course](#7-clone-the-gitphone-course)
8. [Daily Workflow: Edit → Stage → Commit → Push](#8-daily-workflow-edit--stage--commit--push)
9. [Common Errors & Fixes](#9-common-errors--fixes)
10. [Next Steps](#10-next-steps)

---

## 1. What You Need
- An Android phone (Android 7 or newer)
- Internet connection
- A free GitHub account (created in Section 5)
- Willingness to type every command yourself

All tools are free and open‑source.

---

## 2. Install Termux
Termux is a terminal that gives you a Linux environment on Android without root.

**Important:** Do **not** install from Google Play (it’s outdated). Use F‑Droid instead.

- Open your phone browser and go to:  
  `https://f-droid.org/repo/com.termux_118.apk`
- Download and install the APK. You may need to allow “Install from unknown sources” in Settings → Security.
- Open Termux. You’ll see a black screen with a `$` prompt.

---

## 3. Termux First‑Run Setup
Wait until the initial installation finishes (you’ll see the `$` prompt ready). Then run these commands **one at a time**:

```bash
pkg update
```

(If asked, type y and press Enter.)

```bash
pkg upgrade
```

Install essential packages:

```bash
pkg install python git -y
```

Verify they work:

```bash
python --version
git --version
```

Grant storage access so Termux can see your phone’s files:

```bash
termux-setup-storage
```

Tap Allow when the pop‑up appears.

---

4. Install a Code Editor (Acode)

Acode is a free, powerful editor with syntax highlighting and a file browser.

· Open the Play Store, search for Acode by Foxdebug, and install it.
· Open Acode and grant storage permissions.
· You’ll use Acode to write and edit lesson files; Termux will run the commands.

---

5. Create a GitHub Account & Token

5.1 Sign Up

· Go to https://github.com/signup in your browser.
· Choose a professional username, enter your email and password.

5.2 Create a Personal Access Token (PAT)

GitHub no longer accepts passwords in the terminal. You must use a token.

· On GitHub, tap your avatar (top right) → Settings.
· Scroll down to Developer settings → Personal access tokens → Tokens (classic).
· Tap Generate new token → Generate new token (classic).
· Note: “Termux phone”.
· Set an expiration (e.g., 90 days) or no expiration if you prefer.
· Under Select scopes, check the box repo (full control of your repositories).
· Tap Generate token at the bottom.
· Copy the token immediately and save it in a secure note — you won’t see it again. You’ll use this token instead of a password.

---

6. Configure Git in Termux

In Termux, set your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Store your token so you don’t have to enter it every time:

```bash
git config --global credential.helper store
```

The first time you push, Git will ask for:

· Username: your GitHub username (e.g., Emperor1456)
· Password: paste the personal access token you created

After that, Git remembers it.

---

7. Clone the GitPhone Course

Now get the entire GitPhone curriculum onto your phone.

In Termux, go to the Download folder (easy access from both Termux and Acode):

```bash
cd /storage/emulated/0/Download
```

Clone the repository (replace the URL if yours is different):

```bash
git clone https://github.com/Emperor1456/GitPhone_Emperor.git
```

Enter the course folder:

```bash
cd GitPhone_Emperor
```

List the contents to see all modules:

```bash
ls
```

You’re now ready to start learning.

---

8. Daily Workflow: Edit → Stage → Commit → Push

Every lesson follows this cycle. No copy‑paste. You type everything.

8.1 Open the lesson file

In Acode, navigate to Internal Storage → Download → GitPhone_Emperor and open the lesson file (e.g., L-01_git_init.md inside the module folder).

8.2 Type the commands in Termux

Follow the practice task. Run each Git command, observe the output, understand it.

8.3 Save your notes

After the lesson, write a short summary in the 04.GitPhone NOTES/ folder (optional but recommended).

8.4 Stage and commit your work

```bash
git add .
git commit -m "Complete Lesson 01: git init and git add"
```

8.5 Push to GitHub

```bash
git push origin main
```

(If you see master instead of main, use git push origin master.)

Check your GitHub repo – your progress is safely backed up and visible to the world.

---

9. Common Errors & Fixes

fatal: not a git repository
You ran a Git command outside the course folder. Navigate to GitPhone_Emperor first.

fatal: detected dubious ownership…
This happens on Android’s shared storage. Run the suggested command:

```bash
git config --global --add safe.directory /storage/emulated/0/Download/GitPhone_Emperor
```

remote: Repository not found
The GitHub URL is wrong or the repo doesn’t exist. Double‑check the URL from your GitHub account.

error: failed to push (rejected)
Remote has changes you don’t have. If your local code is correct and you want to overwrite remote (use with caution):

```bash
git push origin main --force
```

keyboard doesn’t appear in Termux
Tap once on the black terminal area to bring up the keyboard.

command not found: git
Make sure you ran pkg install git -y. If missing, install it again.

---

10. Next Steps

· Open GETTING_STARTED.md in the same folder to understand the course structure and methodology.
· Read the syllabus inside 02.GitPhone SYLLABUS/GitPhone_Curriculum.md.
· Start with Module 1, Lesson 1 inside 03.GitPhone COURSE/GitPhone_Module_01/.
· Use the AI mentor prompt (02.GitPhone SYLLABUS/GitPhone_AI_Prompt.md) with your AI assistant for personalized guidance.

Welcome to GitPhone. Your journey to mastering Git and GitHub, entirely from your phone, begins now.