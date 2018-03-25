---
title: Credentials
---

{% include back.html title="Settings" path="/settings" %}

{% include doc-image.html src="/settings/credentials.png" %}

Some services accessed via Drafts actions require authentication. In these cases, the first time the action is used Drafts will trigger the necessary authentication process and when successfully completed, store the credentials for reuse.

In most cases, these services use [OAuth](https://en.wikipedia.org/wiki/OAuth) and you will be redirected to the website for the service to provide your login and authorize Drafts. Drafts will store the token provided in these cases, and you will not need to enter your username and password directly in Drafts.

Some action may also prompt for credentials to be entered directly in Drafts. Action steps (like [WebDAV]({{ site.baseurl }}/actions/steps/webdav)), or scripted actions which use the [Credential](https://github.com/agiletortoise/drafts-documentation/wiki/Credential) object, may prompt for input of credential information on first run as well.

To log out of a service, visit *Settings > Credentials* in Drafts, and "Forget" the account you wish to remove.  If you use an action requiring this service again, you will be prompted to re-authenticate.  When a service is forgotten, all saved data related to that service is removed from your Drafts installation and iCloud. To login again, simply run an action using that service again and you will be prompted to authenticate.

### Multiple Accounts

{% include doc-image.html src="/settings/credentials-accounts.png" %}

Action steps which use credentials have an optional "Credential Identifier" field in their options. If you are only using one account for a service, such as Dropbox or Twitter, this field can remain blank.  To have one or more actions target a second account, place a value in the "Credential Identifier" field and any actions with the same identifier will use the same account.

The first time an action for that service, with a specific identifier, a new authentication process will be started - be sure to login to the proper account you wish to target in that process.

A common example use case for identifiers is to setup actions to target more than one Twitter account. So, for example, you might assign a second Twitter action step an identifier
