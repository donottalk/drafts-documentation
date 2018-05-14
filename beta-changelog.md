---
title: Changelog – Beta Version
---

#### 5.1.0.5

- **New:** Event action step returns for creating calendar events with default system card. [Docs](http://getdrafts.com/actions/steps/event)
- **New:** `event.edit()` method. Displays a `Event` object in the system event editing card. Allows scripting to create modify the default values for the event (start/end, add alarms, etc.) then display the event for modification/editing and adding to the calendar. [Docs](http://beta-reference.getdrafts.com/objects/Event.html)
- **Fix:** Better restore of text selections when undo/redo are used.

#### 5.1.0.4

- **New:** `Calendar` object now has some additional options:
    -  `events(startDate, endDate);` method to query the contents of a calendar. Returns an array of `Event` objects.
    - `Calendar.default` property which returns the system default calendar for new events.
    - `find(title)` method looks up a calendar by name.
    - `Calendar.getAllCalendars();` returns array of all known calendars on the device.
    - [Docs](http://beta-reference.getdrafts.com/objects/Calendar.html)

#### 5.1.0.3

- **Change:** Better error reporting when file imports fail for some reason.
- **Fix:** Workaround dark theme tinting of the system file import view.
- **Fix:** Do not allow external keyboard shortcuts to interfere with arrow keys while editing search fields.

#### 5.1.0.2

- **New:** Box action step to create, append, prepend to files in Box.com service. [Docs and Examples](/actions/steps/box)
- **New:** `Box` script object to read and write files to Box.com service. [Docs](http://beta-reference.getdrafts.com/objects/Box.html)
- **New:** Support traditional table edit mode for better VoiceOver experience.
- **Fix:** Improve frequency of updates to app badge.

#### 5.1.0.1

- **New:** Workspaces and tag filter now support All/Any mode selection to switch between filtering multiple tags in boolean and / or modes.
- **New:** "Open in..." action step to support old-style document interaction export. [Docs and Examples](/actions/steps/openin)
- **New:** Ability to disable/enable and duplicate action steps. Handy for WIP step modifications and variants.

#### 5.0.5.2

- **Fix:** Refactor animation to avoid oddball case where the side panels could get stuck when the cursor was in certain positions with certain content in a draft.

#### 5.0.5.1

- **New:** Full access to Twitter API via Twitter object "request" method. Full docs on the way.
- **Fix:** Threading issue scripting twitter updateStatus calls.

#### 5.0.4.4

- **New:** Inbox/Flagged/Archive/Trash tabs now support drag and drop. Draft drafts from list onto them to move them (or assign flags).

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
