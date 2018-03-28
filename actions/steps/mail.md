---
title: Action Step – Mail
---

Send pre-configured email messages either using Mail.app or web services in the background.

#### Examples

*(Open links on device with Drafts to install)*

- [Mail](http://actions.getdrafts.com/a/1BC)
- [Markdown Mail](http://actions.getdrafts.com/a/1Cp)

#### Options

- **Recipients**: Comma separated list of recipient emails for each of the recipient types. These can be just email address, or "Name <email>" formatted - like "Joe Smith <joe@smith.com>, Jane Doe <jane@doe.com>".
  - **To**
  - **CC**
  - **BCC**
- **Subject**: Template for the subject line.
- **Body**: Template for content of the message. If "Send as HTML" is enabled, this template is expected to output valid HTML, otherwise plain text.
- **Send as HTML**: If enabled, the mail is sent as formatted HTML email and the body template should output fully formed HTML. The most common use of this option is to run Markdown to HTML conversion to get rich-text mail.  In this case the simple template "%%[[body]]%%" can be used.
- **Send in background**: If enabled, the mail will be sent using a web service instead of Mail.app. This does not require user interaction, but recipients must be pre-configured and the email will come addressed "From: drafts5@drafts5.agiletortoise.com". This is best suited for "Email to myself", or to send to services which provide a dedicated unique incoming email address as a dropbox.
