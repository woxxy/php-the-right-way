---
isChild: true
---

## Namespaces

Come detto sopra, la communità PHP ha un vasto numero di sviluppatori che creano tanto codice. Questo vuol dire che il codice PHP di una libreria potrebbe usare lo stesso nome di classe di un'altra libreria. Quando entrambe le librerie sono usate nello stesso namespace, queste collideranno e causeranno problemi.

I _namespace_ risolvono questo problema. Come descritto nel manuale di riferimento di PHP, i namespace possono essere comparati alle directory dei sistemi operativi che separano ("_namespace_") i file. due file con lo stesso nome possono coesistere in directory separate. Allo stesso modo, due classi PHP con lo stesso nome possono coesistere in diversi namespace PHP. E' tanto semplice.

E' importante che tu faccia uso dei namespace per il tuo codice in modo che altri sviluppatori possano utilizzarlo senza preoccuparsi di collisioni con altre librerie.

Un modo raccomandato di usare i namespace è delineato nel [PSR-0][psr0], che mira a provvedere una convenzione standard per file, classe e namespace per permettere di ottenere codice plug-and-play.

* [Leggi a proposito dei Namespace][namespaces]
* [Leggi a proposito del PSR-0][psr0]

[namespaces]: http://php.net/manual/en/language.namespaces.php
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
