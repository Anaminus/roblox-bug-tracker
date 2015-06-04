## Things

- Create steps that require as little complexity as possible while still producing the bug ("minimal reproduction").
- Create a place or model file that shows the bug in action. ([submit it with a PR](#submitting-issue-files))
- Don't group separate issues into one issue.
- Comments that do not contribute may be removed.
- If you don't understand what's going on, or you can't reproduce the bug, don't bother submitting an issue.

## Directory

- For long-winded feature requests, use **[roblox-enhancement-proposals](https://github.com/RobloxLabs/roblox-enhancement-proposals)** instead.
- For bugs (not feature requests) related to CoreScripts, libraries, and other Lua-implemented internals, use the **[ROBLOX/Core-Scripts](https://github.com/ROBLOX/Core-Scripts)** issue tracker.
- Bugs (not feature requests) related to the default PlayerScripts (e.g. camera and character movement) should also be submitted to the **[Core-Scripts](https://github.com/ROBLOX/Core-Scripts)** issue tracker.
- For issues related to Gear, Hats, and other assets **made by ROBLOX**, use the unofficial **[asset bug tracker](https://github.com/matthewdean/roblox-asset-bug-tracker)**.
- Before submitting an issue related to the website, make sure the issue still occurs with browser extensions disabled. Also indicate which browser you are using. To temporarily disable extensions:
	- Chrome Incognito Mode: Menu > New incognito window (or Ctrl+Shift+N)
	- Firefox Safe Mode: Menu > Help Menu > Restart with Add-ons Disabled... > Start in Safe Mode (or hold Shift while opening firefox)
- **Do not** use this tracker to report exploits and vulnerabilities. These should be reported by emailing info@roblox.com, or by sending a private message to [ConvexHero](http://www.roblox.com/User.aspx?id=66766775).
- **[Go to the Issue Tracker](https://github.com/Anaminus/roblox-bug-tracker/issues)**

## Labels

Here be descriptions for labels in the issue tracker. Try to construct your issues around these labels. If you think your issue requires a new kind of label, submit another issue describing it.

### Unlabed

All issues should have some kind of label. Unlabed issues haven't been checked or dealt with yet. These can be searched for with `no:label`.

### Types

Indicates what kind of issue. Each issue will have exactly one of these.

Label       | Description
------------|------------
bug         | Unexpected behavior, doesn't work as specified, etc...
severe      | Bugs that freeze, crash, break the game, cause data loss, etc...
enhancement | Feature requests, things you would like to see added or improved.
tracker     | Related to this tracker.
invalid     | Not an issue (i.e. expected behavior), should be submitted elsewhere, or otherwise does not follow the format of this tracker.

### Categories

Indicates where the issue occurs. Each issue will have exactly one of these.

Label      | Description
-----------|------------
Player     | Occurs only on the Roblox client (RobloxPlayer), not the Studio.
Studio     | Related to the UI or functionality of Roblox Studio, or occurs only in Roblox Studio.
Engine     | Occurs in-game, related to implementation, behavior, etc. Applies to both the Studio and the Player.
Lua API    | Related to the Lua API. e.g. misspelled member name, API does not match implementation, etc.
FileSystem | Involves Roblox-related data on the file system, and how the Roblox launcher/installer interacts with the file system.
Website    | Occurs on Roblox websites; roblox.com, m.roblox.com, wiki.roblox.com, etc. **robloxlabs.com is not included!**

### Status

The current state of the issue. Each issue will have zero or one of these.

Label     | Description
----------|------------
duplicate | A similar issue has already been submitted. The issue will still be marked with the appropriate labels.
needsinfo | The issue is unclear or needs reproduction steps. Issues with this tag are closed, but may be reopened if sufficient information is provided. The issue will still be marked with the appropriate labels.

### Developer

Indicates interaction involving actual developers of Roblox. Each issue may have zero or one of these.

Label   | Description
--------|------------
willfix | Confirmed by a developer that the issue will be fixed/added.
wontfix | Confirmed by a developer that the issue will not be fixed/added.

### Platforms

On which platform (operating system) an issue occurs. These will only be used if an issue occurs on some platforms, but not others.

- Windows XP
- Windows 7
- Windows 8
- OS X
- iOS
- Android

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

## Assignees

No actual use. Issues assigned to the owner are marked for periodic checking
to see whether they've been fixed. Collaborators should not assign issues to
anyone.
