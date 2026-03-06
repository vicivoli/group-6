# J220 Group Project - Github Branches

In this assignment, your group will collaboratively build a website using GitHub branching system with pull requests. This assignment simulates a real-world collaborative Git workflow.

Groups will be assigned in bCourses as well as a video tutorial of all steps in this process. It's important you watch it fully first and follow each step exactly. This process is much easier if you arrange a time on Zoom to do this together. 


## First Step: Assign Group Members

There are six people in a group. Assign each person to a letter (Person A, Person B, Person C, and so forth...) **Person A** will be the point person and have a special role. They will be the one to accept each group member's pull request into the main repository. They will also be the one to submit the final website to bCourses at the end.


## Person A (Point Person) Starts Before Anyone Else

### 1. Person A Creates the Group Repository

1. On this template repository. Click the green **"Use this template"**
2. Create a new **public** repository under Person A's own GitHub account.
3. Make sure it is **Public**.
4. Name it `group-1` (depending on your group number)

### 2. Enable GitHub Pages

1. On the repository page, go to **Settings → Pages**
2. Under **Source**, choose:
   - Branch: `main`
   - Folder: `/ (root)`
3. Click **Save**

Your site will be available at: https://your-username.github.io/repository-name/

## Next, Other Group Members (Everyone Except Person A)

## Step 1: Fork Person A's Repository

1. Go to Person A’s `group-1` repository they just created on GitHub (**NOT** the instructor's)
2. Click **Fork** (top right).
3. Create the fork under your own account. Make it public
4. Name the fork `group-1-your-name` replacing the group number with your group number, and your name with your own name.
5. Once you have a copy of the repository, click the green "Code" button and copy the HTTPS URL to your clipboard.

## Step 2: Clone Your Fork in VS Code

1. Open **VS Code**
2. Create a new window
3. Click the link to **Clone Git Repository**
4. Paste in the URL you copied from the fork you created on Github.com
5. Clone to your computer, saving it in a folder in J220 Coding Projects.
6. **Important:** Don't start coding or changing anything yet until the next step.

## Step 3: Create a Branch

1. Look at the bottom-left corner of VS Code.
2. Click the branch name (`main`).
3. Select **Create New Branch**
4. Name your branch: `your-first-name` (using of course, your own name)

## Step 4: Edit Your Page

Avoic renaming folders.  You should work with your group to have been assigned a letter.

Your folder structure looks like:

```
group-member-pages/
  person-a/index.html
  person-b/index.html
  person-c/index.html
```

Find the folder assigned to you and open:

`group-member-pages/person-x/index.html`

Edit only that file.

Follow the instructions inside the file to add your name, add content and customize your page. 

Do NOT:
- Rename folders
- Edit other students' folders
- Edit other parts of the repository

## Step 5: Commit Your Changes

1. Click the **Source Control** icon (left sidebar).
2. Review the changed files.
3. In the message box, write `Updated your-name (person-X) page`
4. Click **Commit** (checkmark icon).

## Step 6: Push Your Branch to Github.com

After committing:

1. Click **Publish Branch** OR **Sync Changes** (depending on if this is yoru first time publishing or you've made several changes)

Your branch is now on GitHub.

## Step 7: Create a Pull Request (On GitHub Website)

1. Go to your own forked repository on GitHub.com.
2. You should see a banner:
   > “Compare & pull request”

   Click it.
3. Confirm:
   - Base repository: Person A’s repository
   - Base branch: `main`
   - Compare branch: `your-name`

4. Click **Create Pull Request**

Done.

## Back to Person A — Merging Pull Requests

1. Open the Pull Request (refresh your browser and click on "Pull Requests" tab)
2. Review changes.
3. Click **Merge Pull Request**
4. Confirm merge. The site will automatically update on GitHub Pages.

Person A can also clone the repository to their own computer and make edits to the front page. Make sure you are clicking sync to bring in merges. 

## Optional for other students: Syncing Your Fork (Advanced)

You do NOT need to do this for the assignment. However, if you want your fork to stay updated with your group’s merged work, meaning you see other student pages on your repository, including the front page from Person A, you will need to add an "Upstream" remote so that you can sync the original repository from Person A. 

### Add Upstream (One Time)

Go to the original Person A repository (NOT on your own account. This is Person A's version on their account. Copy the URL.)

In VSCode:

1. Open Command Palette
2. Type: Git: Add Remote
3. Remote URL: (paste in Person A's repository URL)
4. Remote name: `upstream`
5. Switch to `main` branch on botton left.
6. Fetch: Source Control, click the three dots `...`, click **Fetch**
7. Pull from upstream
8. Push to origin

This updates your fork with the latest merged changes. Again, this step is optional.


