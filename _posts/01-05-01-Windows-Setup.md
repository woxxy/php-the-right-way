---
isChild: true
---

## Setup Su Windows

PHP è disponibile in varie forme su Windows. Puoi [scaricare i binari](php-downloads) e fino a recente data è stato possibile usare un '.msi' installer. L'installer non è più supportato ed è stato terminato con PHP 5.3.0.

Per imparare e per sviluppare localmente puoi usare il webserver incluso in PHP 5.4 così non dovrai preoccuparti di configurarlo. Se vuoi un pacchetto "all-in-one" che comprenda un completo webserver e MySQL allora strumenti quali [Web Platform Installer][wpi], 
[Zend Server CE][zsce], [XAMPP][xampp] and [WAMP][wamp] ti aiuteranno a  un ambiente di sviluppo in breve tempo. Questo detto, questi strumenti saranno leggermente diversi da quelli in produzione quindi fai attenzione alle differenze tra gli ambienti se stai sviluppando su windows ed mettendo in produzione su Linux.

Se necessiti operare il tuo sistema di produzione su Windows, allora IIS7 ti darà le migliori performance e la migliore stabilità. Puoi usare [phpmanager][phpmanager] (un plugin GUI per IIS7) per rendere facile la configurazione e la gestione di PHP. Con IIS7 ha FastCGI integrato e pronto all'uso, devi solo configurare PHP come handler. Per supporto ed ulteriori risorse c'è [un'area dedicata su iis.net][php-iis] per PHP.

In genere avviare la tua applicazione in diversi ambienti in sviluppo ed in produzione può portare all'apparizione strani bug nel momento in cui si vada live. Se stai sviluppando su windows e mettendo in produzione si Linux (o su qualsiasi sistema non-Windows) allora dovresti considerare l'uso di una Macchina Virtuale. Questo può suonare complesso, ma usando [Vagrant][vagrant] puoi preparare semplici wrapper, e poi usare [Puppet][puppet] or [Chef][chef] per preparare queste istanze e distribuirle con i tuoi colleghi per assicurarti che stiate tutti lavorando sullo stesso stack. Altre informazioni a proposito di questo verranno presto aggiunte.

[php-downloads]: http://windows.php.net
[phpmanager]: http://phpmanager.codeplex.com/
[wpi]: http://www.microsoft.com/web/downloads/platform.aspx
[zsce]: http://www.zend.com/en/products/server-ce/
[xampp]: http://www.apachefriends.org/en/xampp.html
[wamp]: http://www.wampserver.com/
[php-iis]: http://php.iis.net/
[vagrant]: http://vagrantup.com/
[puppet]: http://www.puppetlabs.com/
[chef]: http://www.opscode.com/
