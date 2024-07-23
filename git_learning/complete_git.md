# Git

## 1.  Basic Concepts
    
  #### What is version control?

**Version Control** is a system that records changes to a file or set of files over time so that you can recall specific versions later. It allows multiple people to collaborate on a project, track and manage changes, and revert to previous versions if necessary.

**Key benefits of version control include:**

-   **Collaboration:** Multiple team members can work on the same project simultaneously without overwriting each other's changes.
-   **Tracking History:** Keeps a history of all changes made to a file or set of files, including who made the changes and when.
-   **Branching and Merging:** Allows the creation of separate branches for different features or releases, which can be merged back into the main branch once they're complete.
-   **Backup:** Acts as a backup by storing versions of the project, so you can restore previous versions if something goes wrong.

#### Difference between Git and other VCS

**Git vs. Other Version Control Systems (VCS)**

1.  **Centralized vs. Distributed:**
    
    -   **Centralized VCS (CVCS):** Systems like Subversion (SVN) and Perforce rely on a single central repository that all users interact with. Users check out files, make changes, and then commit them back to the central repository.
    -   **Distributed VCS (DVCS):** Systems like Git and Mercurial allow each user to have their own complete copy of the repository, including the entire history. Users can work offline and commit changes locally, then push or pull changes to and from a shared repository when needed.
2.  **Speed and Performance:**
    
    -   **Git:** Since every user has a full copy of the repository, many operations (like commits, diffs, and history viewing) are performed locally and are therefore very fast.
    -   **CVCS:** Operations that require communication with the central server can be slower, especially with large projects or slow network connections.
3.  **Branching and Merging:**
    
    -   **Git:** Branching is a core feature and is very lightweight and fast. Merging branches is a common workflow and is well-supported.
    -   **CVCS:** Branching can be more complex and resource-intensive, and merging changes from different branches can sometimes be more challenging.
4.  **Data Integrity:**
    
    -   **Git:** Every file and commit is checksummed using SHA-1 hashing, ensuring the integrity of the repository. If any data is corrupted or altered, Git can detect it.
    -   **CVCS:** Data integrity is generally maintained, but the methods can vary, and some systems may not be as robust as Git's checksumming.
5.  **Usage and Popularity:**
    
    -   **Git:** Widely used in open-source projects and many organizations due to its flexibility, performance, and branching capabilities.
    -   **CVCS:** Still used in many enterprise environments, particularly in legacy systems or where centralized control is preferred.

#### Repositories (Local and Remote)

**Repositories** are the storage locations where the project files and their histories are kept.

1.  **Local Repository:**
    
    -   This is the repository on your local machine. When you clone a remote repository, a copy of it is stored locally on your machine. You can commit changes to your local repository independently of others.
    -   The local repository consists of three areas:
        -   **Working Directory:** Where you make changes to your files.
        -   **Staging Area (Index):** Where you place files that you want to include in the next commit.
        -   **Repository (HEAD):** The committed files and history of changes.
2.  **Remote Repository:**
    
    -   This is the repository hosted on a server or cloud service, accessible by multiple users over a network. Remote repositories are used for collaboration, allowing team members to share changes.
    -   Commonly used remote repository hosting services include GitHub, GitLab, Bitbucket, and Azure Repos.
    -   You interact with remote repositories using commands like `git push`, `git pull`, and `git fetch`.

**Key Commands:**

-   **Cloning a repository:** `git clone <repository-url>`
-   **Adding changes to the staging area:** `git add <file>`
-   **Committing changes:** `git commit -m "commit message"`
-   **Pushing changes to a remote repository:** `git push <remote> <branch>`
-   **Pulling changes from a remote repository:** `git pull <remote> <branch>`


# Reference 
[video](https://www.youtube.com/watch?v=AT1uxOLsCdk)

2.  **Basic Commands**
    
    -   `git init`, `git clone`
    -   `git add`, `git commit`
    -   `git status`, `git log`
    -   `git branch`, `git checkout`
    -   `git merge`, `git rebase`
3.  **Advanced Commands**
    
    -   `git stash`
    -   `git cherry-pick`
    -   `git revert`, `git reset`
    -   `git diff`
    -   `git fetch`, `git pull`, `git push`
4.  **Branching and Merging**
    
    -   Branching strategies
    -   Handling merge conflicts
5.  **Tagging and Releases**
    
    -   Creating and managing tags
6.  **Working with Remotes**
    
    -   Adding and removing remotes
    -   Fetching and pulling from remotes
    -   Pushing to remotes
7.  **Git Configuration**
    
    -   `.gitignore` file
    -   Git hooks
    -   Configuring Git settings

### GitHub

1.  **Introduction to GitHub**
    
    -   Creating a GitHub account
    -   Understanding the GitHub interface
2.  **Repositories**
    
    -   Creating and managing repositories
    -   Forking repositories
    -   Collaborating on repositories
3.  **Issues and Projects**
    
    -   Creating and managing issues
    -   Using project boards
4.  **Pull Requests**
    
    -   Creating and managing pull requests
    -   Code review process
5.  **GitHub Actions**
    
    -   Setting up CI/CD pipelines
6.  **GitHub Pages**
    
    -   Hosting static sites with GitHub Pages
7.  **Security**
    
    -   Managing access permissions
    -   Setting up branch protection rules

### GitLab

1.  **Introduction to GitLab**
    
    -   Creating a GitLab account
    -   Navigating the GitLab interface
2.  **Repositories**
    
    -   Creating and managing repositories
    -   Forking and cloning repositories
3.  **Issues and Boards**
    
    -   Creating and managing issues
    -   Using issue boards
4.  **Merge Requests**
    
    -   Creating and managing merge requests
    -   Conducting code reviews
5.  **GitLab CI/CD**
    
    -   Setting up and configuring GitLab CI/CD
    -   Writing `.gitlab-ci.yml` files
6.  **GitLab Runners**
    
    -   Setting up and managing runners
7.  **Security and Permissions**
    
    -   Managing user permissions
    -   Setting up project and group permissions
8.  **GitLab Pages**
    
    -   Hosting static sites with GitLab Pages

### Additional Topics

1.  **Best Practices**
    
    -   Commit message conventions
    -   Branch naming conventions
    -   Versioning strategies
2.  **Integration with Other Tools**
    
    -   Integrating with IDEs
    -   Using Git with continuous integration tools
    -   Managing dependencies
