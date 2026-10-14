# 1. Student Activity Guide: Team GitHub Pages Lab

In this activity, you will form a team of 5, set up a shared repository, configure GitHub Pages, create individual profile files, and practice Git commits, pulls, and pushes.

---

# Step-by-Step Instructions

## Phase 1: Team Setup & Repo Owner Instructions

1. **Form a Team:** Group up with 5 students sitting near you. Name your team.
2. **Assign a Team Lead (Repo Owner):** One team member creates the group repository.
3. **Repo Owner Actions:**
* Go to [GitHub.com](https://github.com) and click **New Repository**.
* Name the repository `cs211-your-team-name` (or similar) and set it to **Public**.
* Check **Add a README file** and click **Create repository**.

- Go to **Settings** > **Collaborators** > **Add people**, and invite the other 4 team members using their GitHub usernames.
 
4. **Team Members:** Check your email or GitHub notifications and accept the repository collaboration invite.

5. **Repo Owner Actions:**

Go to **Settings** > **Pages**:
* Under **Source**, select **Deploy from a branch**.
* Under **Branch**, select `main` and `/ (root)`, then click **Save**.
* Copy the published page URL once generated (e.g., `https://<owner-username>.github.io/cs211-your-team-name/`).


---

## Phase 2: Add Your Profile (Choose Option A or B)

---

### Option A: Using GitHub Desktop

1. **Clone the Repo:**
* Open **GitHub Desktop** > `File` > `Clone Repository...`.
* Find your team leader's repo under your repository list (or paste the repository URL) and click **Clone**.


2. **Create Your File:**
* In your code editor, create a new file named `<your-netid>.md` (e.g., `jsmith2.md`) inside the cloned folder.
* Fill out the template:

```markdown
# Profile: [Your Full Name]

- **NetID:** [Your NetID]
- **Major:** [Your Major]
- **Question that I chose from the memoization exercise:** [Type the Question as listed on the Website]
- **Link to the question article:** [Paste the URL to the question article]
- **My solution:**

\```

Paste your C code here. It should contain the comments you added when trying to solve.

\```



```




3. **Commit Locally:**
* Return to GitHub Desktop. Enter the summary `Add profile for <netid>` at the bottom left.
* Click **Commit to main**. *(This saves a local snapshot on your machine).*


4. **Pull Latest Changes:**
* Click **Fetch origin** / **Pull origin** at the top.
* *Why Pull?* Keeps your local folder updated with changes pushed by your teammates to avoid conflicts.


5. **Push Your Changes:**
* Click **Push origin** to upload your commit to GitHub.



---

### Option B: Using the Command Line (Terminal / Git Bash)

1. **Clone the Repo:**
```bash
git clone https://github.com/<owner-username>/<repo-name>.git
cd <repo-name>

```


2. **Create Your File:**
```bash
touch <your-netid>.md

```


Open the file in your text editor and paste:
```markdown
# Profile: [Your Full Name]

- **NetID:** [Your NetID]
- **Major:** [Your Major]
- **Favorite CS Topic:** [Topic]
- **Topic I Find Challenging / Want to Learn:** [Topic]

```


3. **Commit Locally:**
```bash
git add <your-netid>.md
git commit -m "Add profile for <your-netid>"

```


*(Creates a local snapshot on your machine).*
4. **Pull Latest Changes:**
```bash
git pull origin main

```


*(Integrates updates pushed by teammates before uploading yours).*
5. **Push Your Changes:**
```bash
git push origin main

```



---

## Phase 3: Link Profiles & Verify

1. **Update `README.md` (Team Lead or Any Member):**
* Edit `README.md` to list links to each member's Markdown file:

```markdown
# Team Member Profiles

- [Member 1 Profile](./netid1.md)
- [Member 2 Profile](./netid2.md)
- [Member 3 Profile](./netid3.md)
- [Member 4 Profile](./netid4.md)
- [Member 5 Profile](./netid5.md)

```


* Commit, pull, and push the updated `README.md`.


2. **Verify Live Site:** Visit the GitHub Pages link to ensure all team profile links work on the live site.

---

## Phase 4: Peer Review & Extensions

1. Open GitHub.com, navigate to a teammate's `.md` file, and leave feedback on formatting and completeness.
2. Enhance your Markdown file with an image, a formatted table, and a code block, then **Commit -> Pull -> Push** again.

---

### Resources

* [GitHub Desktop Download & Guide](https://desktop.github.com/)
* [Git Command Cheat Sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
* [Markdown Guide Syntax Cheat Sheet](https://www.markdownguide.org/basic-syntax/)

