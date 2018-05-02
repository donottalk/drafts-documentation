---
title: Changelog – Beta Version
---

#### 5.0.4.3

- **New:** "Inbox default swipe action" setting in "..." options of draft list. Allow changing of the default behavior of a full swipe on a draft in the inbox between "Archive" and "Trash". Default is "Archive".
- **New:** `editor.deactivate();` method to resign focus - opposite of existing `editor.activate();` method
- **Change:** Use Safari View Controller in-app to open http links in Link mode.
- **Change:** Improve visibility in Workspaces Today widget.
- **New:** Keyboard shortcuts for cancel (cmd-.) and continue (cmd-return) options in HTML Previews.
- **Change:** Prompt for reviews occassionally.
- **Fix:** Crasher accessing App Store with poor network connectivity.
- **Fix:** Clean up a few crashes calling Javascript methods is bad arguments.
- **Change:** A few tweaks to Evernote login process to try to fix login for some in China.

#### 5.0.4.2

- **New:** iMessages app is back.
- **New:** Improvements to drafts selection screen, which is used in iMessages, the Share extension and the `app.selectDraft()` method.  Can now be filtered by a tag and archive can be browsed. Sometime down the road it will get better filtering, but this will do for now.

#### 5.0.4.1

- **Change:** Update MultiMarkdown from 6.0 to 6.3.2 to incorporate latest fixes/updates. Includes a few bugs rendering tables w/o opening closing pipe characters and with maintaining indents in code blocks.
- **Change:** Improve margin calculations to better optimize readable line lengths, especially on the big iPads.
- **New:** Twitter action now logs URL for tweet in action log when successful.
- **New:** `Twitter` script object.
    - `Twitter.create(identifier)`
    - `updateStatus(string)` method to post a tweet, returns bool success value.
- **Change:** Some improvements for migrating actions from Drafts 4.
- **Fix:** Text could go behind keyboard row on iPhone X with external keyboard connected.
- **Fix:** Do not allow edit of name in current list options workspace.
- **Fix:** `editor.undo()`, `editor.redo()` were not working properly.
- **Fix:** Maintain position of quick access tabs (both Workspace and Action Groups) after selecting new tab.
- **Fix:** VoiceOver issues with tag selection and editing.
- **Change:** Improved refresh of processed updates when viewing a draft on Apple Watch.
