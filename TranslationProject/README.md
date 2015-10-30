Translation Project
===================

[Translation Project](https://translationproject.org) is where most GNU
projects put their translations on. It also welcomes other free software.

Submission
----------

TP uses a email [bot](mailto:robot@translationproject.org) for accepting
and processing submissions. The bot only accepts a translation that meets
its [requirements](https://translationproject.org/html/robot.html), in short:

- Subject should be the same as the file name.
  - Package name and version inferred from file name should match
    `Project-Id-Version` field.
- Sender must be in the translators list for the language, so does the
  `Last-Translator`.
- Header should contain valid license information, etc.
- For projects that requires disclaiming, check for sender's disclaim.

TP uses a terrible `--no-wrap` style for archiving, but since it does it
automatically, we don't care about it. Just don't do this here or you will
get a huge commit.

Contact
-------

- [zh_CN](https://translationproject.org/team/zh_CN.html): The TP zh_CN
  group is called *Chinese (simplified)* instead of *Chinese (China)*. It
  doesn't matter except for locale code OCD patients.
  - This group is half-active.
    [List](http://groups.google.com/group/i18n-zh)
- [zh_TW](https://translationproject.org/team/zh_TW.html): *Chinese
  (Traditonal)*, same thing as `zh_CN`.
  - This group is seldom active.
    [List](http://lists.linux.org.tw/cgi-bin/mailman/listinfo/zh-l10n)
- [zh_HK](https://translationproject.org/team/zh_HK.html): *Chinese
  (Hong Kong)*, finally right.
  - This group is silent. No mailing lists available.
- [Coordinators](mailto:coordinator@translationproject.org) are useful if you
  want to do something big. Non-Hostile, rich in protein.

Message Match Possibilities
---------------------------

This graph shows roughly how close packages are to each other. It can be used
as a directive for choosing what files to compendium / TM match from.

- GNU Toolchain
  - Binaries
    - gcc 
    - binutils
      - ld
      - bfd
      - gold
      - gas
      - opcodes
  - Lex n' parse
    - flex
    - bison (-runtime)
  - base-libs
    - libc
    - cpplib (from gcc)
  - m4
  - make
- GNU coreutils-like
  - util-linux
  - tar
  - wget
  - psmisc
    - procps
