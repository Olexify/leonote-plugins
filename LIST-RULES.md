# Rules for the plugin list

The list is one public file, `plugins.json`, in the `leonote-plugins` repository. The Leonote app reads it only when
someone opens Settings › Plugins › Search plugins. To add or update a plugin, open a pull request there that changes
its row. `plugins.template.json` shows a row.

A plugin on the list must:

1. Be free, with its code public in its own GitHub repository.
2. Have an open-source licence in that repository.
3. Follow the law, and the rules of every service it uses. No getting around a site's rules, limits, ads or paywall,
   and no saving what a site does not allow to be saved.
4. Do what its description says, and ask only for the permissions it uses.
5. Contain nothing from Leonote itself except the examples (`example/` and `plugins.template.json`, under MIT-0), and
   not patch or bypass it (LICENSE, section 2B). Do not suggest that Leonote's maker made or endorses it.
6. Hold no paid unlocks, ads, tracking or hidden downloads of more code.
7. Hold nothing unsuitable for a general audience.

The row:

- `zip` is a file of that repository's own GitHub release, with `plugin.json` at its top or in one folder.
- `sha256` is that file's SHA-256. `id`, `version` and `permissions` match its `plugin.json`.
- `stars` is the repository's GitHub stars on the day the list's maintainer last counted them. The list's top-level
  `"updated": "YYYY-MM-DD"` names that day, and Leonote shows the stars "as of" it.
- `verified` is `null`, or `{ "version": ..., "sha256": ... }`.
  Verified: the list's maintainer read the code of this exact version and file for network use it does not declare, and nothing else. Not a security audit, and no guarantee.
  A new version or file is "Not verified" until read again. Verification is never paid for, in money or
  anything else. A plugin by the list's maintainer says so in its description.

Anyone can report a plugin on the list's issue page, which each row's Report button opens. A plugin that breaks these
rules may be taken off the list. Removing it from the list does not remove it from anyone's computer. If a plugin on the
list infringes your copyright or other rights, write to the address for copyright complaints in Leonote's LICENSE
(section 10), naming the plugin, the work concerned and how to contact you.
