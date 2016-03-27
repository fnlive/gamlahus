
Gamla Hus
=========

Denna webb-applikation är utvecklad av Fredrik Nilsson som del i ett kursmoment i kursen ["phpmvc - Databasdrivna webbappl med PHP och MVC"](http://dbwebb.se/phpmvc/).

Applikationen är en stackoverflow-lik Q&A-site fast med Gamla Hus som ämnesområde.

Installation
------------

Ladda ner zip-fil och kopiera den till en folder under apaches web-root folder.

Uppdatera RewriteBase i .htaccess filen enligt din installation.

Gör följande foldrar skrivbara för webbservern:
* webroot/ (så att webbservern kan skriva till databasfilen .htsqlite.db)
* webroot/css/anax-grid/ (så att webbservern kan skapa en .less-fil)

Vid behov, ändra sökväg till databafilen genom att uppdatera filen app/config/database_sqlite.php.

Validera composer.json fil genom att köra följande kommando i web-root folder:

    composer validate

Installera 3dje-parts moduler från Packagist med följande kommando:

    composer install

Peka din webb-läsare till url "web-root"/webroot/index.php/admin/setup för att initiera databas med testdata.

Nu är installationen komplett. Du kan logga in med användare admin, password admin.
