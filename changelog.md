---
title: Changelog
---

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
