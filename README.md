# Update Notifier

Checks for application updates and notifies when one is available.

Install this module by copying it into your *~/.textadept/modules/* directory or Textadept's
*modules/* directory, and then putting the following in your *~/.textadept/init.lua*:

```lua
local update_notifier = require('update_notifier')
```

There will be a "Help > Check for Updates" menu item. You can also have Textadept check for
updates on startup by setting [`update_notifier.check_on_startup`](#update_notifier.check_on_startup).

This module does not perform any updates. The user is expected to act on any update
notifications.

<a id="update_notifier.browser"></a>
## `update_notifier.browser`

Command used to open a URL in a browser.

<a id="update_notifier.check"></a>
## `update_notifier.check`()

Checks for updates, shows a message box if there is one, and copies the update URL to the
clipboard so the user can download it.

<a id="update_notifier.check_on_startup"></a>
## `update_notifier.check_on_startup`

Whether or not to check for updates on startup.

The default value is `false`.

<a id="update_notifier.fetch"></a>
## `update_notifier.fetch`

Command to send an HTTP request to check for updates.

The default value uses 'curl' on Windows, macOS, and BSD; it uses 'wget' on Linux.



