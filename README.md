# Demo-for-project

# 1. Rushikesh Bhavar
# 2. Ganesh Sakhare
# 3. Vinit Dhondapati
# 4. Abhijit Kumbhar



```
Exported with AIPRM https://www.aiprm.com by rushikeshbhawar12@gmail.com on 30/05/2023, 21:46:49
```

---


**User:**
how to push chnages to forked repo from local and then rais a pr to merget to repo from where it has been forked

---

**ChatGPT:**
To push changes to a forked repository from your local machine and then raise a pull request to merge those changes into the original repository, you can follow these steps:
<li><p>Clone the Forked Repository:</p><ul><li>Open a terminal or command prompt on your local machine.</li><li>Use the <code>git clone</code> command to clone the forked repository to your local machine.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>bash</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-bash">git <span class="hljs-built_in">clone</span> &lt;forked-repository-url&gt;
</code></div></div></pre></li><li>Replace <code>&lt;forked-repository-url&gt;</code> with the actual URL of the forked repository. You can find this URL on the repository's page on GitHub.</li></ul></li><li><p>Configure Upstream Remote:</p><ul><li>Change into the cloned repository's directory.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>bash</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-bash"><span class="hljs-built_in">cd</span> &lt;forked-repository-name&gt;
</code></div></div></pre></li><li>Add the original repository as the upstream remote.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>csharp</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-csharp">git remote <span class="hljs-keyword">add</span> upstream &lt;original-repository-url&gt;
</code></div></div></pre></li><li>Replace <code>&lt;original-repository-url&gt;</code> with the actual URL of the original repository. This URL can also be found on the repository's page on GitHub.</li></ul></li><li><p>Fetch the Latest Changes:</p><ul><li>Fetch the latest changes from both the origin (forked repository) and upstream (original repository) remotes.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>sql</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-sql">git <span class="hljs-keyword">fetch</span> origin
git <span class="hljs-keyword">fetch</span> upstream
</code></div></div></pre></li></ul></li><li><p>Create a New Branch:</p><ul><li>Create a new branch to work on your changes.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>css</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-css">git checkout -<span class="hljs-selector-tag">b</span> &lt;branch-name&gt;
</code></div></div></pre></li><li>Replace <code>&lt;branch-name&gt;</code> with a descriptive name for your branch.</li></ul></li><li><p>Make and Commit Your Changes:</p><ul><li>Make the necessary changes to the files in your local repository using your preferred editor or IDE.</li><li>Stage the changes you want to commit.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>php</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-php-template"><span class="xml">git add <span class="hljs-tag">&lt;<span class="hljs-name">file1</span>&gt;</span> <span class="hljs-tag">&lt;<span class="hljs-name">file2</span>&gt;</span> ...
</span></code></div></div></pre></li><li>Replace <code>&lt;file1&gt; &lt;file2&gt; ...</code> with the names of the specific files you want to stage, or use <code>.</code> to stage all changes.</li><li>Commit the changes.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>sql</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-sql">git <span class="hljs-keyword">commit</span> <span class="hljs-operator">-</span>m "Descriptive commit message"
</code></div></div></pre></li></ul></li><li><p>Push Changes to Forked Repository:</p><ul><li>Push your branch with the changes to the forked repository.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>perl</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-perl">git <span class="hljs-keyword">push</span> origin &lt;branch-name&gt;
</code></div></div></pre></li></ul></li><li><p>Raise a Pull Request:</p><ul><li>Go to the forked repository on GitHub in your web browser.</li><li>You should see a message prompting you to compare and pull request. Click on it.</li><li>Review the changes you made and provide a descriptive title and comment for your pull request.</li><li>Click on "Create pull request" to raise the pull request.</li></ul></li>
Once you've raised the pull request, the maintainers of the original repository can review your changes and choose to merge them into the main repository.

---

**User:**
how can we restrict to no to clone the main branch of the repo

---

**ChatGPT:**
If you want to restrict users from cloning the main branch of a repository, you can use Git branch protection settings on platforms like GitHub. Here's how you can do it:
<li>Navigate to the repository on GitHub.</li><li>Click on the "Settings" tab.</li><li>In the left sidebar, click on "Branches".</li><li>Under the "Branch protection rules" section, click on "Add rule".</li><li>In the "Branch name pattern" field, enter the branch name of the main branch (e.g., <code>main</code> or <code>master</code>).</li><li>Check the box for "Require pull request reviews before merging".<ul><li>This ensures that any changes to the main branch must go through a pull request and receive the necessary reviews before being merged.</li></ul></li><li>Optionally, you can enable other restrictions like requiring status checks, requiring signed commits, or enabling branch administrators.</li><li>Click on "Create" to save the branch protection rule.</li>
With this setup, users will not be able to clone the main branch directly. They will need to create a new branch, make their changes there, and then submit a pull request to merge those changes into the main branch. This helps enforce a workflow that encourages collaboration and code review before changes are merged into the main branch.

---

**User:**
git pull from upstream branch

---

**ChatGPT:**
To pull changes from an upstream branch in Git, you can follow these steps:
<li><p>Verify Remote Configuration:</p><ul><li>Ensure that you have added the upstream remote to your local repository. You can check your remote configuration using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs">git remote -v
</code></div></div></pre></li><li>It should display the upstream remote URL along with other remotes like origin.</li></ul></li><li><p>Fetch Upstream Changes:</p><ul><li>Fetch the latest changes from the upstream remote using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>sql</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-sql">git <span class="hljs-keyword">fetch</span> upstream
</code></div></div></pre></li><li>This command fetches the latest changes from the upstream repository without merging them into your local branch.</li></ul></li><li><p>Switch to Your Branch:</p><ul><li>If you're not already on your branch, switch to it using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>php</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-php-template"><span class="xml">git checkout <span class="hljs-tag">&lt;<span class="hljs-name">your-branch</span>&gt;</span>
</span></code></div></div></pre></li><li>Replace <code>&lt;your-branch&gt;</code> with the name of your branch.</li></ul></li><li><p>Merge Upstream Changes:</p><ul><li>After fetching the upstream changes, you can merge them into your local branch using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>php</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-php-template"><span class="xml">git merge upstream/<span class="hljs-tag">&lt;<span class="hljs-name">upstream-branch</span>&gt;</span>
</span></code></div></div></pre></li><li>Replace <code>&lt;upstream-branch&gt;</code> with the name of the upstream branch you want to merge.</li><li>This command will incorporate the changes from the upstream branch into your local branch.</li></ul></li><li><p>Resolve Conflicts (if any):</p><ul><li>If there are any conflicts between your local changes and the upstream changes, Git will notify you during the merge process.</li><li>Open the conflicting files and resolve the conflicts manually by editing the files to contain the desired changes.</li><li>After resolving the conflicts, stage the changes using <code>git add &lt;file&gt;</code> for each conflicted file.</li></ul></li><li><p>Commit the Merge:</p><ul><li>Once all conflicts are resolved, commit the merge using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>sql</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-sql">git <span class="hljs-keyword">commit</span> <span class="hljs-operator">-</span>m "Merge upstream/&lt;upstream-branch&gt;"
</code></div></div></pre></li><li>Add an appropriate commit message to describe the merge.</li></ul></li>
Now you have successfully pulled the latest changes from the upstream branch into your local branch. Remember to push your changes to your forked repository if you want to contribute them back to the upstream repository.

---

**User:**
how to push from my main to upstream dev branch of forked repo

---

**ChatGPT:**
To push changes from your local main branch to the upstream dev branch of a forked repository, you can follow these steps:
<li><p>Verify Remote Configuration:</p><ul><li>Ensure that you have added the upstream remote to your local repository. You can check your remote configuration using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs">git remote -v
</code></div></div></pre></li><li>It should display the upstream remote URL along with other remotes like origin.</li></ul></li><li><p>Switch to the Main Branch:</p><ul><li>If you're not already on the main branch, switch to it using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>css</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-css">git checkout <span class="hljs-selector-tag">main</span>
</code></div></div></pre></li><li>This command switches your current branch to the main branch.</li></ul></li><li><p>Pull the Latest Changes:</p><ul><li>Before pushing your changes, it's recommended to pull the latest changes from the upstream dev branch to ensure you have the most up-to-date code.<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs">git pull upstream dev
</code></div></div></pre></li><li>This command fetches and merges the latest changes from the upstream dev branch into your local main branch.</li></ul></li><li><p>Push Changes to Upstream:</p><ul><li>Once you have the latest changes and are on the main branch, you can push your changes to the upstream dev branch using the following command:<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>css</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-css">git push upstream <span class="hljs-selector-tag">main</span>:dev
</code></div></div></pre></li><li>This command pushes the commits from your local main branch to the upstream dev branch of the forked repository.</li></ul></li>
After pushing your changes, the upstream dev branch of the forked repository will be updated with your latest code. You can then raise a pull request from the dev branch to propose merging your changes into the original repository.