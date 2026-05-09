# Push to GitHub

With a clean build confirmed, publish the project source to a public GitHub repository so others can access and contribute to the documentation.

<note>
New Writerside projects do not include a Git repository by default. The <b>Share Project on GitHub</b> action initializes a local Git repository, creates the remote repository on GitHub, and pushes — all in one step.
</note>

<procedure title="Share the project on GitHub" id="push-github">
    <step>
        <p>In the left-side tool window bar (the narrow strip of icons at the very edge of the IDE), click the <b>Version Control</b> icon (or press <shortcut>Alt+9</shortcut>).</p>
        <img src="vcs-toolwindow-bar.png" alt="Version Control icon in the left tool window bar" border-effect="line"/>
        <p>The <b>Version Control</b> panel opens at the bottom of the IDE.</p>
        <img src="vcs-panel-options.png" alt="Version Control panel showing GitHub sharing options" border-effect="line"/>
    </step>
    <step>
        <p>Click <b>Share project on GitHub</b>. The sharing dialog opens.</p>
        <img src="github-share-dialog.png" alt="Share Project On GitHub dialog" border-effect="line"/>
        <p>In the dialog, do the following:</p>
        <list>
            <li>Set a <b>Repository name</b>.</li>
            <li>Uncheck <b>Private</b> if the assignment requires a public repository.</li>
            <li>Optionally add a <b>Description</b>.</li>
        </list>
    </step>
    <step>
        <p>If you are not yet signed in to GitHub, click <b>Add account</b> and choose a login method.</p>
        <img src="github-add-account.png" alt="Add account dropdown with login options" border-effect="line"/>
        <p>Available options:</p>
        <list>
            <li><b>Log In via GitHub</b> — opens your browser to authorize IntelliJ IDEA through GitHub's OAuth flow; no credentials are stored in the IDE.</li>
            <li><b>Log In with Token</b> — lets you paste a Personal Access Token generated in your GitHub account settings; useful when browser-based OAuth is blocked.</li>
            <li><b>Log In to GitHub Enterprise</b> — connects to a self-hosted GitHub Enterprise Server instance using your organization's URL.</li>
        </list>
    </step>
    <step>
        <p>Click <b>Share</b>. IntelliJ IDEA creates the remote repository, commits all project files, and pushes to the default branch.</p>
    </step>
</procedure>

Your project is now live on GitHub. From here you can invite collaborators, set up continuous integration, or configure [automatic deployment to GitHub Pages](https://www.jetbrains.com/help/writerside/deploy-docs-to-github-pages.html) so every push publishes a new version of your documentation site automatically.
