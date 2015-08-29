Contributing
============

We appreciate all kinds of contributions into our repo. As most of our members
use Chinese (more specifically `zh_CN`), it's generally a good idea to throw
Chinese translations to us. All the communication work to upstream will be done
by us.

![Workflow](https://cdn.rawgit.com/AOSC-Dev/translations/master/workflow.svg)

Issues
------

You can report issues using our Issue feature. Be clear of what you are talking
about. In most cases, you can fix the translation errors yourself by sending
the correct ones for us to merge.

Pull Requests
-------------

Pull requests are appreciated, but since GitHub's never going to run the merge
driver for PO, you should merge it locally first.

And never use the **Merge** button for PO files.

Git
---

We use [git-merge-po](https://github.com/mezis/git-whistles) to perform proper
three-way merges of gettext POs.

To use it, get one copy of the script, give it an excutable permission, and
then add the following lines to your `~/.gitconfig` or `.git/config`:

```INI
# set the command in driver properly to its actual path.
[merge "merge-po"]
	name = Gettext Merge Driver
	driver = git-merge-po %O %A %B
```

Crowdin
-------

Our [Crowdin project](http://l10n.anthonos.org) can be used to contribute
translations. However, we seldom use it, so don't expect your translations
to be merged quickly.

zhconv
------

zhconv is a wrapper script for [OpenCC](https://github.com/BYVoid/OpenCC) and
msgmerge. We use it to utilize translations from other Chinese variants.
Get one copy from
[scriptlets](https://github.com/AOSC-Dev/scriptlets/blob/master/zhconv-merge.sh).

It's highly suggested that you use the example `ZH_POST_OCC()`.
