WineHQ
======

[Wine](http://winehq.org) enables Linux, Mac, FreeBSD, and Solaris users
to run Windows applications without a copy of Microsoft Windows. Wine 
is free software under constant development. Other platforms may benefit 
as well, for example some Windows users find wine working better
than compatibility mode with certain apps.

* General Guides: [WineHQ](https://wiki.winehq.org/Translating),
  [ReactOS](https://reactos.org/wiki/Translation_Introduction).
* StyleGuides: https://www.microsoft.com/Language/en-US/StyleGuides.aspx.
* Terminology: https://www.microsoft.com/Language/en-US/Terminology.aspx.
  This is in [TBX](https://en.wikipedia.org/wiki/TermBase_eXchange) format,
  you may want some really CAT software to use it to help you, for example
  [OmegaT](http://omegat.org). Or you can try Transifex or Crowdin.
* Upstream: [Stats](http://fgouget.free.fr/wine-po/),
  [Git](https://source.winehq.org/git/wine.git/tree/HEAD:/po).

Submission
----------

The only possible way to submit Wine translations is through their 
`wine-patches` mailing list, with an attatchment containing a properly
formatted diff (patch) output.

Unfortunately, it is not easy to make the translation into the 
`wine-devel` list where Wine developers can merge in the new 
translations.

Translation Notes
-----------------

To maintain consistency with Microsoft (R) Windows (R) Text, you should
read Microsoft (R)'s Style Guides first. Like all `zh_CN` translations,
you should also read our PDF.

Like what ReactOS guys say, 
> You don't have to translate everything exactly the same as Windows.
> If you believe you can translate something better than Windows, go on!
> However you are encouraged to keep common terms, like for example the
> menus in the windows.
>
> Also, Try to keep your translation consistent, i.e. try to not translate
> the same term differently in different places.

You can always improve the translations, for example the famous idiotic
zh_CN-MS term “内存不能为 read” (The memory cannot be read) should be
changed.

How Wine's Clean Room Guidelines apply to the translations are still unknown,
so we suggest translators to do it the hard way, i.e. read the guide and try
to follow it, instead of writing a crawler to crawl all those error messages
from MSDN (technically easy when you are feeling lucky).
