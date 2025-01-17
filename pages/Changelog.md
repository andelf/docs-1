- [[Dec 29th, 2021]]
  **Beta 0.5.6**
  Desktop app and Android apk download link: https://github.com/logseq/logseq/releases/tag/0.5.6
	- [[Features]]
		- Add `{{namespace [[page]]}}` macro which can be used as a toc [#3616](https://github.com/logseq/logseq/pull/3616)
		- Docker image for Logseq web app and [Guide Doc](https://github.com/logseq/logseq/blob/master/docs/Docker%20Web%20App%20Guide.md) [#3604](https://github.com/logseq/logseq/pull/3604)
	- [[Thanks]]
		- [[shidenggui]]
			- Enhance block toggle feature [#3559](https://github.com/logseq/logseq/pull/3559)
		- [[Peng Xiao]]
			- Fix empty block children is not clickable issue [#3593](https://github.com/logseq/logseq/pull/3593)
		- [[Yuexun Jiang]]
			- Fix drop into insert mode after using journal shortcut [#3600](https://github.com/logseq/logseq/pull/3600)
	- [[Fixed issues]]
		- Nodes in Graph View is unclickable, caused by wrong pixi.js version introduced in v0.5.5 [#3579](https://github.com/logseq/logseq/issues/3579)
		- Click link and button behaviour [#3599](https://github.com/logseq/logseq/pull/3599) [#3603](https://github.com/logseq/logseq/pull/3603) [#3607](https://github.com/logseq/logseq/pull/3607)
		- Unsynced db between multiple windows, which will cause blank search result pages  [#3640](https://github.com/logseq/logseq/pull/3640)
	- [[Enhancement]]
		- Block expand/collapse toggle [#3585](https://github.com/logseq/logseq/pull/3585)
		- Transition of left sidebar when toggling [#3606](https://github.com/logseq/logseq/pull/3606)
		- Development experience under Linux/Windows [#3575](https://github.com/logseq/logseq/pull/3575) [#3508](https://github.com/logseq/logseq/pull/3608)
- [[Dec 25th, 2021]]
  **Beta 0.5.5**
  Desktop app and Android apk download link: https://github.com/logseq/logseq/releases/tag/0.5.5
	- [[Known Issues]]
		- Graph view pages are not clickable https://github.com/logseq/logseq/issues/3579 (already fixed in nightly build)
	- [[Features]]
		- Multi-window support(New shortcut: `mod+n` to open a new window)
		- Add Android APK build to both Beta release and [Nightly](https://github.com/logseq/logseq/releases/tag/nightly) release
	- [[Thanks]]
		- [[Clark Cui]]
			- Fix some CSS errors
		- [[Bad3r]]
			- Formatting keyboard shortcuts
		- [[Moritz Ulrich]]
			- More fluid Graph scaling on lower-end
	- [[Fixed issues]]
		- Code editor's language label interfere with first line of code
		- Code editor won't switch content while edit config files
		- Some IME doesn't trigger command menu, or have buggy behaviour while inputing
		- Unexpected behaviour caused by abuse of keycode
		- Complex regexp in property parsing
		- Alias is not considered from shortcut / graph / press enter
		- Should not encrypt content of specific file types
	- [[Enhancement]]
		- Add as many language mode to Code editor
		- More precise language highlight in both code editor and presentation mode
		- UI on narrow screens
		- More fluid Graph scaling on lower-end
		- Re-number list items when dwim in an ordered list
		- Pugin APIs, new libs version
		- Massive enhancement on mobile app, both iOS and Android
- [[Dec 14th, 2021]]
  id:: 1df7499f-f3dc-488e-b7c7-05caf07e7505
  **Beta 0.5.4**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.5.4
	- [[Fixed issues]]
		- Today's journal file is not recognized by Logseq when starting
		- Can't embed some IFrame links because of `x-frame-options`
		- Handle code block with non-latin1 chars
		- Modal displaying on narrow screens
	- [[Enhancement]]
		- Graph view forces
			-
			  <div style="position: relative; padding-bottom: 55.72755417956656%; height: 0;"><iframe src="https://www.loom.com/embed/7567e69efa8440cf986c871463586ed3" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
			-
	- [[Nightly]] release!
		- #+BEGIN_WARNING
		  It's unstable compared to the official releases, **use it with caution**!
		  #+END_WARNING
		- https://github.com/logseq/logseq/releases/tag/nightly
- [[Dec 12th, 2021]]
  id:: 6f7ac89f-4a99-426d-8ba9-4a2bf5ef5763
  **Beta 0.5.3**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.5.3
	- [[Fixed issues]]
		- Horizontal line `---` doesn't work
		- Extra newline in code editor
		- Refine saving of code editor and e2e tests
		- Empty blocks are not hidden
		- Can't collapse a block with body
		- Ignore properties when displaying the block's body
		- Search blank
		- High cpu usage introduced by wrong Excalidraw version
- [[Dec 10th, 2021]]
  id:: 14067234-cd43-40d8-9e25-26d2ba75a0a9
  **Beta 0.5.2**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.5.2
	- [[Thanks]]
		- [[Junyi Du]]
			- Enhance WYSIWYG experience of multiline heading
			- fix: DWIM isn't activated at one-line block
			- enhance: only apply DWIM to list item when cursor at EOL
		- [[Devon Zuegel]]
			- Improvements to Settings
			- enhance: improve alert for "a new version has been downloaded"
			- refactor: hard-coded colors -> CSS variables for header tips
			- enhance: tidy up repo dropdown in sidebar
			- fix: handle windows path in shorten-repo-name
			- fix: make Continue? modals more consistent
			- feat: add "add to / remove from favorites" to command palette
				- Shortcut: `Cmd+Shift+F`
			- enhance: color code SRS buttons & extract shortcut to tippy
		- [[Bad3r]]
			- Updated README E2E Testing Instructions
			- Enhance: add waring for clear cache
			- Helping a lot in the community!
		- [[ahonn]]
			- feat: keep indent after copy block refs
		- [[Peng Xiao]]
			- fix: queryElementById type
		- [[Vladimir Sorokin]]
			- Added Russian translation
		- [[Moritz Ulrich]]
			- follow-link-under-cursor!: Add page to 'Recent' list
			- Always add target of `redirect-to-page!` to 'Recent' list.
	- [[Fixed issues]]
		- Code block are not saved
		- Empty block not deleted when there's new file detected from #data-safety
		- Wrong indentation for both templates and copied selections
		- Avoid cyclical refs and deep refs
		- Cut a block doesn't copy its nested children blocks
		- Switching between code block to text editing will cause leading spaces not rendered
		- #tag query doesn't work
		- Handle encryption errors
		- Local graph should popup encryption dialog when re-index
		- Wrong link href for file links #[[Org Mode]]
		- Add .svg to image ext
		- Display user-defined drawer
		- Automatic jump back when click 'prev' in a long page
		- Problem keeping separate graphs separated
		- Logbook disappears when block got embedded
	- [[Enhancement]]
		- Reduce start time from minutes to seconds for large graphs (tested on 10k Markdown files)
		- Type ``` and press Enter to switch to codemirror mode
		- New [[Shortcuts]]
			- `g a` to all pages
			- `g g` to graph view
			- `g f` to open flashcards
		- Move editing into the center of viewport when out of viewport
		- Disable spell check on electron by default
	- [[Breaking Changes]]
		- `:block/title`, `:block/body` and `:block/unordered` are removed from the database schema to reduce both memory usage and start time
			- Re-index is needed!
- [[Nov 25th, 2021]]
  id:: a7a7603c-f4f2-49ab-a9c5-ca78c41b07db
  **Beta 0.5.1**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.5.1
	- [[Fixed issues]]
		- Changes are not saved to files when using Logseq and OneDrive on multiple computers
			- **We strongly encourage you to upgrade to the latest version to avoid any data loss.**
		- Markdown blockquote syntax parsing not backward compatible
		- `Contents` is not considered a "Built-in page" for Graph view
- [[Nov 24th, 2021]]
  id:: 619e5440-72c1-4d04-bf4b-dd911f1c69b3
  **Beta 0.5.0**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.5.0
	- [[Thanks]]
		- [[Gabriel Horner]]
			- Add datalog console extension in dev
			- Fix GitHub CI
		- [[David Whittington]]
			- Support #Arweave URLs for links and images
		- [[Peng Xiao]]
			- Custom macro click issue
	- [[Fixed issues]]
		- [[Windows]] desktop app is finally signed
		- Clean block's referenced old orphaned pages when saving it
		- Can't open a new graph on Linux
		- Git Autocommit not working
		- Can't open external links like Zotero and mail clients
		- Don't create empty pages for alias and tags page properties
		- Auto-complete doesn't vanish after /current time
		- Slow parsing on base64 image link
		- Query filters like `and`, `or` are case sensitive
		- Can't rename pages with nested titles
		- Remove space when showing template popup
		- All Pages view lists all of the images
		- Sometimes shortcuts stopped working
		- `[[` doesn't trigger auto-complete for non-english input methods
	- [[Enhancement]]
		- Convert highlighted word to a link when pasting a URL
		- Save a backup file to `logseq/bak` if writes failed (EBUSY lock)
		- Separate plugins and themes in the marketplace
		- Create today's page when redirect to the home or scrolling to the top of journals
		- Jump to the end of page ref after pressing Enter
		- Avoid press enter at empty page-ref
- [[Nov 19th, 2021]]
  **Beta 0.4.9**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.4.9
	- [[Fixed issues]]
		- Empty graph view
		- Shortcuts can be repeated sometimes
- [[Nov 18th, 2021]]
  id:: 8590ee9b-3f85-40cc-954d-857715503802
  **Beta 0.4.7**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.4.7
	- [[Thanks]]
		- [[Devon Zuegel]]
			- Enhance shortcut tooltips
	- [[Fixed issues]]
		- Rename page references when merging pages
		- Code block indentation
		- Block id not persisted when copy block embed
		- Linked references missing in the right sidebar
		- Make sure blocks have the same format when dragging to another page
		- Check for update
	- [[Enhancement]]
		- Toggle displaying shortcut tooltips on settings
			- ![CleanShot 2021-11-18 at 10.33.24.png](../assets/CleanShot_2021-11-18_at_10.33.24_1637202815754_0.png)
		- Display a warning if a block's content include multiple lists or headings
	- [[Breaking Changes]]
		- Deprecate both Ctrl/Cmd+u for searching and  `Ctrl/Cmd+Shift+u` for search in page, use `Ctrl/Cmd+k` and `Ctrl/Cmd+Shift+k` instead.
- [[Nov 16th, 2021]]
  id:: 38a7f160-5dbb-4ab0-8556-5e45cd15144a
  **Beta 0.4.6**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.4.6
	- [[Thanks]]
		- [[Devon Zuegel]]
			- Add more content-aware classes to textarea for a more WYSIWYG experience
			- Show default home instead of journals in side bar
			- Polish cards
			- Rename "page emoji" to "page icons"
				- This PR renames the page property `emoji` to `icon`, which is a more typical and more flexible name.
		- [[Peng Xiao]]
			- Add page & block ref to search item
			- Add back haschild attribute
	- [[Fixed issues]]
		- Navigating to a page through search caused Logseq to crash to a blank screen
		- Rename page should delete the old page name from search
		- Graphs disappeared (not data-loss) after restarting the app
		- Backspace can't move to previous block if it's a embed block
		- Cycle todos will not deselect the blocks
		- Git still commits even if it's toggled off on settings
		- Pages with "." in the title do not show Hierarchy at the bottom
		- Line starting with - will be disappear after exit editing
		- Cannot edit deadline/schedule using date picking panel
		- Ordered list can't be shown in reference list
		- Drag and Drop inconsistently not working
		- Alt-dragging a bullet to an indented position will create multiple empty bullet
		- Import JSON from Roam has trouble with certain code block syntax
		- No more auto-complete if the cursor moves back to [[]]
		- Empty path when importing roam's json
		- Renaming namespace page will update all its children's links
		- Page-ref replacement if non-slash in path
	- [[Enhancement]]
		- Merging pages when renaming one page to the name of another page
		- Add copy block embed(s)
		- Delay query for linked references
			- Editing the main page should be fast no matter how many linked references it has
		- Cycle todos support cmd+enter
		- Display a warning if config.edn is invalid
		- Don't add another set of (()) when copy block ref to embed
		- Remove built-in properties from search result
		- When depth level > 3, the breadcrumb displays an ellipsis
- [[Nov 10th, 2021]]
  id:: 45fc2d43-4154-4f20-ad60-c3039e35256d
  **Beta 0.4.5**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.4.5
	- [[Features]]
		- Move selected blocks up/down (Ctrl/Cmd + Shift + UP/DOWN)
		- `All pages` support batch delete, search, journals filter and remove orphaned pages
		  collapsed:: true
			- ![CleanShot 2021-10-23 at 00.06.33.png](../assets/CleanShot_2021-10-23_at_00.06.33_1634918821593_0.png)
		- Persist right sidebar state
		- [[Shortcuts]]
			- `g t` to go to tomorrow's page
			- `g p` to go to the previous journal
			- `g n` to go to the next journal
		- `custom.js` support
			- See more at https://github.com/logseq/logseq/pull/2943
	- [[Thanks]]
		- [[Devon Zuegel]]
			- Enhance: add hotkeys for open file in directory (`o d`) / default app (`o f`)
			- Emoji page identifiers + sidebar tweaks
			- Custom editor command trigger
				- New configuration option `:editor/command-trigger`
					- e.g. To use `\` instead of `/` for commands trigger, add `:editor/command-trigger "\\"` to `config.edn`.
		- [[Andelf]]
			- Wrong delta pos when change to empty marker
			- fix: pos and space when cycling marker in header
		- [[Seth]]
			- Update readme to include platform specific docker instructions
		- [[GoldinGuy]]
			- Add time wrapper for scheduled/deadline
		- [[Yongqinchuan Du]]
			- Fix code block wide mode toggle
		- [[Peng Xiao]]
			- Fix: notification wrapper blocks user from interacting with the main area
	- [[Fixed issues]]
		- Failed to import roam research's json
		- Both `Copy as` and `Export page` should be fast now
		- Display the below plus button when zoom in
		- Several issues when renaming namespace pages
		- Marking task from "Now" to "Done" lost tracking time duration data
		- Timetracking for now->later on repeated task
		- Timetracking support seconds now
		- Logbook related issues
		- Files not saved when onboarding if canceled the file picker
		- Encrypted page for revert history version by git
		- Decrypt file content when diff
		- Broken image preview in the right sidebar
		- Fix slash command clashes with Org-mode italics
		- Org page reference allows different page-name and label
		- Blank screen on preview card with empty card
		- Clear block content when auto-complete page references
		- Insert page attributes instead of block property when creating and renaming a page
		- Latex can't be displayed in both block and page preview
		- Unexpected behavior of Ctrl + b
		- Black screen when closing window in fullscreen mode on MacOS
	- [[Enhancement]]
		- Click to edit should jump to the end of inline emphasis and links
		- Smooth transition for left sidebar
		- Make [[DWIM]] optional
			- See more at https://github.com/logseq/logseq/issues/2958#issuecomment-945761631
		- Page suggestion will not allow you to deny the suggestion
		- Enable Enter key to rename page
		- Reload commands when toggle plugins (no need to restart the app)
- [[Oct 12th, 2021]]
  id:: 14cbc67d-695a-48b3-8d33-ddf936977d43
  **Beta 0.4.4**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.4.4
	- [[Fixed issues]]
		- Can't open graph on Linux
		- Performance degradation
		- Favorite when renaming page's title
		- Undo need multiple steps (inserting new block)
		- Recent not working
		- Url can include `{` and `}` now
- [[Oct 11th, 2021]]
  id:: 2c01a84b-d944-4755-bed4-6ff079465567
  **Beta 0.4.3**
  Desktop app download link: https://github.com/logseq/logseq/releases/tag/0.4.3
	- [[Features]]
		- Left sidebar!  🌈  🌈
			-
			  <div style="position: relative; padding-bottom: 93.02325581395348%; height: 0;"><iframe src="https://www.loom.com/embed/5fd05d33377c4254b4ee4b6aae5b193d" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
			-
		- Select multiple blocks to `copy block refs` and `cycle todos`
	- [[Thanks]]
		- [[Ed]]
			- The beautiful https://logseqweekly.com/! Don't forget to subscribe!
				- > With the rapid development of the app and new features/improvements, I created this Weekly Summary to help community members keep up with everything being thought of, created and shared by other fellow Logseq users.
		- [[Mispille]]
			- Awesome proposal to tagging Logseq's issues on GitHub!
				- This proposal is at https://docs.google.com/spreadsheets/d/10-LplNuMo2MUy67lt-WX1z1x50L1pY4bSLPIob1eHRQ/edit?usp=sharing!
		- [[llcc]]
			- [[DWIM]] (do what I mean) for `Enter` key when editing.  
			  Context-awareness of `Enter` key makes editing more easily.
		- [[Devon Zuegel]]
			- Consolidate shortcut docs
		- [[hyrijk]]
			- Fix: plugin api moveBlock not working
		- [[Tomas Vik]]
			- Enhance: pretty print pages-metadata.edn
	- [[Fixed issues]]
		- Data loss when dragging blocks to empty pages
		- Create today's journal when the corresponding file doesn't exist yet
		- Broken block references
			- Remove blank line for some blocks when outputting to md/org
		- Importing from Roam has issues with illegal filenames (Windows)
		- Flashcards wrong number during the review
		- Page rename doesn't work for case-sensitive pages
		- Respect the original page's name in the block content
		- Flashcards don't work when publishing
		- A block can be collapsed only when it has children or its body is not empty
		- Display the edit icon only for the embedded parent block
		- Sanitize html for security (plugins)
		- Disable nested queries (page crash)
		- Support raw path under win32 that includes backslash for local pdf files
		- Goto pdf highlights not working sometimes
		- Markdown footnote definition not working when re-index or refresh
		- preferredThemeMode doesn't work (plugins API)
	- [[Enhancement]]
		- Click title to rename a page
		- Open the first block when opening a new page by Mod+o
		- Many UX enhancements
- [[Changelog_07_09]]
- [[Changelog_06]]
- [[Changelog 2020]]