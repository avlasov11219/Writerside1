# Install IntelliJ IDEA

Choose an installation method below. The Toolbox App is recommended for most users as it manages updates and multiple IDE versions automatically.

<note>
IntelliJ IDEA is available in two editions: <b>Community</b> (free, open source) and <b>Ultimate</b> (paid, with additional web and enterprise features). The free Community Edition is sufficient for Writerside.
</note>

<tabs>
    <tab title="Toolbox App (recommended)">
        <procedure title="Install IntelliJ IDEA via the Toolbox App" id="install-toolbox">
            <step>
                <p>Go to the <a href="https://www.jetbrains.com/toolbox-app/">JetBrains Toolbox App page</a>, download the installer for your operating system, and run it.</p>
                <img src="toolbox-installer.png" alt="JetBrains Toolbox installer dialog" border-effect="line"/>
            </step>
            <step>
                <p>The Toolbox App opens a small welcome screen in the bottom-right corner of your desktop. Check <b>Agree to the JetBrains User Agreement</b> and click <b>Start</b>.</p>
                <img src="toolbox-welcome.png" alt="Toolbox App welcome screen" border-effect="line"/>
            </step>
            <step>
                <p>The Toolbox App main window opens and lists available JetBrains tools. Under <b>Available tools</b>, find <b>IntelliJ IDEA</b> and click <b>Install</b>.</p>
                <img src="toolbox-main.png" alt="Toolbox App main window showing available tools" border-effect="line"/>
            </step>
            <step>
                <p>The IDE downloads and installs automatically. You can monitor the progress in the <b>Installed</b> section.</p>
                <img src="intellij-downloading.png" alt="IntelliJ IDEA downloading in the Toolbox App" border-effect="line"/>
            </step>
            <step>
                <p>When the progress bar disappears and only the version number remains, the installation is complete. Click <b>IntelliJ IDEA</b> to launch it.</p>
                <img src="intellij-installed.png" alt="IntelliJ IDEA installed in the Toolbox App" border-effect="line"/>
            </step>
        </procedure>
    </tab>
    <tab title="Standalone installer">
        <procedure title="Install the standalone package" id="install-standalone">
            <step>
                <p>Go to the <a href="https://www.jetbrains.com/idea/download/">IntelliJ IDEA download page</a>. Under <b>Community Edition</b>, click <b>Download</b> for your operating system.</p>
                <tip>
                    The page shows two editions: <b>Ultimate</b> (paid) and <b>Community</b> (free). The free Community Edition is sufficient for Writerside.
                    On macOS, choose the correct download for your processor — <b>Apple Silicon</b> (.dmg) for M-series Macs, or <b>Intel</b> (.dmg) for older Intel Macs.
                </tip>
            </step>
            <step>
                <p>Install IntelliJ IDEA for your operating system:</p>
                <tabs>
                    <tab title="Windows">
                        <p>Run the downloaded <code>.exe</code> installer. The setup wizard opens — follow the prompts to complete the installation.</p>
                        <img src="standalone-installer-wizard.png" alt="IntelliJ IDEA setup wizard on Windows" border-effect="line"/>
                    </tab>
                    <tab title="macOS">
                        <p>Open the downloaded <code>.dmg</code> file. Drag the <b>IntelliJ IDEA</b> application icon into the <b>Applications</b> folder, then eject the disk image.</p>
                    </tab>
                </tabs>
            </step>
            <step>
                <p>Launch IntelliJ IDEA from the desktop shortcut (Windows) or from the Applications folder (macOS).</p>
            </step>
        </procedure>
    </tab>
</tabs>

When you launch IntelliJ IDEA for the first time, the IDE guides you through initial setup: selecting a UI theme, configuring a keymap, and optionally signing in to your JetBrains account.

With IntelliJ IDEA running, continue to [Install the Writerside plugin](install-writerside-plugin.md).
