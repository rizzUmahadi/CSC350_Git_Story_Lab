# CSC350 Pre-Class Quiz — Update Activity 2

**Time:** 15 minutes  
**Goal:** Use the Lab 1 strategy: **Predict → Execute → Read → Verify**

## Important

Complete this quiz independently in your existing Lab 1 repository.

- Do not delete this repository.
- Do not run `git init`, `git add .`, `git push`, or `git pull`.
- This quiz ends with a **local commit**.
- Use the exact file path `activities/02_REMOTE_SYNC.md`.

After the quiz, your pair will select one repository as the **Author repository**. The other student will preserve the original folder and clone the pair's GitHub repository into a new folder for Lab 2.

---

## 1. Check the starting state — 2 minutes

Open your existing Lab 1 repository in VS Code and open the terminal.

### Predict

What branch and repository condition do you expect?

____________________________________________________________________________

### Execute

```bash
git status
git branch --show-current
git log --oneline --decorate -3
```

### Evidence

- Current branch: ____________________
- Newest commit message: _________________________________________________
- Does `git status` report a clean working tree? __________________________

Stop and ask for help if the branch is not `main`, your Lab 1 commit is missing, or the working tree is not clean.

---

## 2. Replace and inspect Activity 2 — 4 minutes

Download the revised `02_REMOTE_SYNC.md` supplied by your instructor. Replace the old file at:

```text
activities/02_REMOTE_SYNC.md
```

Do not create `02_REMOTE_SYNC (1).md`. Open the revised file in VS Code and save it.

### Predict

Before running the next command:

1. Where does the change currently live? __________________________________
2. Is it staged? __________________________________________________________
3. Has a new commit been created? _________________________________________

### Execute

```bash
git status
git diff -- activities/02_REMOTE_SYNC.md
```

### Evidence

- Under which `git status` section does the file appear?

  __________________________________________________________________________

- Write one important change shown by `git diff`:

  __________________________________________________________________________

- Is any other file modified? ______________________________________________

Only `activities/02_REMOTE_SYNC.md` should be modified.

---

## 3. Stage and verify — 3 minutes

### Predict

After `git add`, where will Git place the revised snapshot?

____________________________________________________________________________

### Execute

```bash
git add activities/02_REMOTE_SYNC.md
git status
git diff --staged -- activities/02_REMOTE_SYNC.md
```

### Evidence

- Under which `git status` section does the file now appear?

  __________________________________________________________________________

- Does the staged diff contain the intended Activity 2 revision? ___________
- Is any unrelated file staged? ____________________________________________

Do not continue if an unrelated file is staged. Ask the instructor for help.

---

## 4. Commit locally — 2 minutes

### Predict

After the commit, where will the revised snapshot be recorded?

____________________________________________________________________________

Will it automatically appear on GitHub? ____________________________________

### Execute

```bash
git commit -m "Update remote synchronization instructions"
```

Record the short commit ID reported by Git:

Commit ID: __________________________

---

## 5. Verify the result — 2 minutes

```bash
git status
git log --oneline --decorate -3
```

### Final evidence

- Final `git status`: ______________________________________________________
- Newest commit message: _________________________________________________
- Does `HEAD -> main` point to the new commit? _____________________________

### Success checklist

- [ ] The working tree is clean.
- [ ] `Update remote synchronization instructions` is the newest commit.
- [ ] The revised file is located at `activities/02_REMOTE_SYNC.md`.
- [ ] No remote command was used.

---

## 6. Short explanation — 2 minutes

Answer in one sentence each.

1. What is the difference between `git diff` and `git diff --staged`?

   __________________________________________________________________________

2. Why can your partner not receive this new commit yet?

   __________________________________________________________________________

3. What evidence proves that your commit succeeded?

   __________________________________________________________________________

## Submit

Submit this completed quiz and evidence showing the output of:

```bash
git status
git log --oneline --decorate -3
```

Do not submit passwords or authentication information.