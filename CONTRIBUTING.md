Contributing
============

We appreciate all kinds of contributions into our repo. As most of our members
use Chinese (more specifically `zh_CN`), it's generally a good idea to throw
Chinese translations to us. All the communication work to upstream will be done
by us.

![Workflow](workflow.svg)

You may want to check the commit history of translations so you don't mess up
with someone else doing the same work as yours. [magtac](http://git.io/vZFnd)
can be used to reverse the order of items in a PO file, so you can minimize the
chance of conflict.

Issues
------

You can report issues using our Issue feature. Be clear of what you are talking
about. In most cases, you can fix the translation errors yourself by sending
the correct ones for us to merge.

Practices
---------

While we appreciate frequent updates on translation works, it is recommended
that you:

- Avoid commit-per-minute;
- Use proper git commit format, as demonstrated below;

```
project: language (locale code), number-of-non-finished, percentage-of-completion
```

You should also read our
[zh_CN L10n Guide](https://repo.aosc.io/aosc-l10n/zh_CN_l10n.pdf).

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

Crowdin Translations should be often synced with master, and each push to
Crowdin should have the current commit hash recorded, so we can use the
three-way driver for us.

zhconv
------

zhconv is a wrapper script for [OpenCC](https://github.com/BYVoid/OpenCC) and
msgmerge. We use it to utilize translations from other Chinese variants.
Get one copy from
[scriptlets](https://github.com/AOSC-Dev/scriptlets/blob/master/zhconv-merge.sh).

It's highly suggested that you use the example `ZH_POST_OCC()`.
