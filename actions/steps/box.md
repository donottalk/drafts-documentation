---
title: Action Step – Box
---

{% include back.html title="Action Steps" path="/actions/steps" %}

Create, append or prepend to files in the [Box.com service](http://box.com). Note that more advanced Box actions can also be scripted with [Box scripting support](http://reference.getdrafts.com/objects/Box.html).

#### Examples

- [Save to Box](https://actions.getdrafts.com/a/1IX)
- [Append to Box Journal](https://actions.getdrafts.com/a/1IY)

#### Options

- **Name**: Template for file name, including extension.
- **Path**: Path of folder, relative to Box.com account root, to place file. Default "/" is the root of your Box.com folder. Should begin with "/"
- **Template**: Template for the content of the file.
- **Write Type**:
  - **create**: Create a new file. If an existing file already exists at the location, create as new file with a number suffix added.
  - **replace**: Create new file, overwriting an existing if it exists.
  - **prepend**: Prepend template content at the beginning of the file. Create the file if it does not already exist.
  - **append**: Append template content at the end of the file. Create the file if it does not already exist.
- **Identifier**: A string identifier for the OneDrive account to use. This value is only needed if you wish to use more than one Box.com account with Drafts. If used, all actions with the same identifier will use the same alternate login for OneDrive.
