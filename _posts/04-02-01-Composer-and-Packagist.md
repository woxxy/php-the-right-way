---
isChild: true
---

## Composer e Packagist

Composer è un **brillante** gestore delle dipendenze per PHP. Crea una lista delle dipendenze del tuo progetto in un file chiamato `composer.json` e, in pochi comandi, Composer automaticamente scaricherà le dipendenze del tuo progetto e preparerà l'autoloading per te.

Ci sono già molte librerie PHP compatibili con Composer, pronte da essere usate nel tuo progetto. Questi "pacchetti" sono elencati su [Packagist][1], la repository ufficiale per le librerie PHP compatibili con Composer.

### Come Installare Composer

Puoi installare Composer localmente (nella tua directory di lavoro; tuttavia questo non è più raccomandato) o globalmente (ad esempio /usr/local/bin). Presumiamo che tu voglia installare Composer localmente. Dalla directory root del tuo progetto:

    curl -s http://getcomposer.org/installer | php

Questo scaricherà `composer.phar` (un archivio PHP binario). Puoi avviarlo con `php` per gestire le dipendenze del tuo progetto. <strong>Per favore tieni nota:</strong> Se fai pipe del contenuto scaricato direttamente nell'interprete, per favore per prima cosa leggi il codice online per confermare che sia sicuro.

### Come installare Composer (manualmente)

Installare Composer manualmente è una tecnica avanzata; in ogni caso, ci sono alcune motivazioni per cui uno sviluppatore possa preferire questo metodo in confronto ad usare la routine dell'installazione interattiva. L'installazione interattiva controlla la tua installazione PHP per rendere certo che:

- una versione di PHP sufficiente sia usata
- i file `.phar` possano essere eseguiti correttamente
- i permessi di certe directory siano sufficienti
- certe estensioni problematiche non siano caricate
- certi settaggi in `php.ini` siano settati

Siccome un'installazione manuale non esegue alcuno di questi controlli, devi decidere tu se ti conviene usare questo metodo. Quindi, quanto segue è come ottenere Composer manualmente:

    curl -s http://getcomposer.org/composer.phar -o $HOME/local/bin/composer
    chmod +x $HOME/local/bin/composer

La path `$HOME/local/bin` (o una directory a tua scelta) dovrebbe essere nella tua variabile d'ambiente `$PATH`. Questo renderà il comando `composer` disponibile.

Quando incontrerai documentazione che specifichi di avviare Composer con `php composer.phar install`, puoi sostituire questo con:

    composer install

### Come Definire ed Installare le Dipendenze

Prima di tutto, crea un file `composer.json` nella stessa directory di `composer.phar`. Ecco un esempio che elenca [Twig][2] come dipendenza ad un progetto.

	{
	    "require": {
	        "twig/twig": "1.8.*"
	    }
	}

In seguito, avvia questo comando dalla directory radice del tuo progetto.

    php composer.phar install
    
Questo scaricherà ed installerà le dipendenze del progetto in una directory `vendors/`. Poi, aggiungi questa linea al file PHP principale del tuo progetto; questo avviserà PHP di usare l'autoloader di Composer per le dipendenze del tuo progetto.

{% highlight php %}
<?php
require 'vendor/autoload.php';
{% endhighlight %}

Ora potrai usare le dipendenze del tuo progetto, che verranno caricate automaticamente sotto richiesta.

* [Scopri Composer][3]

[1]: http://packagist.org/
[2]: http://twig.sensiolabs.org
[3]: http://getcomposer.org/doc/00-intro.md
