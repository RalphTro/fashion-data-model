# GS1 Fashion Data model

Dieses Repository enthält alle notwendigen Informationen für die Modeindustrie um einen Datenaustausch im GS1 Fashion Datenmodell zu implementieren.

# Motivation

Die GS1 möchte den Teilnehmern in der Modeindustrie den Datenaustausch erleichtern. Schneller Produktionszyklen, eine größere Anzahl an Datenaustauschpartnern und die immer größere Wichtigkeit von Produktdaten in Zeiten des E-Commerce erfordern einen reibungslosen Datenaustausch. Durch die Vereinbarung eines Standards wird sichergestellt, dass innerhalb der Modeindustrie eine einheitliche "Sprache" gesprochen wird.
Der Fokus wurde auf eine einfache Verwendung und Implementierung gelegt, ebenso auf die Bedürfnisse der Internationalisierung und der damit verbundenen Mehrsprachigkeit der Daten.

# Inhalt

-   [Datenmodellbeschreibung als Excel](https://github.com/boernard/fashion-data-model/raw/master/Fashion%20data%20model_AT_DE_CH_V1_Pilot.xlsx)
-   [JSON Schema zur Validierung von JSON Nachrichten](https://raw.githubusercontent.com/boernard/fashion-data-model/master/fashionDataModelJsonSchema.json)
-   [JSON Beispiel Datensatz](https://raw.githubusercontent.com/boernard/fashion-data-model/master/fashionDataModel_example.json)
-   [Update fashion data model im Pilotprojekt](https://github.com/boernard/fashion-data-model/raw/master/Update%20fashion%20data%20model%20im%20Pilotprojekt.pdf)

Das vorliegende Syntax neutrale Excel Pilot Datenmodell ist in Zusammenarbeit mit den Unternehmen Ahlers Group, Hagemeyer, Zalando, KATAG, Falke und Fashion Cloud erstellt worden.

-   In Sope 1 der Umsetzung liegt die Konzentration auf die Attribute die Stand heute vom Datensender geliefert werden können.

-   In Sope 2-n ist eine Erweiterung um Attribute geplant die für Online benötigt werden.

-   Ziel ist es, dem Datensender einen Überblick über zukünftige Anforderungen zu geben, die er dann mit entsprechenden Zeitpuffer in seine internen Prozesse umsetzen kann.

### Das Excel Pilotdatenmodell ist wie folgt aufgebaut:

-   Es dient als Basis Information mit allen von der Branche bisher und zukünftig definierten Attribute

-   Filterung in Spalte M auf Scope 1 mit 59 Attributen für den Start in den elektronischen Datenaustausch

Da die Fashion Branche technologisch unabhängig sein möchte, haben wir versucht mehrere Kommunikationsstandards abzubilden, welches nun mit aktiven Piloten live getestet werden soll. Im Detail sind das:

-   Definition der Attribute die PRICAT übermittelt werden können (Spalte P-R)

-   Eine Beschreibung des Aufbaus der JSON Blaupause als Schema und eine Dokumentation wie daraus eine api Schnittstellenbeschreibung erstellt werden kann

-   Eine Dokumentation wie für diese 59 Attribute ebenfalls eine XML API Schnittstellenbeschreibung erstellt werden kann

### XML Schema Definiton

Das JSON Schema hilft bei der Erstellung von validen JSON Dokumenten im Fashion Data Model. Die Generierung eines XML Schemas (=XSD, XML Schema Definition) ist mit Hilfe von online Tools wie bspw. https://www.freeformatter.com/json-to-xml-converter.html mit geringem Aufwand möglich.
Hierfür würde man zunächst die JSON Beispiel-Datei online in XML konvertieren. Anschließend kann man aus dem XML eine XSD generieren, die dann mit den gültigen Wertebereichen aus dem JSON Schema befüllt werden muss.
