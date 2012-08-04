---
isChild: true
---

## Paradigmi di Programmazione

PHP è un linguaggio di programmazione dinamica flessibile, che supporta una varietà di tecniche di programmazione. Si è evoluto drammaticamente nel corso degli anni, in mod notabile aggiungendo un solido modello orientato ad oggetti in PHP 5.0 (2004), funzioni anonime e namespace in PHP 5.3 (2009), e trait in PHP 5.4 (2012).

## Programmazione Orientata ad Oggetti

PHP ha un insieme molto completo di funzionalità di programmazione ad oggetti compreso il supporto per classi, classi astratte, interfacce, ereditarietà, costruttori, cloning, eccezzioni, ed altro.

* [Leggi a proposito di PHP Orientato ad Oggetti][oop]
* [Leggi a proposito dei Traits][traits]

### Programmazione Funzionale

PHP supporta funzioni di prima classe, il che vuol dire che una funzione può essere assegnate ad una variabile. Sia le funzioni definite dall'utente che quelle integrate possono essere assegnate ad una variabile ed essere invocate in maniera dinamica. Le funzioni possono essere passate come argomenti ad altre funzioni (funzionalità chiamata Higher-order functions) e le funzioni possono ritornare altre funzioni.

La ricorsione, una funzionalità che permette ad una funzione di chiamare se stessa, è supportata dal linguaggio, ma la maggior parte del codice PHP si concentra sulle iterazioni.

Le nuove funzioni anonime (con supporto per closures) è presente da PHP 5.3 (2009).

PHP 5.4 ha aggiunto la possibilità di legare closures all'ambito dell'oggetto ed ha anche migliorato il supporto per i callables in modo che possano essere usate intercambiabilmente con funzioni anonime in quasi ogni caso.

* Continua la lettura sul [Functional Programming in PHP](pages/Functional-Programming.html)
* [Leggi a proposito delle Funzioni Anonime][anonymous-functions]
* [Leggi a proposito della classe Closure][closure-class]
* [Altri dettagli sulla RFC delle Closures][closures-rfc]
* [Leggi a proposito dei Callables][callables]
* [Leggi a proposito di chiamare dinamicamente funzioni con `call_user_func_array`][call-user-func-array]

### Programmazione Meta

PHP supporta varie forme di meta programming attraverso meccanismi come la Reflection API ed i Magic Methods. Ci sono molti Magic Methods disponibili quali `__get()`, `__set()`, `__clone()`, `__toString()`, `__invoke()`, etc. che permettono agli sviluppatori di agganciarsi al comportamento della classe. Gli sviluppatori Ruby spesso dicono che PHP non ha disponibile `method_missing`, ma è disponibile con `__call()` e `__callStatic()`.

* [Leggi a proposito dei Magic Methods][magic-methods]
* [Leggi a proposito di Reflection][reflection]

[namespaces]: http://php.net/manual/en/language.namespaces.php
[overloading]: http://uk.php.net/manual/en/language.oop5.overloading.php
[oop]: http://www.php.net/manual/en/language.oop5.php
[anonymous-functions]: http://www.php.net/manual/en/functions.anonymous.php
[closure-class]: http://php.net/manual/en/class.closure.php
[callables]: http://php.net/manual/en/language.types.callable.php
[magic-methods]: http://php.net/manual/en/language.oop5.magic.php
[reflection]: http://www.php.net/manual/en/intro.reflection.php
[traits]: http://www.php.net/traits
[call-user-func-array]: http://php.net/manual/en/function.call-user-func-array.php
[closures-rfc]: https://wiki.php.net/rfc/closures
