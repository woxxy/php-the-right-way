# Guida dello Stile del Codice

La communità PHP è grande e variegata, composta di innumerevoli librerie, framework e componenti. E' abituale per gli sviluppatori PHP scegliere alcune di queste e combinarle nello stesso progetto. E' importante che il codice PHP aderisca (il più possibile) uno stile del codice comune per rendere facile per gli sviluppatori mischiare ed accoppiare varie librerie per i loro progetti.

Il [Framework Interop Group][fig] (precedentemente chiamato 'PHP Standards Group') ha proposto ed approvato una serie di raccomandazioni sullo stile, conosciute come [PSR-0][psr0], [PSR-1][psr1] e [PSR-2][psr2]. Non lasciare che i particolari nomi ti confondano, queste raccomandazioni sono solo una serie di regole che alcuni progetti come Drupal, Zend, CakePHP, phpBB, AWS SDK, FuelPHP, Lithium, etc stanno iniziando ad adottare. Puoi usarle per i tuoi progetti, oppure continuare ad usare il tuo stile personale.

Idealmente dovresti scrivere codice PHP che aderisca ad uno o più di questi standard in modo che altri sviluppatori possano leggere e lavorare il tuo codice con facilità. Questi si accumulano sulla raccomandazione precedente, quindi usare PSR-1 richiede PSR-0, ma non richiede PSR-2.

* [Leggi a proposito di PSR-0][psr0]
* [Leggi a proposito di PSR-1][psr1]
* [Leggi a proposito di PSR-2][psr2]

Puoi usare il [phpcs-psr][phpcs-psr] sniffer per [PHP_CodeSniffer][phpcs] per controllare del codice rispetto queste raccomandazioni. Usa il [PHP Coding Standards Fixer][phpcsfixer] di Fabien Potencier per modificare automaticamente la sintassi del codice in modo che sia conforme con questi standard, risparmiandoti dal sistemare ogni problema manualmente.

[fig]: http://www.php-fig.org/
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
[psr1]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md
[psr2]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md
[phpcs]: http://pear.php.net/package/PHP_CodeSniffer/
[phpcs-psr]: https://github.com/klaussilveira/phpcs-psr
[phpcsfixer]: http://cs.sensiolabs.org/
