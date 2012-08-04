---
isChild: true
---

## Mac Setup

OSX include PHP, ma è solitamente una versione po' arretrata rispetto a quella stabile più recente. Lion include PHP 5.3.6 e Mountain Lion 5.3.10.

Per aggiornare PHP su OSX puoi installarlo con l'ausilio di alcuni [package managers][mac-package-managers] per Max, dei quali [php-osx by Liip][php-osx-downloads] è raccomandato.

L'altra opzione è [compilarlo da sé][mac-compile], nel caso in cui devi assicurarti di aver installato Xcode oppure l'alternativa della Apple ["Command Line Tools for Xcode"][apple-developer] scaricabile dall'Apple's Mac Developer Center.

Per un pacchetto completo "all-in-one" che comprenda PHP, web server Apache e database MySQL, ed il tutto con una buona interfaccia grafica, prova [MAMP][mamp-downloads].

[mac-package-managers]: http://www.php.net/manual/en/install.macosx.packages.php
[mac-compile]: http://www.php.net/manual/en/install.macosx.compile.php
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
[apple-developer]: https://developer.apple.com/downloads
[mamp-downloads]: http://www.mamp.info/en/downloads/index.html
[php-osx-downloads]: http://php-osx.liip.ch/
