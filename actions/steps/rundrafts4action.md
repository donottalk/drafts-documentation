---
title: Action Step – Run Drafts 4 Action
---

Run a named action in the Drafts 4, the previous version of Drafts. This step is a convenience method for cases where a certain action configured in Drafts 4 can not be directly migrated to Drafts 5.

Under the hood this method uses Drafts 5 callback URL support and Drafts 4 URL schemes to open Drafts 4, run the action, and return to Drafts.

## Options

- **Action name**: Name of a valid action in the Drafts 4 app. Must match exactly.
- **Template**: Template for content to send to Drafts 4 as an "text" parameter.
