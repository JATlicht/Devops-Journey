---


---

<h3 id="basic-commands">Basic Commands</h3>
<h4 id="git-init"><code>git init</code></h4>
<p>Initializes a new Git repository in the current directory.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> init
</code></pre>
<h4 id="git-clone"><code>git clone</code></h4>
<p>Creates a local copy of a remote repository.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> clone <span class="token operator">&lt;</span>repository-url<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-add"><code>git add</code></h4>
<p>Stages changes in the working directory for the next commit.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> add <span class="token operator">&lt;</span>file<span class="token operator">&gt;</span>
<span class="token function">git</span> add <span class="token keyword">.</span>
</code></pre>
<h4 id="git-commit"><code>git commit</code></h4>
<p>Saves staged changes to the local repository with a descriptive message.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> commit -m <span class="token string">"commit message"</span>
</code></pre>
<h4 id="git-status"><code>git status</code></h4>
<p>Displays the state of the working directory and staging area.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> status
</code></pre>
<h4 id="git-log"><code>git log</code></h4>
<p>Shows the commit history of the repository.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> log
</code></pre>
<h3 id="branching-and-merging">Branching and Merging</h3>
<h4 id="git-branch"><code>git branch</code></h4>
<p>Lists, creates, or deletes branches.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> branch
<span class="token function">git</span> branch <span class="token operator">&lt;</span>branch-name<span class="token operator">&gt;</span>
<span class="token function">git</span> branch -d <span class="token operator">&lt;</span>branch-name<span class="token operator">&gt;</span> <span class="token comment"># delete from local repo</span>
<span class="token function">git</span> push origin --delete <span class="token operator">&lt;</span>branch-name<span class="token operator">&gt;</span> <span class="token comment"># delete from remote(github)</span>
</code></pre>
<h4 id="git-checkout"><code>git checkout</code></h4>
<p>Switches between branches or restores working directory files.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> checkout <span class="token operator">&lt;</span>branch-name<span class="token operator">&gt;</span>
<span class="token function">git</span> checkout -- <span class="token operator">&lt;</span>file<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-merge"><code>git merge</code></h4>
<p>Combines changes from one branch into another.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> merge <span class="token operator">&lt;</span>branch-name<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-rebase"><code>git rebase</code></h4>
<p>Applies commits from the current branch on top of another branch.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> rebase <span class="token operator">&lt;</span>branch-name<span class="token operator">&gt;</span>
</code></pre>
<h3 id="remote-repositories">Remote Repositories</h3>
<h4 id="git-remote"><code>git remote</code></h4>
<p>Manages set of tracked repositories.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> remote -v
<span class="token function">git</span> remote add <span class="token operator">&lt;</span>name<span class="token operator">&gt;</span> <span class="token operator">&lt;</span>url<span class="token operator">&gt;</span>
<span class="token function">git</span> remote remove <span class="token operator">&lt;</span>name<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-fetch"><code>git fetch</code></h4>
<p>Downloads objects and refs from another repository.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> fetch <span class="token operator">&lt;</span>remote<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-pull"><code>git pull</code></h4>
<p>Fetches from and integrates with another repository or a local branch.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> pull <span class="token operator">&lt;</span>remote<span class="token operator">&gt;</span> <span class="token operator">&lt;</span>branch<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-push"><code>git push</code></h4>
<p>Updates remote refs along with associated objects.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> push <span class="token operator">&lt;</span>remote<span class="token operator">&gt;</span> <span class="token operator">&lt;</span>branch<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-remote-show"><code>git remote show</code></h4>
<p>Displays detailed information about a remote repository.</p>
<h3 id="inspecting-and-comparing">Inspecting and Comparing</h3>
<h4 id="git-diff"><code>git diff</code></h4>
<p>Shows changes between commits, commit and working tree, etc.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> <span class="token function">diff</span>
<span class="token function">git</span> <span class="token function">diff</span> <span class="token operator">&lt;</span>commit1<span class="token operator">&gt;</span> <span class="token operator">&lt;</span>commit2<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-show"><code>git show</code></h4>
<p>Displays various types of objects (commits, tags, trees, blobs).</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> show <span class="token operator">&lt;</span>commit<span class="token operator">&gt;</span>
</code></pre>
<h3 id="undoing-changes">Undoing Changes</h3>
<h4 id="git-reset"><code>git reset</code></h4>
<p>Resets current HEAD to the specified state.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> reset --hard <span class="token operator">&lt;</span>commit <span class="token function">id</span> <span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-revert"><code>git revert</code></h4>
<p>Creates a new commit that undoes the changes made by a previous commit.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> revert <span class="token operator">&lt;</span>commit id<span class="token operator">&gt;</span>
</code></pre>
<h4 id="git-clean"><code>git clean</code></h4>
<p>Removes untracked files from the working directory.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> clean -f
</code></pre>
<h3 id="stashing">Stashing</h3>
<h4 id="git-stash"><code>git stash</code></h4>
<p>Temporarily saves changes in a dirty working directory.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> stash
</code></pre>
<h4 id="git-stash-apply"><code>git stash apply</code></h4>
<p>Applies previously stashed changes.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> stash apply
</code></pre>
<h3 id="tagging">Tagging</h3>
<h4 id="git-tag"><code>git tag</code></h4>
<p>Creates, lists, deletes, or verifies a tag object signed with GPG.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> tag
<span class="token function">git</span> tag <span class="token operator">&lt;</span>tag-name<span class="token operator">&gt;</span>
<span class="token function">git</span> tag -d <span class="token operator">&lt;</span>tag-name<span class="token operator">&gt;</span>
</code></pre>
<h3 id="configuration">Configuration</h3>
<h4 id="git-config"><code>git config</code></h4>
<p>Gets and sets repository or global options.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> config --global user.name <span class="token string">"Your Name"</span>
<span class="token function">git</span> config --global user.email <span class="token string">"you@example.com"</span>
</code></pre>

