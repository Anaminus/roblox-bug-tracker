# Roblox Bug Tracker

An unofficial tracker for bugs that I encounter on [Roblox](www.roblox.com).

**[Go to the Issue Tracker](https://github.com/Anaminus/roblox-bug-tracker/issues)**

For long-winded feature requests, try checking out **[roblox-enhancement-
proposals](https://github.com/RobloxLabs/roblox-enhancement-proposals)**
instead.

## Things

- Try to create steps that reproduce a bug.
- Create a place or model file that shows a bug in action.
- Don't group separate issues into one issue.
- Comments that do not contribute may be removed.
- If you don't understand what's going on, or you can't reproduce a bug, don't
  bother submitting an issue.

## Labels

Here be descriptions for labels in the issue tracker. Try to construct your
issues around these labels. If you think your issue requires a new kind of
label, submit an issue describing it.

### Types

What kind of issue. Every issue should have one of these.

<table>
<tr><th>Label</th><th>Description</th></tr>
<tr><td> bug </td><td>Unexpected behavior, doesn't work as specified, etc...</td></tr>
<tr><td> crash </td><td>Bugs that crash or break the game.</td></tr>
<tr><td> wishlist </td><td>Feature requests, things you would like to see added or improved.</td></tr>
<tr><td> tracker </td><td>Issues related to this bug tracker.</td></tr>
</table>

### Status

<table>
<tr><td> willfix </td><td>Issues where it is confirmed that they will be fixed/added.</td></tr>
<tr><td> wontfix </td><td>Issues where it is confirmed that they will not be fixed/added.</td></tr>
</table>

### Categories

Where the issue occurs.
<table>
<tr><th>Label</th><th>Description</th></tr>
<tr><td> Player </td><td>Issues that occur only on the Roblox client (RobloxPlayer).</td></tr>
<tr><td> Studio </td><td>Issues related to the UI or functionality of Roblox Studio 2013, or issues that occur only in Studio 2013.</td></tr>
<tr><td> Game Engine </td><td>Issues occurring in-game, Instances, the Lua API, etc... Applies to both the Studio and the Player.</td></tr>
<tr><td> Website </td><td>Issues on Roblox websites; roblox.com, m.roblox.com, wiki.roblox.com, etc. <b>robloxlabs.com is not included!</b></td></tr>
</table>

### Platforms

On which platform (operating system) the issue occurs. These should only be
used if an issue occurs on some platforms, but not others.

- Windows XP
- Windows 7
- Windows 8
- OS X
- iOS

Some of these labels may not actually exist until they are needed.

## Submitting Issue Files

You may submit files related to a certain issue by making a pull request.
These files are located in the `issues` folder.

1. Fork this repository.
2. Go to the `issues` folder, and add a new folder. Make sure its name is the
   number of the related issue (i.e. "100" for issue #100).
3. Add your files. Good files are places files (`.rbxl`, `.rbxlx`), model
   files (`.rbxm`), and READMEs, containing instructions.
4. [Create a new pull request](https://help.github.com/articles/creating-a-pull-request).
5. When adding a title and description, refer to the related issue.

If files already exist for an issue, you can create a sub-folder and put your
files there. Try to give the folder a name that suggests why it is separate
from existing files. You may also move the existing files to their own sub-
folder, if necessary. Example:

Existing:

	issues
		100
			ExistingFile.rbxl
			README.md

Updated:

	issues
		100
			ExistingFiles
				ExistingFile.rbxl
				README.md
			YourNewFiles
				YourFile.rbxl
				README.md

### Place files

Try to save places as `.rbxlx` instead of `.rbxl`, since the file's contents
are easier to read.

### Make a pull request separate from the related issue!

If you submit an issue as a pull request, I wont be able to merge it without
also closing the issue.