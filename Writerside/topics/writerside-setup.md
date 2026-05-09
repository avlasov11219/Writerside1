# Building Your First Documentation Project with Writerside

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
        <p>Most desktop Linux distributions already include the required system libraries. If you are on a minimal or server install, verify that the following packages are present and install any that are missing:</p>
        <code-block lang="bash">
sudo apt install libxi6 libxrender1 libxtst6 mesa-utils libfontconfig libgtk-3-bin tar dbus-user-session
        </code-block>
    </tab>
</tabs>

<note>
BSD-based operating systems are not supported.
</note>

You do not need to install Java separately. IntelliJ IDEA bundles JetBrains Runtime (based on Java 21).

## In this guide

1. [Install IntelliJ IDEA](install-intellij.md) — via the Toolbox App or a standalone installer
2. [Install the Writerside plugin](install-writerside-plugin.md) — from inside the IDE or the JetBrains Marketplace
3. [Create a documentation project](create-project.md) — set up your first Writerside project from a template
4. [Build and preview the documentation](build-preview.md) — compile and verify your docs locally
5. [Push to GitHub](push-github.md) — publish your project source to a remote repository

<seealso>
    <category ref="wrs">
        <a href="https://www.jetbrains.com/help/writerside/local-build.html">Build documentation locally</a>
        <a href="https://www.jetbrains.com/help/writerside/markup-reference.html">Markup reference</a>
        <a href="https://www.jetbrains.com/help/writerside/manage-table-of-contents.html">Manage the table of contents</a>
        <a href="https://www.jetbrains.com/help/writerside/deploy-docs-to-github-pages.html">Deploy to GitHub Pages</a>
    </category>
</seealso>
