# Build and preview the documentation

At any point while writing, you can preview your work in the IDE or generate a full build to verify the complete output — without committing anything.

Writerside gives you two ways to review your work:

- **Live preview** — the Writerside Preview pane updates as you type, with no build required. Use this for everyday writing.
- **Full build** — generates a complete website archive. Use this to verify cross-page navigation, search, and custom styling.

## Live preview

The Writerside Preview tool window opens automatically the first time you open a topic. If you close it, reopen it in any of these ways:

- Click the **Writerside Preview** button in the right-side tool window bar.
- From the main menu, select **View | Tool Windows | Writerside Preview**.
- Right-click any topic in the table of contents and select **Preview Topic**.

<img src="writerside-preview-pane.png" alt="Writerside Preview pane showing the rendered documentation topic" border-effect="line"/>

The pane renders the active topic in real time and scrolls in sync with your cursor position in the editor.

## Build

The first time you build, you need to create a run configuration from the Writerside tool window. Subsequent builds can be triggered from the toolbar.

<procedure title="Run the first build" id="local-build">
    <step>
        <p>In the <b>Writerside</b> tool window, select your help instance. Click <b>Export To</b>, then select <b>Web Archive</b>.</p>
        <p>Writerside creates a run configuration and starts the build immediately.</p>
    </step>
    <step>
        <p>The <b>Run</b> tool window opens at the bottom of the IDE and shows the build progress. A successful build ends with the message <em>'[your project] built without problems.'</em></p>
        <img src="build-output.png" alt="Run tool window showing a successful build with no problems" border-effect="line"/>
        <p>If the output contains errors, fix the flagged topics and run the build again.</p>
    </step>
</procedure>

After the first build, the run configuration appears in the top toolbar. For subsequent builds, click the green **Run** triangle or press <shortcut>Shift+F10</shortcut>.

<img src="run-toolbar.png" alt="Top toolbar showing the saved build configuration and Run button" border-effect="line"/>

<tip>
To check for errors without generating the full output archive, enable dry run mode: press <shortcut>Ctrl+Shift+A</shortcut> (Windows/Linux) or <shortcut>Cmd+Shift+A</shortcut> (macOS), search for <b>Registry</b>, then find and enable the <code>wrs.dry.run</code> key.
</tip>

## Browser preview

To verify the full built site — with working search, all pages, and any custom CSS — click **Open in Browser** in the top-right corner of the Writerside Preview pane.

<img src="writerside-preview-tooltip.png" alt="Writerside Preview toolbar with Open in Browser button highlighted" border-effect="line"/>

<note>
The in-IDE preview renders individual topics. Use the browser view to verify cross-page navigation, search, and any custom CSS defined in <code>buildprofiles.xml</code>. You need a successful full build before opening in browser.
</note>

Once your documentation builds and renders correctly, continue to [Push to GitHub](push-github.md) to publish the project source to a remote repository.
