[![Stories in Ready](https://badge.waffle.io/meandor/projecttwomicroservice.png?label=ready&title=Ready)](https://waffle.io/meandor/projecttwomicroservice)
# projecttwomicroservice

[![Build Status](https://travis-ci.org/meandor/projecttwomicroservice.svg?branch=master)](https://travis-ci.org/meandor/projecttwomicroservice)

This microservice can add and maintain additional data to pbx provider and their products.

It is build on the [Edison Microservice](https://github.com/otto-de/edison-microservice) and uses AngularJS.

## Usage
This project uses gradle to build everything. There is a custom script to start the server, do all the testing and so on.

To run the microservice simply use the go script: ````./bin/go bootRun````.

To test everything run: ````./bin/go test````

## Experts
* frontend (Dustin Malte)
* backend (daniel, jana, rene, christof)
* api ()

## Fragenkatalog
* Wie sehen die Schnittstellen aus die wir von den anderen Systemen nutzen können?
    * Es gibt nur eine Schnitstelle die wir nutzen, nämlich die Login-Schnitstelle. Diese soll von uns gemockt werden. Ggf. bekommen wir im Laufe des Projektes Zugriff auf die echte Login-Schnitstelle.
* Wie soll die Schnitstellen aussehen die wir nach außen anbieten?
    * Die Schnittstelle soll in Absprache mit dem Kunden entwickelt werden, dazu sollen wir aber einen Entwurf vorlegen, den wir als Grundlage für diese Entwicklung nutzen können. Unsere Schnittstelle soll alle Daten über REST anbieten können, die wir auf der Anbieter Seite aufnehmen. Dabei ist es noch komplett frei wie wir diese Daten anbieten.
* Wie soll das GUI aussehen?
    * Keine Vorgaben vom Kunden
* Welche Daten sollen gespeichert werden?
    * Grundsätzlich sollen alle Daten gespeichert werden, welche der Anbieter auf unserer Microservices Seite eingeben kann:
    * Name
    * Kurzbeschreibung 
    * Lange Beschreibung
    * Hauptbild
    * Bilder-/PDF-Galerie Inhalte
    * Fakten-Tabelle
* Welche Formate sollen für Produktbroschüren und Bilder unterstützt werden?
    * PDF für Broschüren
    * mindestens JPG, PNG, GIF für die Bilder
* Wo finden wir die Schnittstellenbeschreibungen?
    * Bisher noch gar nicht, so lange sollen die Schnittstellen gemockt werden, ggf. werden die Beschreibungen nachgereicht.
* Welche Funktionen sollen zusätzlich abgedeckt werden?
    * Teaser und Name sollen in der Länge begrenzbar sein (config-file)
    * Für die Lange Beschreibung soll es möglich sein, den Text via Rich-Text Editor zu formatieren (je mehr Funktionen desto besser)
    * Eingabe in den Editor für Lange Texte soll kompatibel mit Word Copy&Paste sein
    * Bilder sollen beim Hochladen vom Kunden sortiert werden können

## Tools
* [Slack](https://projmicro.slack.com)
* [Waffle.io](https://waffle.io/meandor/projecttwomicroservice)
* IntelliJ
