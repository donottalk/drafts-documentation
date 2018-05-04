---
title: Changelog
---

#### 5.0.5

- **New:** Full access to Twitter API via Twitter object `request` method. Drafts will handle the OAuth, and you can make any valid calls against the Twitter API. [Details on methods in scripting documentation](http://reference.getdrafts.com/objects/Twitter.html). Same actions, like a Tweet Storm example, in the [Twitter integration guide](https://forums.getdrafts.com/t/using-twitter-with-drafts/109).
- **Fix:** Refactor animation to avoid oddball case where the side panels could get stuck when the cursor was in certain positions with certain content in a draft.
- **Fix:** Threading issue scripting twitter updateStatus calls.
- **New:** Inbox/Flagged/Archive/Trash tabs now support drag and drop. Draft drafts from list onto them to move them (or assign flags).

### 5.0.4

- **New:** iMessages app is back and better than ever. With tag filtering, it makes it really easy to use Drafts as a snippet library to insert text into Messages. [More information](/messages)
- **New:** Inbox/Flagged/Archive/Trash tabs in draft list now support drag and drop. Drag drafts from list onto them to move them (or assign flags).
- **New:** "Inbox default swipe action" setting in "..." options of draft list. Allow changing of the default behavior of a full swipe on a draft in the inbox between "Archive" and "Trash". Default is "Archive".
- **New:** External keyboard shortcuts for cancel (cmd-.) and continue (cmd-return) options in HTML Previews.
- **New:** Improvements to drafts selection screen, which is used in iMessages, the Share extension and the `app.selectDraft()` method. Can now be filtered by a tag and archive can be browsed. Sometime down the road it will get better filtering, but this will do for now.
- **New:** Twitter action now logs URL for tweet in action log when successful in the action log. - **New:** `Twitter` script object with `updateStatus(string)` method to post a tweet, returns bool success value. Details in scripting reference. [Details](https://github.com/agiletortoise/drafts-documentation/wiki/Twitter)
- **New:** `editor.deactivate();` script method to resign focus - opposite of existing `editor.activate();` method

- **Change:** Update MultiMarkdown from 6.0 to 6.3.2 to incorporate latest fixes/updates. Includes a few bugs rendering tables w/o opening closing pipe characters and with maintaining indents in code blocks.
- **Change:** Improve margin calculations to better optimize readable line lengths, especially on the big iPads.
- **Change:** Use Safari View Controller in-app to open http links in Link mode.
- **Change:** Improved refresh of processed updates when viewing a draft on Apple Watch.
- **Change:** Improve visibility in Workspaces Today widget.
- **Change:** A few tweaks to Evernote login process to try to fix login for some in China - this may or may not help users seeing these issues, please report back.
- **Change:** Some improvements for migrating actions from Drafts 4.

- **Fix:** `editor.undo()`, `editor.redo()` were not working properly.
- **Fix:** Maintain position of quick access tabs (both Workspace and Action Groups) after selecting new tab.
- **Fix:** Text could go behind keyboard row on iPhone X with external keyboard connected. - **Fix:** Crash accessing App Store with poor network connectivity.
- **Fix:** Clean up a few crashes calling Javascript methods is bad arguments.
- **Fix:** Do not allow edit of name in current list options workspace.
- **Fix:** VoiceOver issues with tag selection and editing.

### 5.0.3

- **New:** Better drag and drop in action list. Actions can now be dragged between groups by switching group tabs, and also dropped on a different group in the group list to move them.
- **Fix:** Automatic theme change would loose cursor position and not update keyboard appearance.
- **Fix:** Rework implementation of "Insert text" to be faster and work better with TextExpander snippets.
- **Fix:** Better updating of app badge when background sync completes or Siri creates draft.
- **Fix:** [[selection]] tag not return correct result when selection was at very end of draft.
- **Fix:** If a query was left in the draft list search field, it would get restored on a cold start of the app, but the not show in the search text in the text box making you wonder where all your drafts went.
- **Fix:** Changes to tags made in scripting might not save if the action had after success setting.
- **Fix:** Share extension might not immediately unlock pro features when subscription is initiated.
- **Fix:** Clear button in recent tag suggestions would not stay in scrollable view.
- **Fix:** Make sure custom template tags generated in an action are cleared when action is finished running.
- **Fix:** Remove some overhead from scripts which manipulate editor selections to prevent some race conditions with the selection when actions are run quickly, repeatedly, like from a keyboard shortcut.
- **Fix:** Case where bad tag filter could get applied to draft list after launching to search from widget.
- **Fix:** Changing syntax highlighting for draft without making any other changes to draft did not save change.
- **Fix:** Add "after success" label in group editing.
- **Fix:** Scripting theme change should require Pro subscription.

### 5.0.2

- Initial public release.
