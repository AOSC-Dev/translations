Claws Mail
==========

Moved to Transifex: https://www.transifex.com/aosc-dev/claws-mail

Do not start yet -- there are still some more scripts to be run.

Upstream Guide: http://www.claws-mail.org/faq/index.php/Translator's_Information

Header
------

```PO
# Chinese (China) translation of Claws Mail.
# Copyright © 2000-2015 The Claws Mail team.
# This file is distributed under the same license
# as the Claws Mail package, see COPYING file.
#
# Tsu-Fan Cheng <tscheng@ic.sunysb.edu>, 2003.
# Ralgh Young <bamanzi@gmail.com>, 2004-2007.
# Yuwei Yu <acevery@gmail.com>, 2010.
# Rob <rbnwmk@gmail.com>, 2012.
# Mark Chang (zh_TW translator) <mark.cyj@gmail.com>, 2015.
# Mingye Wang (Arthur2e5) <arthur200126@gmail.com>, 2015.
#
```

Submission
----------

1. Grab from Transifex
2. Merge header translators list
3. `msgmerge -U trans.po repo.po` with current repo file
4. `msgfmt -vc -o /dev/null --check-accelerator=_ --statistics trans.po`
5. Send PO to translations@thewildbeast.co.uk

Maintainance
------------

1. Remember to `msgmerge -U` with upstream POT
2. Remember to upload upstream POT to Transifex
