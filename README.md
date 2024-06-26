# LA1304-Zahlensystem

Sathana Suganthasri, Ava Hassani

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 28.02 | 0.0.1 | Projekt ausgewählt, Repository erstellt, repetiert wie man von Hexadezimal zu Dezimal rechnet, erste Anforderugnen erstellt |
| 06.03 | 0.0.2 | Anforderungen vollendet, Zahelnsysteme ausgewählt, |
| 27.03 | 0.0.3 | Projekt fertig programmiert. |
| 27.03 | 0.0.4 | Dokumentation fertig erstellt. |

## 1 Informieren

### 1.1 Ihr Projekt

Ein Programm mit welchem man verschiedene (benutzerunfreundliche) Zahlensysteme in (benutzerfreundliche) Dezimalzahlen, als auch zurück, rechnen kann. Folgende Zahlensystem verwenden wir um umzuwandeln:
Hexadezimal, Dezimal, Oktal und Binär.

### 1.2 Anforderungen

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1  | muss | funktional | Das Programm soll mit C# geschrieben werden. |
| 2  | muss | funktional | Der Benutzer muss Zahlen/Buchstaben eingeben können. |
| 3  | muss | funktional | Das Programm soll ein Ausgangsmenu haben, auf welchem der Benutzer die Übersetzungsrichtung des gewünschten Zahlensystems selektieren kann. |
| 4  | muss | funktional | Der Benutzer soll mit einem Button selektieren können und mit diesem auf ein weiteres Fenster landen, wo die Rechnung stattfindet.  |
| 5  | kann | funktional | Der Benutzer soll in der lage sein mit einem Button auf das Startmenu zurück laden zu können und von dort aus neu zu selektieren. |
| 6  | kann | qualität | Bei einer ungültigen Eingabe soll ein Fenster aufklappen, welches dies dem Benutzer sagt. |
| 7  | kann | qualität |  Der Benutzer soll mit dem Programm Hexadezimal zu Dezimal und vice versa umrechnen können.  |
| 8  | muss | funktional | Man soll von Oktal zu Dezimal und vice versa rechnen können.|
| 9  | muss | funktional | Man soll von Binär zu Dezimal und vice versa rechnen können.|
| 10 | muss | qualität |  Das Programm soll ein ansprechendes Design haben. |

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 2.1  | Fenster Hexadezimal --> Dezimal | a93b | 43323 |
| 3.1  | Menu | Button klicken auf Dezimal --> Hexadezimal | DH Fenstern |
| 3.2  | Menu | Button klicken auf Hexadezimal --> Dezimal | HD Fenster |
| 3.3  | Menu | Button klicken auf Dezimal --> Oktal | DO Fenster |
| 3.4  | Menu | Button klicken auf Oktal --> Dezimal | OD Fenster |
| 3.5  | Menu | Button klicken auf Dezimal --> Binär | DB Fenster |
| 3.6  | Menu | Button klicken auf Binär --> Dezimal | BD Fenster |
| 4.1  | Menu | Irgendwelche Button klicken | Fenster mit Rechnung |
| 5.1  | Rechnungsfenster von DH | "Zurück" Button klicken | Menu |
| 5.2  | Rechnungsfenster von HD | "Zurück" Button klicken | Menu |
| 5.3  | Rechnungsfenster von DO | "Zurück" Button klicken | Menu |
| 5.4  | Rechnungsfenster von OD | "Zurück" Button klicken | Menu |
| 5.5  | Rechnungsfenster von DB | "Zurück" Button klicken | Menu |
| 5.6  | Rechnungsfenster von BD | "Zurück" Button klicken | Menu |
| 6.1  | Rechnungsfenster von HD | dioj2o1 | Diese Eingabe enthält ungültige Zeichen! |
| 7.1  | Rechnungsfenster von HD | 4D2 | 1234 |
| 7.2  | Rechnungsfenster von DH | 1234 | 4D2 |
| 8.1  | Rechnungsfenster von DO | 1234 | 2322 |
| 8.2  | Rechnungsfenster von OD | 2322 | 1234 |
| 9.1  | Rechnungsfenster von BD | 11001 | 25 |
| 9.2  | Rechnungsfenster von DB | 25 | 11001 |

Abkürzungen:
DH = Dezimal --> Hexadezimal
HD = Hexadezimal --> Dezimal
DO = Dezimal --> Oktal
OD = Oktal --> Dezimal
DB = Dezimal --> Binär
BD = Binär --> Dezimal

### 1.4 Diagramme
vorstellung:
![image](https://github.com/Saadu02/LA1304-Zahlensystem/assets/111046257/bb481304-75b4-4e7b-a674-3ef3f1c1c9eb)
umrechnung:
![WhatsApp Bild 2024-02-28 um 11 17 45_b3453bfa](https://github.com/Saadu02/LA1304-Zahlensystem/assets/111046257/7417de29-673e-4452-b269-78ab32cf3bb7)


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 2.A  | 06.03.2024 | Sathana | Wörter einfügen | 20 min |
| 3.A  | 06.03.2024 | Ava | Menü | 2 x 45 min |
| 4.A  | 06.03.2024 | Ava | Button --> neues Fenster | 20 min |
| 5.A  | 06.03.2024 | Sathana | Button --> Menu Fenster | 35 min|
| 6.A  | 13.03.2024 | Sathana & Ava | Dialog Fehlermeldung | 30 min|
| 7.A  | 13.03.2024 | Sathana | Umrechnung Hexadezimal --> Dezimal | 2 x 45 min |
| 7.B  | 13.03.2024 | Sathana | Umrechnung Dezimal --> Hexadezimal | 2 x 45 min |
| 8.A  | 13.03.2024 | Sathana | Umrechnung Binär --> Dezimal | 2 x 45 min |      
| 8.B  | 13.03.2024 | Sathana | Umrechnung Dezimal --> Binär | 2x 45 min |
| 9.A  | 20.03.2024 | Ava | Umrechnung Oktal --> Dezimal | 2x 45 min |
| 9.B  | 20.03.2024 | Ava | Umrechnung Dezimal --> Oktal | 2x 45 min |
| 10.A | 27.03.2024 | Ava | Design | 45 min |

## 3 Entscheiden

Wir haben uns entschieden das Programm mit C# zu arbeiten. Danach haben uns wir uns entschieden das Zahlensystem Hexadezimal, Dezimal, Oktal und Binär zu verwenden. 

## 4 Realisieren


| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 2.A  | 06.03.2024 | Sathana | 20 min | 10 min |
| 3.A  | 06.03.2024 | Ava | 2 x 45 min | 2 x 45 min |
| 4.A  | 06.03.2024 | Ava | 35 min | 30 min |
| 5.A  | 06.03.2024 | Sathana | 30 min | 30 min |
| 6.A  | 13.03.2024 | Sathana & Ava | 2 x 45 min | 2 x 45 min |
| 7.A  | 13.03.2024 | Sathana | 2 x 45 min | 45 min |
| 7.B  | 13.03.2024 | Sathana | 2 x 45 min | 45 min |
| 8.A  | 20.03.2024 | Sathana | 2 x 45 min | 20 min |
| 8.B  | 20.03.2024 | Sathana | 2 x 45 min | 20 min |
| 9.A  | 20.03.2024 | Ava | 2 x 45 min | 25 min |
| 9.B  | 20.03.2024 | Ava | 2 x 45 min | 15 min |
| 10.A | 27.03.2024 | Ava | 45 min | 2 x 45 min |

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 2.1  | 20.03.2024 | OK | Sathana Suganthasri|
| 3.1  | 20.03.2024 | OK | Sathana Suganthasri|
| 3.2  | 20.03.2024 | OK | Sathana Suganthasri|
| 3.3  | 20.03.2024 | OK | Sathana Suganthasri|
| 3.4  | 20.03.2024 | OK | Sathana Suganthasri|
| 3.5  | 20.03.2024 | OK | Sathana Suganthasri|
| 3.6  | 20.03.2024 | OK | Sathana Suganthasri|
| 4.1  | 20.03.2024 | OK | Sathana Suganthasri|
| 5.1  | 20.03.2024 | OK | Sathana Suganthasri|
| 5.2  | 20.03.2024 | OK | Sathana Suganthasri|
| 5.3  | 20.03.2024 | OK | Ava Hassani |
| 5.4  | 20.03.2024 | OK | Ava Hassani |
| 5.5  | 20.03.2024 | OK | Ava Hassani |
| 5.6  | 20.03.2024 | OK | Ava Hassani |
| 6.1  | 20.03.2024 | OK | Ava Hassani |
| 7.1  | 20.03.2024 | OK | Ava Hassani |
| 7.2  | 20.03.2024 | OK | Ava Hassani |
| 8.1  | 20.03.2024 | OK | Ava Hassani |
| 8.2  | 20.03.2024 | OK | Ava Hassani |
| 9.1  | 20.03.2024 | OK | Ava Hassani |
| 9.2  | 20.03.2024 | OK | Ava Hassani |

Das Programm wurde auf einem HP Windows 11 Pro und Windows 11 Enterprise getestet. Alle Tests wurden bestanden.
