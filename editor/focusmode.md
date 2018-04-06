---
title: Focus Mode & "New Draft After" Timeout
---

{% include back.html title="Editor" path="/editor" %}

To enable quick-capture, by default Drafts opens to a new, ready-to-edit draft. Drafts offers control over this behavior with the "New draft after" timeout setting, and Focus mode.

### New Draft After Timeout

The new draft after timeout controls how long Drafts has to be idle before returning to the app will create a new draft. The setting defaults to 60 seconds, but can be set to as short as 30 seconds or as long as an hour. This buffer allows you to jump between apps, copy and paste information, etc., with loosing your current draft, while still allowing the app to be ready for a new item after you return. What timeout works best varies depending on how you use the app and how often you return to existing drafts to update them. Focus mode (details below) can be used to completely disable this timeout.

{% include doc-image.html src="/editor/focusmode.png" %}

### Focus Mode

Newly introduced in Drafts 5, focus mode changes two key Drafts behaviors to let you focus on a particular on-going project, or to more easily process a collection of drafts. Focus mode is enabled and disabled using the focus mode button in the lower left of the editor, or in settings. When in focus mode, these two changes occur:

1. The "New draft after" setting is disabled. Draft will always return to the last edited draft, rather than creating a new one when you return to the app after the specified period of time.
2. If an action which uses the [after success](/actions/advancedsettings) to move draft to the archive or trash is used, the next draft in the current draft list filter will be loaded, as if the next button were pressed, rather than creating a new draft.

In combination, these change make it easy to focus on a particular draft if you are doing on-going research, etc., and also make it easy to focus on processing a series of drafts one after the other without having to navigate the draft list to find the next unprocessed draft.
