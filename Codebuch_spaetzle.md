# Datensatz Spaetzle Connection

Codebuch Stand 2022-02 erstellt von Jessica Schreiner (js419@hdm-stuttgart.de)

# Inhalt

    edgelist_spaetzle.csv (Edgelist)
    nodelist_spaetzle.csv (Nodelist)
    Codebuch_spaetzle.md (Codierung der Datensätze)

# Ursprung und Datenerhebung

Im Fokus stehen Karrierenetzwerke und gegenseitige Beziehungen zwischenden baden-württembergischen Regierungsmitgliedern: welche biographischen
Muster sind besonders auffallend? Gibt es Karrierenetzwerke? 

Das Netzwerk ist ein two-mode Akteursnetzwerk. 

# EDGE-Attribute

id 
(identisch mit edgelist, aber hier nur einmalige Nennung)

from 
initiierender Knoten

to 
erhaltender Knoten

relationship 
Beziehungsart zwischen den Politiker:innen und zu den Organisationen/Ort/Verband etc.

1 = Achtung: Regierung umfasst auch Staatsekretäre und das
Bundeskanzleramt, etc. hier sollte als Knoten das entsprechende
Ministerium angegeben werden.

2 = aktuelle und ehemalige politische Funktionen in politischen
Ausschüssen, Gremien und der Partei. etc. Das kÃ¶nnen auch frÃ¼here
Stationen gewesen sein, z.B. GeschÃ¤ftsfÃ¼hrer:in einer Partei, etc.

3 = umfasst alle Mitgliedschaften in NGOs, Stiftungen, GedenkstÃ¤tten,
etc: werden im Bundestagsprofil als KÃ¶rperschaften Ã¶ffentlichen Rechts
bezeichnet.

4 = Beteiligung an Unternehmen durch Mandate, etwa Aufsichtsratsmandate,
Gremien, etc.

5 = erhalten Stipendien (egal wann), etwa Deutsche Studienstiftung,
Parteinahe Stiftungen, Internationale Organisationen im In- und Ausland
etc.

6 = ausgeÃ¼bte BerufstÃ¤tigkeiten, falls vorhanden

7 = Studien- bzw. (lÃ¤ngere) Aufenthaltsort(e) in In- und Ausland

year 
(Bezieht sich auf das Jahr, in dem die Variable relationship erhoben wurde)

# NODE-Attribute
id (identisch mit edgelist, aber hier nur einmalige Nennung),
name_short (Nachname)
name (voller Name)
type (0 = Person, 1 = Organisation/Ort/Verband etc.),
sex (Geschlecht)
birth (Geburtsjahr)
position (jetzige Position, z.B. StaatssekretÃ¤r:in, Minister)
education (hÃ¶chster Bildungsabschluss)
subject (Fachrichtung bei Studium/Promotion)
party (ParteizugehÃ¶rigkeit)
religion (Religion)
kids (Anzahl der Kinder)
twitter (Anzahl follower)
instagram (Anzahl follower)
facebook (Anzahl follower)
youtube (Anzahl Abonnenten)

id
Identische ID wie aus der edgelist zur Identifikation der Knoten. In diesem Fall sind alle personenbezogenen Daten anonymisiert von 1 bis 38.

name numerische ID

name_first Vorname abgekürzt, z.B. für Visualiserung, falls der Name zu lange ist

sex
Bitte geben Sie ihr Geschlecht an:
1 = weiblich
2 = männlich
3 = divers

crpr*
Welche Studienrichtung haben Sie vertieft?
1 = CR
2 = PR

height
Größe in cm

weight
Gewicht in kg

age_real
Alter in natürlichen Zahlen.

age
Bitte geben Sie Ihr Alter an:
1 = bis 20 Jahre
2 = 21 bis 22 Jahre
3 = 23 bis 24 Jahre
4 = 25 und älter

smoke
Rauchen Sie mindestens ein Mal pro Woche?
1 = nein
2 = ja

tatoo
Tatoo vorhanden?
1 = nein
2 = ja

phone
1 = android
2 = iOS/iphone

eyes
Welche Augenfarbe?
1 = grün,
2 = blau,
3 = braun,
4 = blau.

hair
Welche Haarfarbe?
1 = braun,
2 = schwarz,
3 = blond,
4 = rot.

location Wohnort, als string/characters codiert

county
Bundesland, als string/characters codiert
