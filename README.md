# Kaiserpfalz Homepage git

## Vorwort

Dieses Git beschreibt die Homepage der K.d.St.V. Kaiserpfalz, zumindest sollte es das.

## Inhalte anpassen

> Das hier ist der Teil für Chargen und Ämter

Der Text-Inhalt der Webseite liegt im `/content` Ordner und idealerweise sonst nirgends. Das ändern von Dateien in diesem Ordner *sollte* also nichts kaputt machen.

Jede Seite wird abgebildet durch eine `.md` Datei. Das Format heißt [Markdown](https://www.markdownguide.org/basic-syntax/) und ist wirklich stupide einfach zu lesen und zu verstehen\*. Das Problem an Hugo-Flavoured-Markdown ist das es signifikant mächtiger ist als das basisformat durch sogenannte "Shortcodes". Diese sind für den geneigten Texte-Pfuscher nicht von Bedeutung und erkennbar an den geschwungenen Klammern: `{{<imgsection src="images/bierjunge.jpg">}}`. An sich sollten die Dinger aber auch intuitiv nutzbar sein (wenn man kurz nachdenkt).

## Lokale Entwicklung

> Das hier ist der Teil für Nerds.

Der inhalt der Webseite liegt im `/content` Ordner und idealerweise sonst nirgends. Dadurch ist eine trennung von Inhalt und Layout gegeben aber das macht das anpassen vom Layout zunächst unintuitiver als der *ahem* klicki-bunti-Editor den z.B. Wordpress bereitstellt. Andererseits ist direkt code schreiben viel ausdrucksstärker und mächtiger (die Fußkanone ist groß, sei gewarnt). Um nun also die Webseite für änderungen lokal auf dem eigenen System zum laufen zu bekommen benötigt es einige wenige vorbedingungen:

* [Hugo](https://gohugo.io/) - Static site generator
* [Node.js](https://nodejs.org/en) - Für TailwindCSS dependency

durch das rezitieren das folgenden magischen Spruches entsteht ein lokaler dev-server (erreichtbar unter http://localhost:1313):
```sh
hugo server
```