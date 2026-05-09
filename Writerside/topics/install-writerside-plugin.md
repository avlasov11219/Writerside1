# Install the Writerside plugin

Writerside is a free plugin available from the JetBrains Plugin Marketplace. Install the latest stable version — no specific version is required.

You can install it from inside the IDE or from the Marketplace website.

<tabs>
    <tab title="From inside the IDE">
        <procedure title="Install Writerside from inside the IDE" id="install-plugin-ide">
            <step>
                <p>In IntelliJ IDEA, click the <b>Settings</b> gear icon in the top-right corner of the window and select <b>Plugins</b>.</p>
                <img src="ide-settings-menu.png" alt="Settings gear menu with Plugins highlighted" border-effect="line"/>
            </step>
            <step>
                <p>The <b>Plugins</b> dialog opens on the <b>Installed</b> tab. Switch to the <b>Marketplace</b> tab.</p>
                <img src="plugins-installed-tab.png" alt="Plugins dialog showing the Installed tab" border-effect="line"/>
            </step>
            <step>
                <p>In the search bar, type <em>writerside</em>. Select <b>Writerside</b> by JetBrains s.r.o. from the results and click <b>Install</b>.</p>
                <img src="plugins-marketplace-writerside.png" alt="Marketplace tab with Writerside search results" border-effect="line"/>
            </step>
            <step>
                <p>When installation completes, the button changes to <b>Restart IDE</b>. Click it, then confirm in the dialog that appears.</p>
                <img src="restart-ide-dialog.png" alt="Restart IDE confirmation dialog" border-effect="line"/>
            </step>
        </procedure>
    </tab>
    <tab title="From the Marketplace website">
        <procedure title="Install Writerside from the Marketplace website" id="install-plugin-browser">
            <step>
                <p>Open the <a href="https://plugins.jetbrains.com/plugin/20158-writerside">Writerside plugin page</a> in your browser.</p>
                <img src="marketplace-website-versions.png" alt="Writerside page on the JetBrains Marketplace" border-effect="line"/>
                <note>
                    The button in the top-right corner changes depending on whether IntelliJ IDEA is installed:
                    <list>
                        <li>If IntelliJ IDEA is <b>not yet installed</b>, the button reads <b>Get</b> and takes you to the IntelliJ IDEA download page. Install the IDE first, then return here.</li>
                        <li>If IntelliJ IDEA <b>is installed</b>, the button reads <b>Install to IntelliJ IDEA</b> and installs the plugin directly.</li>
                    </list>
                </note>
            </step>
            <step>
                <p>Click the <b>Install to IntelliJ IDEA</b> button. Your browser may ask for permission to open IntelliJ IDEA — allow it.</p>
                <tip>
                    The <b>Versions</b> tab lists older releases you can download as archives and install manually via <b>Settings | Plugins</b>, then click the gear icon and select <b>Install Plugin from Disk</b>. For a new setup, always use the latest version shown on the main page.
                </tip>
            </step>
            <step>
                <p>In IntelliJ IDEA, confirm the installation prompt, then click <b>Restart IDE</b> and confirm in the dialog.</p>
            </step>
        </procedure>
    </tab>
</tabs>

After the IDE restarts, the **Writerside** tool window icon appears in the left-side tool window bar.

With the plugin active, continue to [Create a documentation project](create-project.md).
