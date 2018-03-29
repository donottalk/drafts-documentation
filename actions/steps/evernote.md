---
title: Action Step – Evernote
---

{% include back.html title="Action Steps" path="/actions/steps" %}

Create, append or prepend to notes in [Evernote](http://evernote.com).

#### Examples

- [Save to Evernote]()
- [Append to Evernote Journal]()

#### Options

- **Note**: Template for note name.
- **Notebook**: Template for name of an existing Notebook in your Evernote account. Leave blank to use the default notebook.
- **Tags**: Template for tags to assign the note. Should be comma-delimited list of tags. If they do not exist, they will be created. Use the [[tags]] template tag to assign draft tags.
- **Template**: Template for the content of the note.
- **Template Output Format**: The type of output from the above template property. Evernote uses it's own [HTML-like ENML markup](https://dev.evernote.com/doc/articles/enml.php) for notes and conversion needs to be done before saving. This setting determines how Drafts will apply conversion. Options are:
  - **Text**: Assume the output of the template plain text. Drafts will convert the plain text to ENML by adding line feed tags.
  - **Markdown**: Assume the template output is Markdown. If you want Markdown syntax to be converted to rich-text in Evernote, choose "Markdown". Drafts will take the output of the template and run it through the Markdown processor to convert to X-HTML before sending to Evernote.
  - **ENML**: Assume the output of the template is already valid ENML. This is an advanced setting for cases where scripting or special output is already configured with the necessary valid ENML tags.
- **Write Type**:
  - **create**: Create a new note.
  - **replace**: Create new note, overwriting an existing one with the same name, if it exists.
  - **prepend**: Prepend template content at the beginning of the note. Create the note if it does not already exist.
  - **append**: Append template content at the end of the note. Create the note if it does not already exist.
