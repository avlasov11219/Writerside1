# Set up Writerside in IntelliJ IDEA

[Writerside](https://www.jetbrains.com/writerside/) is a JetBrains plugin for authoring enterprise-ready documentation. It supports a hybrid format combining Markdown and semantic XML markup, and integrates directly into IntelliJ IDEA.

This guide walks you through the complete setup so that you can start writing and previewing documentation on your own machine. By the end, you will have:

- IntelliJ IDEA installed and running
- The Writerside plugin active in the IDE
- A new documentation project open and ready for authoring

## Before you begin

This guide uses the JetBrains Toolbox App to install IntelliJ IDEA. Both the Toolbox App and IntelliJ IDEA share the same operating system support, so the requirements below cover the full setup.

### Hardware

These are the minimum requirements for IntelliJ IDEA. The Toolbox App itself is lightweight and runs on any machine that meets them.

| Requirement | Minimum                                      |
|-------------|----------------------------------------------|
| CPU         | x86_64 or arm64, 4 cores                    |
| RAM         | 8 GB total; 3 GB available for IDE processes |
| Disk space  | 10 GB                                        |
| Display     | 1280 × 720                                   |

### Operating system

<tabs>
    <tab title="Windows">
        <p>Windows 10 (version 1809 or higher) or Windows 11.</p>
    </tab>
    <tab title="macOS">
        <p>macOS 15 or later.</p>
    </tab>
    <tab title="Linux">
        <p>Supported distributions:</p>
        <list>
            <li>Ubuntu 22.04 LTS or 24.04 LTS</li>
            <li>Fedora 42 or 43</li>
            <li>Amazon Linux 2023</li>
        </list>
        <p>Supported desktop environments: GNOME, KDE Plasma.</p>
        <p>The following system packages must be present for the Toolbox App to run:</p>
        <code-block lang="bash">
libxi6 libxrender1 libxtst6 mesa-utils libfontconfig libgtk-3-bin tar dbus-user-session
        </code-block>
        <p>Install any missing packages with:</p>
        <code-block lang="bash">
sudo apt install libxi6 libxrender1 libxtst6 mesa-utils libfontconfig libgtk-3-bin tar dbus-user-session
        </code-block>
    </tab>
</tabs>

<note>
BSD-based operating systems are not supported.
</note>

You do not need to install Java separately. IntelliJ IDEA bundles JetBrains Runtime (based on Java 21).

## Step 1: Install IntelliJ IDEA

The recommended way to install IntelliJ IDEA is through the JetBrains Toolbox App. It handles updates automatically and lets you manage multiple IDE versions side-by-side.

<procedure title="Install IntelliJ IDEA via the Toolbox App" id="install-toolbox">
    <step>
        <p>Go to the <a href="https://www.jetbrains.com/toolbox-app/">JetBrains Toolbox App page</a>, download the installer for your operating system, and run it.</p>
        <img src="toolbox-installer.png" alt="JetBrains Toolbox installer dialog" width="440" border-effect="line"/>
    </step>
    <step>
        <p>The Toolbox App opens a small welcome screen in the bottom-right corner of your desktop. Check <b>Agree to the JetBrains User Agreement</b> and click <b>Start</b>.</p>
        <img src="toolbox-welcome.png" alt="Toolbox App welcome screen" width="440" border-effect="line"/>
    </step>
    <step>
        <p>The Toolbox App main window opens and lists available JetBrains tools. Under <b>Available tools</b>, find <b>IntelliJ IDEA</b> and click <b>Install</b>.</p>
        <img src="toolbox-main.png" alt="Toolbox App main window showing available tools" width="440" border-effect="line"/>
    </step>
    <step>
        <p>The IDE downloads and installs automatically. You can monitor the progress in the <b>Installed</b> section.</p>
        <img src="intellij-downloading.png" alt="IntelliJ IDEA downloading in the Toolbox App" width="440" border-effect="line"/>
    </step>
    <step>
        <p>When the progress bar disappears and only the version number remains, the installation is complete. Click <b>IntelliJ IDEA</b> to launch it.</p>
        <img src="intellij-installed.png" alt="IntelliJ IDEA installed in the Toolbox App" width="440" border-effect="line"/>
    </step>
</procedure>

When you launch IntelliJ IDEA for the first time, the IDE guides you through initial setup: selecting a UI theme, configuring a keymap, and optionally signing in to your JetBrains account.

## Step 2: Install the Writerside plugin

Writerside is a free plugin available from the JetBrains Plugin Marketplace. You can install it from inside the IDE or directly from the Marketplace website.

<tabs>
    <tab title="From inside the IDE">
        <procedure title="Install Writerside from inside the IDE" id="install-plugin-ide">
            <step>
                <p>In IntelliJ IDEA, click the <b>Settings</b> gear icon in the top-right corner of the window and select <b>Plugins</b>.</p>
                <img src="ide-settings-menu.png" alt="Settings gear menu with Plugins highlighted" width="340" border-effect="line"/>
            </step>
            <step>
                <p>The <b>Plugins</b> dialog opens on the <b>Installed</b> tab. Switch to the <b>Marketplace</b> tab.</p>
                <img src="plugins-installed-tab.png" alt="Plugins dialog showing the Installed tab" width="700" border-effect="line"/>
            </step>
            <step>
                <p>In the search bar, type <em>writerside</em>. Select <b>Writerside</b> by JetBrains s.r.o. from the results and click <b>Install</b>.</p>
                <img src="plugins-marketplace-writerside.png" alt="Marketplace tab with Writerside search results" width="700" border-effect="line"/>
            </step>
            <step>
                <p>When installation completes, the button changes to <b>Restart IDE</b>. Click it, then confirm in the dialog that appears.</p>
                <img src="restart-ide-dialog.png" alt="Restart IDE confirmation dialog" width="440" border-effect="line"/>
            </step>
        </procedure>
    </tab>
    <tab title="From the Marketplace website">
        <procedure title="Install Writerside from the Marketplace website" id="install-plugin-browser">
            <step>
                <p>Open the <a href="https://plugins.jetbrains.com/plugin/20158-writerside/versions/stable">Writerside stable versions page</a> in your browser.</p>
                <img src="marketplace-website-versions.png" alt="Writerside versions page on the JetBrains Marketplace" width="700" border-effect="line"/>
            </step>
            <step>
                <p>Click <b>Install to IntelliJ IDEA 2026.1.1</b> (the button in the top-right corner). Your browser may ask for permission to open IntelliJ IDEA — allow it.</p>
                <tip>
                    The page also lists older versions that you can download as archives and install manually via <b>Settings | Plugins | ⚙ | Install Plugin from Disk</b>.
                </tip>
            </step>
            <step>
                <p>In IntelliJ IDEA, confirm the installation prompt, then click <b>Restart IDE</b> and confirm in the dialog.</p>
            </step>
        </procedure>
    </tab>
</tabs>

After the IDE restarts, the **Writerside** tool window icon appears in the left-side tool window bar.

## Step 3: Create a documentation project

<procedure title="Create a new documentation project" id="create-project">
    <step>
        <p>From the main menu, select <b>File | New | Project</b>.</p>
        <img src="new-project-menu.png" alt="File menu with New > Project highlighted" width="620" border-effect="line"/>
    </step>
    <step>
        <p>In the <b>New Project</b> wizard, select <b>Writerside</b> on the left. On the right, select <b>Starter Project</b> and click <b>Next</b>.</p>
        <img src="new-project-wizard-writerside.png" alt="New Project wizard with Writerside and Starter Project selected" width="700" border-effect="line"/>
        <tip>
            The wizard also offers <b>Playground</b> (multiple sample topics to explore markup features), <b>Import from MD</b> (migrate existing Markdown files), and <b>API Docs</b> (OpenAPI documentation template). For a blank starting point, use <b>Starter Project</b>.
        </tip>
    </step>
    <step>
        <p>Enter a <b>Project name</b> and confirm the <b>Project location</b>, then click <b>Create</b>.</p>
        <img src="new-project-name.png" alt="New Project dialog showing project name and location fields" width="700" border-effect="line"/>
    </step>
</procedure>

IntelliJ IDEA creates the project and opens the Writerside welcome topic. The left panel shows the **Help Instance** and the table of contents. Your project is ready for authoring.

<img src="project-starter-page.png" alt="Newly created Writerside project showing the Getting Started topic" width="700" border-effect="line"/>

### Project structure

The generated project has the following layout:

```
<your-project>/
└── Writerside/              ← help module (all documentation lives here)
    ├── cfg/
    │   └── buildprofiles.xml
    ├── topics/
    │   └── starter.md       ← your first topic
    ├── c.list               ← topic categories
    ├── hi.tree              ← table of contents
    ├── v.list               ← reusable variables
    └── writerside.cfg       ← module configuration
```

The `Writerside/` directory is the *help module*. The `topics/` subdirectory holds your content files. The `hi.tree` file controls the order and hierarchy of topics in the built output.

<note>
The <b>Writerside</b> directory name is the default module name. You can rename it to anything, such as <code>docs</code>, without affecting how the project builds.
</note>

## Step 4: Build and preview the documentation

Before committing your project to version control, run a build to confirm there are no errors, then preview the output.

### Build

<procedure title="Build the documentation" id="local-build">
    <step>
        <p>In the top toolbar, click the green <b>Run</b> triangle next to <b>Web Archive (hi)</b>, or press <shortcut>Shift+F10</shortcut>.</p>
        <img src="run-toolbar.png" alt="Top toolbar showing the Web Archive run configuration and Run button" width="500" border-effect="line"/>
    </step>
    <step>
        <p>The <b>Run</b> tool window opens at the bottom of the IDE and shows the build progress. A successful build ends with the message <em>'hi' built without problems.</em></p>
        <img src="build-output.png" alt="Run tool window showing a successful build with no problems" width="620" border-effect="line"/>
        <p>If the output contains errors, fix the flagged topics and run the build again before continuing.</p>
    </step>
</procedure>

<tip>
To check for errors without generating the full ZIP archive, enable dry run mode: press <shortcut>Ctrl+Shift+A</shortcut>, search for <b>Registry</b>, then find and enable the <code>wrs.dry.run</code> key.
</tip>

### Preview

<procedure title="Preview the documentation" id="preview-docs">
    <step>
        <p>After a successful build, a notification appears in the bottom-right corner of the IDE. Click <b>Got it</b> to open the <b>Writerside Preview</b> tool window, or open it manually from the right-side tool window bar.</p>
        <img src="writerside-preview-tooltip.png" alt="Notification prompting to open the Writerside Preview tool window" width="440" border-effect="line"/>
    </step>
    <step>
        <p>The <b>Writerside Preview</b> pane opens and renders the current topic with full formatting, images, and navigation.</p>
        <img src="writerside-preview-pane.png" alt="Writerside Preview pane showing the rendered documentation topic" width="600" border-effect="line"/>
    </step>
    <step>
        <p>To open the full built site in your browser — with working search, all pages, and complete styling — click <b>Open in Browser</b> in the top-right corner of the preview pane.</p>
    </step>
</procedure>

## Step 5: Push to GitHub

With a clean build confirmed, publish the project source to a public GitHub repository so others can access and contribute to the documentation.

<procedure title="Share the project on GitHub" id="push-github">
    <step>
        <p>In the left-side tool window bar (the narrow strip of icons at the very edge of the IDE), click the <b>Version Control</b> icon (or press <shortcut>Alt+9</shortcut>).</p>
        <img src="vcs-toolwindow-bar.png" alt="Version Control icon in the left tool window bar" width="200" border-effect="line"/>
        <p>The <b>Version Control</b> panel opens at the bottom of the IDE.</p>
        <img src="vcs-panel-options.png" alt="Version Control panel showing GitHub sharing options" width="440" border-effect="line"/>
    </step>
    <step>
        <p>Click <b>Share project on GitHub</b>. The sharing dialog opens.</p>
        <img src="github-share-dialog.png" alt="Share Project On GitHub dialog" width="500" border-effect="line"/>
        <p>In the dialog, do the following:</p>
        <list>
            <li>Set a <b>Repository name</b>.</li>
            <li>Uncheck <b>Private</b> if the assignment requires a public repository.</li>
            <li>Optionally add a <b>Description</b>.</li>
        </list>
    </step>
    <step>
        <p>If you are not yet signed in to GitHub, click <b>Add account</b> and choose a login method.</p>
        <img src="github-add-account.png" alt="Add account dropdown with login options" width="340" border-effect="line"/>
        <p>Available options:</p>
        <list>
            <li><b>Log In via GitHub</b> — opens your browser to authorize IntelliJ IDEA through GitHub's OAuth flow; no credentials are stored in the IDE.</li>
            <li><b>Log In with Token</b> — lets you paste a Personal Access Token generated in your GitHub account settings; useful when browser-based OAuth is blocked.</li>
            <li><b>Log In to GitHub Enterprise</b> — connects to a self-hosted GitHub Enterprise Server instance using your organization's URL.</li>
        </list>
    </step>
    <step>
        <p>Click <b>Share</b>. IntelliJ IDEA creates the remote repository, commits all project files, and pushes to <code>master</code>.</p>
    </step>
</procedure>

## What's next

With a clean local build confirmed, the next step is to push your project to a public GitHub repository and optionally set up a GitHub Actions workflow so that Writerside builds and publishes your documentation automatically on every push.

<seealso>
    <category ref="wrs">
        <a href="https://www.jetbrains.com/help/writerside/local-build.html">Build documentation locally</a>
        <a href="https://www.jetbrains.com/help/writerside/markup-reference.html">Markup reference</a>
        <a href="https://www.jetbrains.com/help/writerside/manage-table-of-contents.html">Manage the table of contents</a>
        <a href="https://www.jetbrains.com/help/writerside/deploy-docs-to-github-pages.html">Deploy to GitHub Pages</a>
    </category>
</seealso>
