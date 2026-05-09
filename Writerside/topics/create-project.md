# Create a documentation project

<procedure title="Create a new documentation project" id="create-project">
    <step>
        <p>From the main menu, select <b>File | New | Project</b>.</p>
        <img src="new-project-menu.png" alt="File menu with New > Project highlighted" border-effect="line"/>
    </step>
    <step>
        <p>In the <b>New Project</b> wizard, select <b>Writerside</b> on the left. On the right, select <b>Starter Project</b> and click <b>Next</b>.</p>
        <img src="new-project-wizard-writerside.png" alt="New Project wizard with Writerside and Starter Project selected" border-effect="line"/>
        <tip>
            The wizard also offers other templates:
            <list>
                <li><b>Playground</b> — multiple sample topics demonstrating Writerside markup features.</li>
                <li><b>Import from MD</b> — imports an existing set of Markdown files.</li>
                <li><b>API Docs</b> — an OpenAPI documentation template.</li>
            </list>
            The steps and project structure below apply to the <b>Starter Project</b> template. Other templates will produce a different set of files.
        </tip>
    </step>
    <step>
        <p>Enter a <b>Project name</b> and confirm the <b>Project location</b>, then click <b>Create</b>.</p>
        <img src="new-project-name.png" alt="New Project dialog showing project name and location fields" border-effect="line"/>
    </step>
</procedure>

IntelliJ IDEA creates the project and opens the Writerside welcome topic. The **Writerside** tool window on the left shows the **Help Instance** and its table of contents.

<img src="project-starter-page.png" alt="Newly created Writerside project showing the Getting Started topic" border-effect="line"/>

## Project structure

A Starter Project generates the following files:

```
MyProject/
└── Writerside/                      ← help module
    ├── cfg/
    │   └── buildprofiles.xml        ← output customization (colors, footer, etc.)
    ├── topics/
    │   ├── Default-topic.md         ← your starter topic — edit this to add content
    │   └── lib.md                   ← reusable snippet library
    ├── c.list                       ← topic categories
    ├── hi.tree                      ← table of contents definition
    ├── v.list                       ← reusable variables
    ├── Writerside_libraries.tree    ← library instance config
    └── writerside.cfg               ← module configuration
```

<note>
Other templates (Playground, Import from MD, API Docs) produce a different file structure. The <b>Writerside</b> directory name is the default module name — you can rename it to anything, such as <code>docs</code>, without affecting how the project builds.
</note>

## Start writing

Open `Writerside/topics/Default-topic.md` — this is your starter topic. Replace the placeholder content with your own documentation. The Writerside Preview pane updates as you type.

To add more topics, right-click the **topics** folder in the Project tool window and select **New | Writerside Topic**, or use the **+** button in the table of contents panel of the Writerside tool window.

Once your project is set up and you have added your content, continue to [Build and preview the documentation](build-preview.md).
