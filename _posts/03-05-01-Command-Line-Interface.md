---
isChild: true
---

## Interfaccia a Riga di Comando

PHP è stato creato prima di tutto per scrivere applicazioni web, ma è anche utile per sviluppare programmi con interfaccia a riga di comando (Command Line Interface - CLI). I programmi a riga di comando in PHP possono aiutarti ad automatizzare mansioni quali testing, deployment ed amministrazione dell'applicazione.

I programmi CLI PHP sono potenti perché puoi usare il codice della tua applicazione direttamente senza dover creare una GUI web sicura. Accertati solo di non mettere i tuoi script CLI PHP nella cartella web pubblica!

Prova ad avviare PHP dalla tua riga di comando:

{% highlight bash %}
> php -i
{% endhighlight %}

L'opzione `-i` stamperà a schermo la tua configurazione PHP come farebbe la funzione [`phpinfo`][phpinfo].

L'opzione `-a` fornisce una shell interattiva, simile all'IRB di ruby o alla shell interattiva di python. C'è un certo numero di altre utili [opzioni da riga di comando][cli-options].

Scriviamo una semplice applicazione CLI "Hello, $name". Per provarla, crea un file e chiamalo `hello.php` come specificato sotto.

{% highlight php %}
<?php
if($argc != 2) {
    echo "Usage: php hello.php [name].\n";
    exit(1);
}
$name = $argv[1];
echo "Hello, $name\n";
{% endhighlight %}

PHP setta due speciali variabili basate sugli argomenti con cui il tuo script è stato avviato. [`$argc`][argc] è una variabile integer che contiene il *conto* degli argomenti e [`$argv`][argv] è una variabile array che contiene i *valori* di ciascun argomento. Il primo argomento è sempre il nome del file dello script PHP, in questo caso `hellp.php`.

L'espressione `exit()` è usata con un numero diverso da zero per rendere noto alla shell che il comando è fallito. I codici di uscita comuni possono essere trovati [qui][exit-codes].

Per avviare il nostro script in alto, dalla riga di comando:

{% highlight bash %}
> php hello.php
Usage: php hello.php [name]
> php hello.php world
Hello, world
{% endhighlight %}


 * [Altre informazioni sull'avviare PHP dalla riga di comando][php-cli]
 * [Altre informazioni sul settare Windows per avviare PHP dalla riga di comando][php-cli-windows]

[phpinfo]: http://php.net/manual/en/function.phpinfo.php
[cli-options]: http://www.php.net/manual/en/features.commandline.options.php
[argc]: http://php.net/manual/en/reserved.variables.argc.php
[argv]: http://php.net/manual/en/reserved.variables.argv.php
[php-cli]: http://php.net/manual/en/features.commandline.php
[php-cli-windows]: http://www.php.net/manual/en/install.windows.commandline.php
[exit-codes]: http://www.gsp.com/cgi-bin/man.cgi?section=3&topic=sysexits