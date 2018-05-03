---
title: Backups
---

{% include back.html title="Settings" path="/settings" %}

Although iCloud sync general serves as a backup to protect you against loss of a device, etc., Drafts can also create on-demand or automated periodic backups of drafts and action groups to iCloud Drive.  These backups can be imported back into Drafts if needed.

{% include doc-image.html src="/settings/backups.png" %}

To make a backup on-demand, or to enable periodic backups, visit Settings > Storage > Backups in Drafts.

Backups will be written to the `Drafts5/Backups` folder in your iCloud Drive.  Once created, these backup files can be imported by opening them from the Files app on any device with Drafts installed.

If periodic backups are enabled, for either drafts or action groups, these periodic backups will be created in the background, approximately every 7 days - depending on how often you launch and use Drafts.

**Note**: _If you enable periodic backups, it is general only needed on one of your devices. For example, if you use Drafts most often on your iPhone, you might enable periodic backup on that device - and NOT on your iPad._

### Details

- All export files may be re-imported into drafts by visiting the Files app, browsing to the file and selecting "Copy to Drafts".
- Drafts export files will have the ".draftsBackup" file extension. The content is encode in JSON format.
- Action Groups are backed up as individual files with ".draftsActionGroup" extensions. These are in a native compressed format, but can be re-imported into Drafts at any time.
- Drafts does not currently perform clean up of older backup files. If periodic back ups are enabled, you may wish to periodically clean up the /Drafts 5/Backups folder in iCloud Drive.
