# Gravity_FOSS_Wing_SelectionTasks_2026

## Task Structure

All three task branches must be created directly from the clean `main` branch and remain completely isolated from one another. Work done in one task must not carry over into another task.

```text
main
│
├── name_rollnumber_task1 (Task 1 Branch - 20 Points)
│   ├── feature branch (for Task 1 feature work)
│   └── output/name_rollnumber_task1/ (output screenshots)
│
├── name_rollnumber_task2 (Task 2 Branch - 50 Points)
│   ├── branch-a
│   ├── branch-b
│   └── output/name_rollnumber_task2/ (output screenshots)
│
└── name_rollnumber_task3 (Task 3 Branch - 30 Points)
    ├── Feature A (feature branch)
    ├── Feature B (rebase-task branch)
    └── output/name_rollnumber_task3/ (output screenshots)
```

### Point Distribution Summary (100 Points Total)

| Task | Title | Points |
| :--- | :--- | :---: |
| **Task 1** | Git Basics | 20 Points |
| **Task 2** | Practical Git Workflow (Branching, Conflicts, Resets, Reflog) | 50 Points |
| **Task 3** | Cherry-Pick and Rebase | 30 Points |
| **Total** | | **100 Points** |

---

## Instructions

Follow these steps carefully to complete and submit your work:

1. **Fork the Repository**:
   - Fork this repository to your personal GitHub account and clone the forked repository to your local machine.

2. **Complete Branch Isolation**:
   - For each task, switch to the `main` branch first to ensure a clean starting point.
   - Create a separate task branch using the format: `name_rollnumber_tasknumber` (for example, `rahul_iec2024001_task1`, `rahul_iec2024001_task2`, `rahul_iec2024001_task3`).
   - Keep all tasks isolated. Do not merge task branches into one another.

3. **Output Screenshots Directory**:
   - In the repository, create a folder named `output`.
   - Inside `output`, create a dedicated subfolder for each task using the format: `name_rollnumber_tasknumber` (for example, `output/rahul_iec2024001_task1/`).
   - Save all required screenshots of your terminal outputs, status, and commit histories inside that specific subfolder.

4. **Pull Request Submission**:
   - Push each task branch to your forked GitHub repository.
   - Open a separate Pull Request for each task from your task branch to the original repository.
   - Title each Pull Request using the format: `name_rollnumber_tasknumber` (for example, `rahul_iec2024001_task1`).

---

## Task 1: Git Basics

Perform the following operations in order on an isolated branch.

### Setup for Task 1
- Switch to `main` and create a new branch named `name_rollnumber_task1`.
- Inside `output`, create a folder named `output/name_rollnumber_task1` to store your screenshots for this task.

### 1. First Commit
- Create a simple text file (for example, introducing yourself or listing your technical interests).
- Stage the file and make your very first commit with a clear message.

### 2. Viewing Commit History
- View your repository's commit history using the standard log view.
- Try different log views:
  - View the log as a single line per commit.
  - View the log showing the summary of changed files and line counts.
  - View the log showing the exact line-by-line differences.
- Save screenshots of these log views in `output/name_rollnumber_task1/`.

### 3. Modifying the Last Commit (Amend)
- Make a change to your text file (such as adding another line of text).
- Instead of creating a brand new commit, amend your previous commit so that the new changes are combined into it, and update the commit message.
- Verify in your log history that only one commit exists with the updated message and changes.
- Save a screenshot showing the amended commit in your log history in `output/name_rollnumber_task1/`.

### 4. Submit Task 1
- Ensure all required screenshots are saved in `output/name_rollnumber_task1/`.
- Commit your changes and push the `name_rollnumber_task1` branch to your fork.
- Open a Pull Request with the title `name_rollnumber_task1`.

---

## Task 2: Practical Git Workflow

Perform the following operations in order on an isolated branch.

### Setup for Task 2
- Switch back to `main` and create a new branch named `name_rollnumber_task2`.
- Inside `output`, create a folder named `output/name_rollnumber_task2` to store your screenshots for this task.

### 1. Create Branch A
- Create an initial commit named "Initial Commit" on your branch.
- Create a new branch called "branch-a" from here and switch to it.
- Make 5 separate commits with the following names:
  - "Task A1"
  - "Task A2"
  - "Task A3"
  - "Task A4"
  - "Task A5"
- After making all commit, check your repository history across all branches.

### 2. Create Branch B
- Switch back to your task branch.
- Create a new branch called "branch-b" and switch to it.
- Make 5 separate commits with the following names:
  - "Task B1"
  - "Task B2"
  - "Task B3"
  - "Task B4"
  - "Task B5"
- After making all commit, check your repository history across all branches.

### 3. Merge and Resolve Conflict
- While on "branch-b", merge "branch-a" into "branch-b".
- Git will report a merge conflict. Open the conflicting file and resolve the conflict manually.
- Complete the merge by staging the resolved file and finalizing the merge commit.
- Display the complete commit history to confirm the merge.
- Save a screenshot showing the conflict resolution and the merged commit history in `output/name_rollnumber_task2/`.

### 4. Soft Reset
- Create a new commit named "Task Soft Reset".
- Perform a soft reset to go back by one commit.
- Check the history and repository status:
  - Confirm that the commit is removed from the history.
  - Confirm that the file changes from that commit are still staged and ready to be committed.
- Save a screenshot of the status showing staged changes in `output/name_rollnumber_task2/`.
- Delete or unstage these changes, and verify that your status is clean.

### 5. Hard Reset the Last 5 Commits
- Display the history graph.
- Perform a hard reset to remove the last 5 commits completely.
- Check the history graph and status to confirm that the last 5 commits and all their changes have been deleted.
- Save a screenshot showing the history after the hard reset in `output/name_rollnumber_task2/`.

### 6. Recovery Using Reflog
- Inspect the reference log (reflog) to see the history of HEAD movements.
- Find the position where your repository was just before the hard reset.
- Recover the deleted commits back onto your branch.
- Verify that the full commit history has been restored.
- Save a screenshot showing the reflog output and the restored commit history in `output/name_rollnumber_task2/`.

### 7. Submit Task 2
- Ensure all required screenshots are saved in `output/name_rollnumber_task2/`.
- Commit your changes and push the `name_rollnumber_task2` branch to your fork.
- Open a Pull Request with the title `name_rollnumber_task2`.

---

## Task 3: Cherry-Pick and Rebase

Perform the following advanced operations on an isolated branch.

### Setup for Task 3
- Switch back to `main` and create a new branch named `name_rollnumber_task3`.
- Inside `output`, create a folder named `output/name_rollnumber_task3` to store your screenshots for this task.

### 1. Cherry-Pick
- Create a new branch called "Feature A" starting from your task branch (`name_rollnumber_task3`).
- Make 3 separate commits on "Feature A":
  - "Feature 1"
  - "Feature 2"
  - "Feature 3"
- Switch back to your task branch `name_rollnumber_task3`.
- Cherry-pick only the commit for "Feature 2" into your task branch using its commit identifier.
- Verify that "Feature 2" is now present in your task branch, while "Feature 1" and "Feature 3" are not.
- Display the history graph to confirm.
- Save a screenshot showing the cherry-picked commit in `output/name_rollnumber_task3/`.

### 2. Basic Rebase
- Create a new branch called "Feature B" starting from your task branch (`name_rollnumber_task3`).
- Make 3 separate commits on "Feature B":
  - "Rebase 1"
  - "Rebase 2"
  - "Rebase 3"
- Switch back to your task branch and make 2 new commits:
  - "Task 3 Update 1"
  - "Task 3 Update 2"
- Switch back to "Feature B".
- Rebase "Feature B" onto your task branch so that your branch changes sit cleanly on top.
- Display the history graph to confirm the linear history.
- Save a screenshot showing the linear rebase history in `output/name_rollnumber_task3/`.

### 3. Submit Task 3
- Ensure all required screenshots are saved in `output/name_rollnumber_task3/`.
- Commit your changes and push the `name_rollnumber_task3` branch to your fork.
- Open a Pull Request with the title `name_rollnumber_task3`.

---
<h2 align="center">All the best</h2>