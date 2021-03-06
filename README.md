# Chord Heavy - A keymap inspired by [Spacemacs](https://www.spacemacs.org/)

- [Chord Heavy - A keymap inspired by Spacemacs](#chord-heavy---a-keymap-inspired-by-spacemacs)
	- [Keymap](#keymap)
		- [Important Single-chords](#important-single-chords)
		- [Preferences/Settings (prefix: `,`)](#preferencessettings-prefix)
		- [Buffers (prefix: `b`)](#buffers-prefix-b)
		- [Code (prefix: `c`)](#code-prefix-c)
		- [Debug (prefix: `d`)](#debug-prefix-d)
		- [Errors (prefix: `e`)](#errors-prefix-e)
		- [Files (prefix: `f`)](#files-prefix-f)
		- [Git (prefix: `g`)](#git-prefix-g)
		- [Help (prefix: `h`)](#help-prefix-h)
		- [Jump (prefix: `j`)](#jump-prefix-j)
		- [Panel (prefix: `l`)](#panel-prefix-l)
		- [Open... (prefix: `o`)](#open-prefix-o)
		- [Project (prefix: `p`)](#project-prefix-p)
		- [Quit/Close (prefix: `q`)](#quitclose-prefix-q)
		- [Refactor (prefix: `r`)](#refactor-prefix-r)
		- [Search (prefix: `s`)](#search-prefix-s)
		- [Toggle (prefix: `t`)](#toggle-prefix-t)
		- [Window (prefix: `w`)](#window-prefix-w)
		- [Yank/Copy (prefix: `y`)](#yankcopy-prefix-y)
		- [Misc. (one-off shortcuts, most not `chords)`](#misc-one-off-shortcuts-most-not-chords)
	- [Inspiration](#inspiration)
	- [Caveats](#caveats)
	- [Issues to Vote For](#issues-to-vote-for)
	- [Potential Future Improvements](#potential-future-improvements)

After trying and failing to get a [Spacemacs](https://www.spacemacs.org/) installation to function properly, I came back to VSCode since it was significantly less finicky to set up (don't @ me, Spacemacs diehards). However, the one thing that I _really_ liked about Spacemacs was the [mnemonic](https://develop.spacemacs.org/doc/DOCUMENTATION.html#mnemonic), chord-focused shortcuts to execute actions and navigate.

So I set out to create [a keymap](#keymap) [within the confines of VSCode's mechanisms](#caveats) that "made sense". A lot of the base keymap configurations were either taken straight from Spacemacs or from the [Intellimacs](https://github.com/MarcoIeni/intellimacs/blob/master/docs/KEYBINDINGS.org) keybindings. Some chords exist because they "made sense" to me, so please refer to the keymap if you need some guidance! Most things should "just work" if you replace common Spacemacs chords' `SPC` with `cmd` in your head (more information on "why `cmd`?" in the [Inspiration](#inspiration) section).

Also, before you get mad at me, I really encourage you to read the [Caveats](#caveats) section for this keymap.

## Keymap

### Important Single-chords

| Action                                     | Keybinding/Chord |
| ------------------------------------------ | ---------------- |
| `workbench.action.showCommands`            | `ctrl+space`     |
| `workbench.action.terminal.toggleTerminal` | `ctrl+'`         |
| `workbench.action.files.save`              | `ctrl+s`         |

### Preferences/Settings (prefix: `,`)

| Action                                                        | Keybinding/Chord |
| ------------------------------------------------------------- | ---------------- |
| `workbench.action.openGlobalSettings`                         | `cmd+, ,`        |
| `workbench.action.selectIconTheme`                            | `cmd+, i`        |
| `workbench.action.openGlobalKeybindings`                      | `cmd+, k`        |
| `workbench.action.configureLanguageBasedSettings`             | `cmd+, l`        |
| `workbench.extensions.action.showRecommendedKeymapExtensions` | `cmd+, m`        |
| `workbench.action.openSnippets`                               | `cmd+, n`        |
| `workbench.action.openSettingsJson`                           | `cmd+, s`        |
| `workbench.action.openGlobalKeybindingsFile`                  | `cmd+, shift+k`  |
| `workbench.action.selectTheme`                                | `cmd+, t`        |
| `workbench.action.openWorkspaceSettings`                      | `cmd+, w`        |

### Buffers (prefix: `b`)

| Action                                    | Keybinding/Chord |
| ----------------------------------------- | ---------------- |
| `workbench.action.quickOpen`              | `cmd+b b`        |
| `workbench.action.closeActiveEditor`      | `cmd+b d`        |
| `workbench.action.closeWindow`            | `cmd+b d`        |
| `workbench.action.nextEditor`             | `cmd+b n`        |
| `workbench.action.previousEditor`         | `cmd+b p`        |
| `workbench.action.files.newUntitledFile`  | `cmd+b s`        |
| `workbench.action.closeUnmodifiedEditors` | `cmd+b shift+d`  |
| `workbench.action.reopenClosedEditor`     | `cmd+b u`        |

### Code (prefix: `c`)

| Action                      | Keybinding/Chord |
| --------------------------- | ---------------- |
| `editor.action.commentLine` | `cmd+c l`        |
| `code-runner.run`           | `cmd+c r`        |

### Debug (prefix: `d`)

| Action                                                | Keybinding/Chord |
| ----------------------------------------------------- | ---------------- |
| `editor.debug.action.goToNextBreakpoint`              | `cmd+d c`        |
| `workbench.action.debug.continue`                     | `cmd+d c`        |
| `workbench.action.debug.start`                        | `cmd+d d`        |
| `workbench.action.debug.stepInto`                     | `cmd+d j`        |
| `workbench.debug.action.toggleRepl`                   | `cmd+d l`        |
| `workbench.action.debug.stepOver`                     | `cmd+d n`        |
| `workbench.action.debug.stepOver`                     | `cmd+d n`        |
| `workbench.view.debug`                                | `cmd+d o`        |
| `workbench.action.debug.run`                          | `cmd+d r`        |
| `workbench.debug.action.focusBreakpointsView`         | `cmd+d shift+b`  |
| `workbench.debug.viewlet.action.removeAllBreakpoints` | `cmd+d shift+c`  |
| `workbench.action.debug.restart`                      | `cmd+d shift+d`  |
| `workbench.action.debug.stepOut`                      | `cmd+d shift+o`  |
| `editor.debug.action.toggleBreakpoint`                | `cmd+d t`        |

### Errors (prefix: `e`)

| Action                                 | Keybinding/Chord |
| -------------------------------------- | ---------------- |
| `workbench.action.problems.focus`      | `cmd+e l`        |
| `editor.action.marker.next`            | `cmd+e n`        |
| `editor.action.marker.next`            | `cmd+e n`        |
| `editor.action.marker.nextInFiles`     | `cmd+e n`        |
| `workbench.action.output.toggleOutput` | `cmd+e o`        |
| `editor.action.marker.prev`            | `cmd+e shift+n`  |
| `editor.action.marker.prev`            | `cmd+e shift+n`  |
| `editor.action.marker.prevInFiles`     | `cmd+e shift+n`  |

### Files (prefix: `f`)

| Action                                            | Keybinding/Chord |
| ------------------------------------------------- | ---------------- |
| `editor.action.formatDocument`                    | `cmd+f =`        |
| `editor.action.formatSelection`                   | `cmd+f =`        |
| `workbench.files.action.compareWithClipboard`     | `cmd+f c`        |
| `revealFileInOS`                                  | `cmd+f cmd+r`    |
| `toggleFindRegex`                                 | `cmd+f cmd+r`    |
| `toggleSearchRegex`                               | `cmd+f cmd+r`    |
| `workbench.action.terminal.toggleFindRegex`       | `cmd+f cmd+r`    |
| `workbench.action.terminal.toggleFindRegex`       | `cmd+f cmd+r`    |
| `workbench.action.openRecent`                     | `cmd+f e`        |
| `workbench.action.quickOpen`                      | `cmd+f f`        |
| `workbench.action.findInFiles`                    | `cmd+f g`        |
| `workbench.action.editor.changeLanguageMode`      | `cmd+f l`        |
| `extension.advancedNewFile`                       | `cmd+f n`        |
| `outline.focus`                                   | `cmd+f o`        |
| `fileutils.renameFile`                            | `cmd+f r`        |
| `workbench.action.files.saveWithoutFormatting`    | `cmd+f s`        |
| `fileutils.newFolderAtRoot`                       | `cmd+f shift+n`  |
| `workbench.files.action.showActiveFileInExplorer` | `cmd+f shift+s`  |
| `workbench.action.toggleSidebarVisibility`        | `cmd+f t`        |
| `workbench.view.explorer`                         | `cmd+f t`        |
| `workbench.view.explorer`                         | `cmd+f t`        |
| `workbench.action.files.newUntitledFile`          | `cmd+f u`        |
| `copyFilePath`                                    | `cmd+f y`        |

### Git (prefix: `g`)

| Action                        | Keybinding/Chord |
| ----------------------------- | ---------------- |
| `git.stageAllTracked`         | `cmd+g a`        |
| `git.checkout`                | `cmd+g b`        |
| `git-graph.view`              | `cmd+g g`        |
| `git.init`                    | `cmd+g i`        |
| `git.pull`                    | `cmd+g l`        |
| `extension.openInGitHub`      | `cmd+g o`        |
| `git.pushTo`                  | `cmd+g p`        |
| `workbench.view.scm`          | `cmd+g s`        |
| `git.stageAll`                | `cmd+g shift+a`  |
| `git.branch`                  | `cmd+g shift+b`  |
| `extension.openPrGitPRovider` | `cmd+g shift+o`  |

### Help (prefix: `h`)

| Action                                       | Keybinding/Chord |
| -------------------------------------------- | ---------------- |
| `workbench.action.openDocumentationUrl`      | `cmd+h d`        |
| `workbench.action.showInteractivePlayground` | `cmd+h p`        |
| `workbench.action.openRequestFeatureUrl`     | `cmd+h s`        |

### Jump (prefix: `j`)

| Action                            | Keybinding/Chord |
| --------------------------------- | ---------------- |
| `editor.action.formatSelection`   | `cmd+j =`        |
| `workbench.action.gotoSymbol`     | `cmd+j e`        |
| `extension.aceJump`               | `cmd+j j`        |
| `workbench.action.gotoMethod`     | `cmd+j m`        |
| `workbench.action.showAllSymbols` | `cmd+j s`        |

### Panel (prefix: `l`)

| Action                                     | Keybinding/Chord  |
| ------------------------------------------ | ----------------- |
| `workbench.action.closePanel`              | `cmd+l c`         |
| `workbench.action.focusPanel`              | `cmd+l f`         |
| `workbench.action.terminal.resizePaneLeft` | `cmd+l left`      |
| `workbench.action.toggleMaximizedPanel`    | `cmd+l m`         |
| `workbench.panel.markers.view.focus`       | `cmd+l p`         |
| `workbench.action.previousPanelView`       | `cmd+l shift+tab` |
| `workbench.action.togglePanel`             | `cmd+l t`         |
| `workbench.action.nextPanelView`           | `cmd+l tab`       |

### Open... (prefix: `o`)

| Action                                              | Keybinding/Chord |
| --------------------------------------------------- | ---------------- |
| `extension.openWithDefault`                         | `cmd+o b`        |
| `extension.dash.emptySyntax`                        | `cmd+o d`        |
| `workbench.view.explorer`                           | `cmd+o e`        |
| `workbench.action.showAllEditorsByMostRecentlyUsed` | `cmd+o shift+e`  |
| `workbench.action.files.openFileFolder`             | `cmd+o f`        |
| `workbench.view.extension.github-pull-requests`     | `cmd+o p`        |
| `workbench.view.extension.project-manager`          | `cmd+o shift+p`  |
| `workbench.view.extension.todo-tree-container`      | `cmd+o t`        |
| `confluence.showPreview`                            | `cmd+o v`        |
| `confluence.showPreviewToSide`                      | `cmd+o v`        |
| `csv.preview`                                       | `cmd+o v`        |
| `csv.preview`                                       | `cmd+o v`        |
| `csv.preview`                                       | `cmd+o v`        |
| `csv.preview`                                       | `cmd+o v`        |
| `excel.preview`                                     | `cmd+o v`        |
| `markdown.showPreview`                              | `cmd+o v`        |
| `markdown.showPreviewToSide`                        | `cmd+o v`        |
| `workbench.view.extensions`                         | `cmd+o x`        |

### Project (prefix: `p`)

| Action                                 | Keybinding/Chord |
| -------------------------------------- | ---------------- |
| `projectManager.saveProject`           | `cmd+p c`        |
| `projectManager.editProjects`          | `cmd+p e`        |
| `workbench.action.quickOpen`           | `cmd+p f`        |
| `projectManager.listProjects`          | `cmd+p p`        |
| `projectManager.renameProject`         | `cmd+p r`        |
| `projectManager.listProjectsNewWindow` | `cmd+p shift+p`  |
| `workbench.action.replaceInFiles`      | `cmd+p shift+r`  |

### Quit/Close (prefix: `q`)

| Action                                       | Keybinding/Chord |
| -------------------------------------------- | ---------------- |
| `workbench.action.closeAllEditors`           | `cmd+q a`        |
| `code-runner.stop`                           | `cmd+q c`        |
| `workbench.action.debug.stop`                | `cmd+q d`        |
| `workbench.action.closeEditorsToTheLeft`     | `cmd+q left`     |
| `workbench.action.closeOtherEditors`         | `cmd+q o`        |
| `workbench.action.quit`                      | `cmd+q q`        |
| `workbench.action.closeEditorsToTheRight`    | `cmd+q right`    |
| `workbench.action.closeEditorInAllGroups`    | `cmd+q shift+a`  |
| `workbench.action.closeEditorsInOtherGroups` | `cmd+q shift+o`  |
| `workbench.action.closeFolder`               | `cmd+q w`        |

### Refactor (prefix: `r`)

| Action                                 | Keybinding/Chord |
| -------------------------------------- | ---------------- |
| `go.godoctor.extract`                  | `cmd+r m`        |
| `python.refactorExtractMethod`         | `cmd+r m`        |
| `editor.action.refactor`               | `cmd+r r`        |
| `editor.action.startFindReplaceAction` | `cmd+r s`        |
| `workbench.action.replaceInFiles`      | `cmd+r shift+s`  |
| `go.godoctor.var`                      | `cmd+r v`        |
| `python.refactorExtractVariable`       | `cmd+r v`        |

### Search (prefix: `s`)

| Action                                      | Keybinding/Chord |
| ------------------------------------------- | ---------------- |
| `workbench.explorer.fileView.focus`         | `cmd+s e`        |
| `actions.find`                              | `cmd+s f`        |
| `editor.action.extensioneditor.showfind`    | `cmd+s f`        |
| `editor.action.webvieweditor.showFind`      | `cmd+s f`        |
| `keybindings.editor.searchKeybindings`      | `cmd+s f`        |
| `problems.action.focusFilter`               | `cmd+s f`        |
| `settings.action.search`                    | `cmd+s f`        |
| `workbench.action.terminal.focusFindWidget` | `cmd+s f`        |
| `workbench.action.terminal.focusFindWidget` | `cmd+s f`        |
| `workbench.action.findInFiles`              | `cmd+s l`        |
| `workbench.action.findInFiles`              | `cmd+s p`        |
| `editor.action.startFindReplaceAction`      | `cmd+s r`        |
| `workbench.action.findInFiles`              | `cmd+s s`        |
| `workbench.action.replaceInFiles`           | `cmd+s shift+r`  |

### Toggle (prefix: `t`)

| Action                              | Keybinding/Chord |
| ----------------------------------- | ---------------- |
| `workbench.action.toggleFullScreen` | `cmd+t f`        |
| `settings.cycle.lineNumbers`        | `cmd+t l`        |
| `toggleVim`                         | `cmd+t v`        |
| `editor.action.toggleWordWrap`      | `cmd+t w`        |
| `workbench.action.toggleZenMode`    | `cmd+t z`        |

### Window (prefix: `w`)

| Action                                             | Keybinding/Chord        |
| -------------------------------------------------- | ----------------------- |
| `workbench.action.splitEditorDown`                 | `cmd+w -`               |
| `workbench.action.splitEditor`                     | `cmd+w /`               |
| `workbench.action.terminal.split`                  | `cmd+w /`               |
| `workbench.action.firstEditorInGroup`              | `cmd+w 1`               |
| `workbench.action.lastEditorInGroup`               | `cmd+w 9`               |
| `workbench.action.previousEditorInGroup`           | `cmd+w alt+cmd+left`    |
| `workbench.action.nextEditorInGroup`               | `cmd+w alt+cmd+right`   |
| `workbench.action.closeEditorsInGroup`             | `cmd+w d`               |
| `workbench.action.closeGroup`                      | `cmd+w d`               |
| `workbench.action.focusBelowGroup`                 | `cmd+w down`            |
| `workbench.action.focusPreviousGroup`              | `cmd+w h`               |
| `workbench.action.focusBelowGroup`                 | `cmd+w j`               |
| `workbench.action.focusAboveGroup`                 | `cmd+w k`               |
| `workbench.action.focusNextGroup`                  | `cmd+w l`               |
| `workbench.action.focusPreviousGroup`              | `cmd+w left`            |
| `multiCommand.closePanelAndSidebarAndOtherEditors` | `cmd+w m`               |
| `workbench.action.newWindow`                       | `cmd+w n`               |
| `workbench.action.quickSwitchWindow`               | `cmd+w o`               |
| `workbench.action.focusNextGroup`                  | `cmd+w right`           |
| `workbench.action.splitEditorDown`                 | `cmd+w s`               |
| `workbench.action.toggleSidebarVisibility`         | `cmd+w s`               |
| `workbench.action.moveEditorLeftInGroup`           | `cmd+w shift+cmd+left`  |
| `workbench.action.moveEditorRightInGroup`          | `cmd+w shift+cmd+right` |
| `workbench.action.closeAllGroups`                  | `cmd+w shift+d`         |
| `workbench.action.moveActiveEditorGroupDown`       | `cmd+w shift+down`      |
| `workbench.action.focusFirstEditorGroup`           | `cmd+w shift+h`         |
| `workbench.action.focusLastEditorGroup`            | `cmd+w shift+j`         |
| `workbench.action.focusFirstEditorGroup`           | `cmd+w shift+k`         |
| `workbench.action.focusLastEditorGroup`            | `cmd+w shift+l`         |
| `workbench.action.moveActiveEditorGroupLeft`       | `cmd+w shift+left`      |
| `workbench.action.moveActiveEditorGroupRight`      | `cmd+w shift+right`     |
| `workbench.action.reopenClosedEditor`              | `cmd+w shift+t`         |
| `workbench.action.moveActiveEditorGroupUp`         | `cmd+w shift+up`        |
| `workbench.action.files.newUntitledFile`           | `cmd+w t`               |
| `workbench.action.focusNextGroup`                  | `cmd+w tab`             |
| `workbench.action.focusPreviousGroup`              | `cmd+w tab`             |
| `workbench.action.focusAboveGroup`                 | `cmd+w up`              |
| `workbench.action.splitEditor`                     | `cmd+w v`               |
| `workbench.action.terminal.split`                  | `cmd+w v`               |
| `workbench.action.closeEditorsInGroup`             | `cmd+w x`               |

### Yank/Copy (prefix: `y`)

| Action                                        | Keybinding/Chord |
| --------------------------------------------- | ---------------- |
| `editor.action.copyLinesDownAction`           | `cmd+y j`        |
| `editor.action.copyLinesDownAction`           | `cmd+y j`        |
| `markdown.extension.onCopyLineDown`           | `cmd+y j`        |
| `editor.action.copyLinesUpAction`             | `cmd+y k`        |
| `markdown.extension.onCopyLineUp`             | `cmd+y k`        |
| `fileutils.copyFileName`                      | `cmd+y n`        |
| `copyFilePath`                                | `cmd+y p`        |
| `workbench.action.files.copyPathOfActiveFile` | `cmd+y p`        |
| `copyRelativeFilePath`                        | `cmd+y shift+p`  |

### Misc. (one-off shortcuts, most not `chords)`

 | Action                                                        | Keybinding/Chord             |
 | ------------------------------------------------------------- | ---------------------------- |
 | `editor.action.selectAll`                                     | `alt+a`                      |
 | `editor.action.webvieweditor.selectAll`                       | `alt+a`                      |
 | `list.selectAll`                                              | `alt+a`                      |
 | `workbench.action.terminal.selectAll`                         | `alt+a`                      |
 | `editor.action.clipboardCopyAction`                           | `alt+c`                      |
 | `editor.action.webvieweditor.copy`                            | `alt+c`                      |
 | `execCopy`                                                    | `alt+c`                      |
 | `filesExplorer.copy`                                          | `alt+c`                      |
 | `gitlens.views.compare.copy`                                  | `alt+c`                      |
 | `gitlens.views.fileHistory.copy`                              | `alt+c`                      |
 | `gitlens.views.lineHistory.copy`                              | `alt+c`                      |
 | `gitlens.views.repositories.copy`                             | `alt+c`                      |
 | `gitlens.views.search.copy`                                   | `alt+c`                      |
 | `keybindings.editor.copyKeybindingEntry`                      | `alt+c`                      |
 | `problems.action.copy`                                        | `alt+c`                      |
 | `remote.tunnel.copyAddressInline`                             | `alt+c`                      |
 | `workbench.action.terminal.copySelection`                     | `alt+c`                      |
 | `undo_expand_region`                                          | `alt+down`                   |
 | `editor.action.peekDefinition`                                | `alt+enter`                  |
 | `markdown-checkbox.markCheckbox`                              | `alt+enter`                  |
 | `editor.action.addSelectionToNextFindMatch`                   | `alt+l`                      |
 | `editor.action.triggerSuggest`                                | `alt+space`                  |
 | `toggleSuggestionDetails`                                     | `alt+space`                  |
 | `expand_region`                                               | `alt+up`                     |
 | `editor.action.fontZoomOut`                                   | `cmd+-`                      |
 | `workbench.action.terminal.focus`                             | `cmd+'`                      |
 | `workbench.action.navigateBack`                               | `cmd+[`                      |
 | `workbench.action.navigateForward`                            | `cmd+]`                      |
 | `editor.action.fontZoomReset`                                 | `cmd+=`                      |
 | `deleteAllLeft`                                               | `cmd+backspace`              |
 | `multiCommand.repeatLastCommand`                              | `cmd+ctrl+r`                 |
 | `editor.action.insertSnippet`                                 | `cmd+k`                      |
 | `editor.action.fontZoomIn`                                    | `cmd+numpad_add`             |
 | `editor.action.commentLine`                                   | `cmd+; ;`                    |
 | `deleteWordPartLeft`                                          | `ctrl+alt+backspace`         |
 | `cursorWordPartStartLeft`                                     | `ctrl+alt+left`              |
 | `cursorWordPartRight`                                         | `ctrl+alt+right`             |
 | `cursorLeft`                                                  | `ctrl+h`                     |
 | `cursorDown`                                                  | `ctrl+j`                     |
 | `list.focusDown`                                              | `ctrl+j`                     |
 | `selectNextSuggestion`                                        | `ctrl+j`                     |
 | `workbench.action.quickOpenSelectNext`                        | `ctrl+j`                     |
 | `cursorUp`                                                    | `ctrl+k`                     |
 | `list.focusUp`                                                | `ctrl+k`                     |
 | `selectPrevSuggestion`                                        | `ctrl+k`                     |
 | `workbench.action.quickOpenSelectPrevious`                    | `ctrl+k`                     |
 | `cursorRight`                                                 | `ctrl+l`                     |
 | `workbench.action.files.save`                                 | `ctrl+s`                     |
 | `deleteWordPartRight`                                         | `ctrl+shift+alt+backspace |` |
 | `cursorWordPartStartLeftSelect`                               | `ctrl+shift+alt+left`        |
 | `cursorWordPartRightSelect`                                   | `ctrl+shift+alt+right`       |
 | `workbench.action.terminal.runSelectedText`                   | `ctrl+shift+alt+t`           |
 | `workbench.action.quickOpenPreviousRecentlyUsedEditorInGroup` | `ctrl+tab`                   |
 | `extension.jumpy-exit`                                        | `Escape`                     |
 | `vscode-neovim.compositeEscape1`                              | `j`                          |
 | `extension.toggleTheme`                                       | `shift+alt+d`                |
 | `extension.jumpy-line`                                        | `shift+alt+enter`            |
 | `editor.action.moveLinesUpAction`                             | `shift+alt+up`               |
 | `editor.action.moveLinesDownAction`                           | `shift+alt+down`             |
 | `editor.action.deleteLines`                                   | `shift+cmd+backspace`        |
 | `cursorUp`                                                    | `up`                         |

## Inspiration

Despite Spacemacs' influence, this keymap uses the "Command (⌘, `cmd`)" key in place of `SPC` in Spacemacs chords. Extensions like [VSpaceCode](https://github.com/VSpaceCode/VSpaceCode) rely on you _needing_ [VSCodeVim](https://github.com/VSCodeVim/Vim) installed, and to be in the editor (the chords in VSpaceCode don't work when your focus is in something like the sidebar). I didn't like that limitation (it didn't feel very Spacemacs-y). Re-orienting myself around such that the `cmd` key was my `leader` key allowed me to remove this restriction and thus be able to use these chords anywhere.

Also, it's worth mentioning that [I use a keyboard powered by QMK software](https://configure.ergodox-ez.com/planck-ez/layouts/5BRQB/Ny4rd/0), and have set my `cmd` key to be a [One Shot Modifier](https://docs.qmk.fm/#/feature_advanced_keycodes?id=one-shot-keys). This makes the chords feel a bit more like Spacemacs, where chords like `SPC w -` are three individual key presses. In this keymap and with a OSM `cmd` key set up, you can think of that same chord as being `cmd w -` (three individual key presses).

Lastly, as I explored creating this keymap, I've come to the conclusion that VSCode generally doesn't really know what to do with chords and they seem to have been bolted on without much thought. As such, there are a number of improvements that can/should be added in the future that would make this keymap even more robust. See the [Issues to Vote For](#issues-to-vote-for) section for some issues to follow/vote for!

## Caveats

There are some caveats to keep in mind if you'd like to use this keymap, which would be difficult to digest for most of the VSCode population (and that's fine; I really only made this because it was fun!). Those caveats are:

- **This keymap removes A LOT of default shortcuts.** If you're not comfortable with looking up the commands or using the command search, stay away from this keymap!
- **There are some chords/shortcuts that are dependent on snippets or extensions that I have personally installed on my machine.** VSCode might complain about this, but you should be fine.
- In VSCode, when you've defined a chord for a specific character, it "clobbers" shortcuts that are only one `modifier+key` combination. Thus, because `cmd+c r` is a chord, things like `cmd+c` in a text editor (copy) won't work (VSCode sits there waiting for a chord to be executed). Despite not needing it in order to get this keymap working, I _am_ a VSCodeVim user, so anything to do with text manipulation is handled by that extension anyway so that's generally not an issue for me. However, if you rely on those kinds of "common" shortcuts, keep in mind that they have changed (more often than not to `alt+key`; for the example above, `alt+c` is the shortcut for copying).
- Right now this keymap only supports the Mac; sorry! I'll add more in the future if literally _anyone_ uses this.

If the above caveats are "fine" for you, I really think that this keymap can work well. It doesn't cover 100% of the capabilities that Spacemacs can, but it gets a lot of the way there!

## Issues to Vote For

VSCode was developed with a completely different user-base in mind, but that doesn't mean that VSCode can't be improved in the future to facilitate Spacemacs-like navigational workflows. While it'd take a significant amount of effort to actually get this to be a Spacemacs replacement, there are some low-hanging fruit issues that, if they were resolved, would improve a keymap like this significantly:

- Add suggested completions for key chords [\#3969](https://github.com/microsoft/vscode/issues/3969)
- Enable keychords of 3 steps [\#6966](https://github.com/microsoft/vscode/issues/6966)
- Reserve shortcut prefix for user [\#87565](https://github.com/microsoft/vscode/issues/87565)
- When using record keys search for individual keys [\#88122](https://github.com/microsoft/vscode/issues/88122)

----

## Potential Future Improvements

- Add support for Linux/Windows
- Create shortcuts that are based on specific file types, so that there is a "major mode" of sorts for them. Can start with HTML and go through other languages as I see fit; use the [Spacemacs layer keybindings](https://www.spacemacs.org/layers/LAYERS.html) for inspiration.
	> NOTE: maybe the `ctrl` key can be first character for "major" mode?
	- [HTML](https://www.spacemacs.org/layers/+lang/html/README.html)
	- [javascript](https://www.spacemacs.org/layers/+lang/javascript/README.html)
	- [markdown](https://www.spacemacs.org/layers/+lang/markdown/README.html)
	- [python](https://www.spacemacs.org/layers/+lang/python/README.html)
	- [go](https://www.spacemacs.org/layers/+lang/go/README.html)
	- [rust](https://www.spacemacs.org/layers/+lang/rust/README.html)
	- [java](https://www.spacemacs.org/layers/+lang/java/README.html)
	- [typescript](https://www.spacemacs.org/layers/+lang/typescript/README.html)
	- [shell-scripts](https://www.spacemacs.org/layers/+lang/shell-scripts/README.html)