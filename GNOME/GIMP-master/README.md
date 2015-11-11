GIMP-master
===========

Cleanup of GIMP-master in GNOME. 

Expected Procedure
------------------

* Pre-Import work: check for newer translations in gimp-2.8, and merge into
  master. Apply file format suggestions (e.g. plurals) as in zh_CN_l10n.
* Import into repo.
* Do cleanup job. This mainly consists of:
  * Punctation and formatting checks as described in zh_CN_l10n.
  * Make a table for terminology differences between common sence (Inkscape &
    Adobe(R) Photoshop(R) combined)
  * Apply the table by running search-and-replace.
* Continue translation.
* Submit translations. Use the table and search-and-replace to generate a
  *old-terminology* version in case someone prefers those creepy terms.
* Port translations to GIMP-2.8.
* Submit 2.8, and update aosc-os-abbs archives to use our own translations.
* Archive the branch status by running `git format-patch` and making a tarball
  for others' reference.

Terminology Difference
----------------------

| Orig         | Old | Ours | Convert back?|
|--------------|-----|------|--------------|
|Brush         |画笔 |笔刷   | yes|
|indexed images|索引图像|索引颜色图像|no|
