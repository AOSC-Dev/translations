### How to apply translations

Install `translate-toolkit` (`pip install translate-toolkit`).

Do `po2prop -i Messages.zh_CN.po -o Messages_zh.properties -t Messages.properties`.

If you are working with compiled `icedtea-web`:

1. Locate `/usr/share/icedtea-web/netx.jar`
2. Open as zip archive
3. Locate `netx/net/sourceforge/jnlp/resources/`
4. Put `Messages_zh.properties` into `netx/net/sourceforge/jnlp/resources/`
