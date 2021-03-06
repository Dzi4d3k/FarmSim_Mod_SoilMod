﻿

NOTICE! NOTICE!
  This translated German text have NOT YET been updated to v2.2.x
NOTICE! NOTICE!




SoilMod – Soil Management & Growth Control (v2.0.x)

SoilMod v2.0.x - Anleitung auf Deutsch

Denke daran, das Support-Topic für zusätzliche Informationen bezüglich dieser Mod zu nutzen.

Changelog
V2.0.x
- Upgrade auf LS15 und einige wenige Veränderungen
- doppelte Auflösung der Boden-pH-Stufen
- bisherige Düngerkonzeption zu N- und PK-Versorgung verändert
- weitere Herbizidtypen hinzugefügt, um  der Unkrautkeimung vorzubeugen (für +3 Tage)
- Bodenfeuchtigkeit hinzugefügt, das heißt Wasser beeinflusst nun die Ernteerträge
- Vollständig ausgewachsenes Unkraut verwelkt, wenn die gesamte N-Versorgung im Umfeld aufgebraucht wurde
- Wechsel zwischen den Spritztypen ist eingeschränkt und funktioniert nur, wenn man sich mit einer Spritze in der Nähe eines Düngertanks (oder einem ähnlichen Befülltrigger) befindet.
- Übersetzungen von DD ModPassion, Gonimy_Vetrom, Iscarriah, mngrazy, Ziuta.

(Anm.: Auf den folgenden Seiten tauchen Begriffe und Abkürzungen auf, die viele nicht kennen und damit wenig bis gar nichts anfangen können. Deshalb möchte ich an dieser Stelle Grundlegendes zu den Themen Düngung, Herbizid und pH-Wert erklären. Möglicherweise ist es für den einen oder anderen dann leichter nachzuvollziehen, wie und warum Decker diese Mod so erstellt hat.
Zunächst einmal gibt es zwei Arten von Düngern, organischen, also natürlichen  Dünger, der von den Tieren oder aus Biogasanlagen stammt, und synthetischen Dünger, sprich Kunstdünger. Organischer Dünger wird nochmals unterschieden in Festmist (das, was wir als „normalen“ Mist kennen) und Flüssigmist (Gülle von den Tieren und Gärrest aus der Biogasanlage). In beiden Düngerarten (organisch und synthetisch) sind unter anderem die Nährstoffe Stickstoff (N), Phosphor (P) und Kalium (K) enthalten. Im Kunstdünger kommen diese Nährstoffe in einer höheren Konzentration vor als im organischen Dünger und sind zudem auch meist schnelllöslich.
Herbizide sind Mittel gegen Unkräuter und Ungräser. Sie werden unterschieden nach:
- Kontaktherbiziden: zerstören das Chlorophyll in den Pflanzen
- Wuchsstoffe: führen zu einem übersteigerten Wachstum der Unkräuter
- Breitbandherbizide: sind Kombinationen aus den oben genannten Arten
- Sylfonylharnstoffe: sie blockieren den Eiweißaufbau in der Pflanze
- Bodenherbizide: hierbei erfolgt die Wirkstoffaufnahme über die Wurzel bzw. auch über das Blatt einer Pflanze
Welche Herbizidart nun in der SoilMod verwendet wird, ist hierbei weniger von Bedeutung. Wichtig ist, dass man weiß, dass bestimmte Feldfrüchte nur bestimmte Herbizide vertragen. Bei falscher Anwendung können Feldfrüchte in ihrem Wachstum gehemmt werden oder im schlimmsten Fall absterben.
Zum pH-Wert. Ich versuche es mal kurz und einfach zu erklären. Der pH-Wert gibt die Menge an Wasserstoff-Ionen an, die sich in einem Liter Flüssigkeit befinden. Je größer die Menge der Wasserstoff-Ionen in einer Flüssigkeit ist, desto größer ist ihr Gewicht und desto kleiner ist ihr Wert. Die pH-Werte reichen von 1 (sehr sauer) über 7 (neutral) bis 14 (sehr alkalisch). Der pH-Wert ist für Böden von sehr großer Bedeutung. Ein Absinken des pH-Wertes (Versauerung) sorgt für eine Abnahme der biologischen Aktivität. Eine Düngung mit Kalk sorgt für ein Anheben des pH-Wertes.
Nun hoffe ich, euch mit der kleinen Einführung nicht überfordert zu haben. Ich wollte euch lediglich einen kleinen Einblick in die reale Landwirtschaft geben. Die SoilMod an sich ist für den LS eine wunderbare Sache, da noch mehr Realismus dazukommt. Endlich macht es Sinn, Dünger und Kalk zu streuen, Spritzmittel auszubringen, zu pflügen und noch mehr vom Wetter abhängig zu sein!)


Modbeschreibung

Die SoilMod ist eine Mod für Maps, die, wenn sie richtig vorbereitet worden sind, folgendes hinzufügt:
- individuelle Steuerung des Wachstums, das der Ingame-Zeit folgt
- eine sinnvolle Verwendung von Kalk, da die Boden-PH-Werte nun eingefügt sind
- Organische Dünger (Gülle, Mist, Gärrest) müssen in den Boden eingearbeitet (Pflug, Grubber) werden, um ihre Wirkung entfalten zu können
- automatische Ausbreitung von Unkraut und Nutzung von Herbiziden
- und weitere Effekte.

BITTE BEACHTE: Diese Mod vermag möglicherweise nicht die Erwartungen zu erfüllen, die an sie gestellt werden. Bitte sei offen, äußere konstruktive Kritik und/oder mach Vorschläge, wie zukünftige Versionen verbessert werden können. 


Vorbereiten der Map – WICHTIGE INFORMATION! – 

Die „SoilManagement.ZIP“-Mod wird NUR auf Maps funktionieren, die darauf ausgelegt sind. Es sind bestimmte Ergänzungen in der „map.I3D“-File erforderlich. Diese befinden sich in der ZIP-File selbst, im Order „Requirements_for_your_MapI3D“ .

Die Benutzung eines Editors, wie Notepad++ oder ähnlichen Programmen, sowie das Zurechtfinden in XML-Textfiles wie der „.I3d-File“ werden vorausgesetzt.


Vorbereiten der Map.I3D für die SoilMod

Bitte lies dir die File „Map_Instructions.txt“ befindlich im Modordner „Requirements_for_your_MapI3D“ der ZIP-File sorgfältig durch. Jene Textfile enthält die Grundlagen, die der eigenen Map.i3D-File zugefügt werden müssen.

Vergiss nicht, vor jeder Änderung der eigenen Map ein Backup davon zu machen. Sollte etwas schief gelaufen sein, kann jederzeit auf die letzte funktionierende Version zurückgegriffen und ein neuer Versuch unternommen werden.
Stell sicher, dass die normale Größe der Map „x1“ ist (das heißt Density Files von 4096 x 4096 Pixeln). Sollte die Map eine andere Größe besitzen, muss auch die Größe der beiden Layer-Files verändert werden!
(Anmerkung: Bis jetzt sind keine Veränderungen der „SampleModMap.LUA“-File erforderlich -  die Anleitungen für die SoilMod v1.0.x funktionieren für die v2.x nicht!)


Verwenden der SoilMod in-game – WICHTIGE INFORMATIONEN FÜR SPIELER –

ACHTUNG: Da es viele andere Mods gibt, die die internen Funktionen Spritzen/Streuen/Bodenbearbeitung/ Ernten im Landwirtschaftssimulator erweitern, kann es zu Konflikten zwischen jenen Mods und der SoilMod kommen.

Es ist überaus ratsam, jegliche Mods und Modmaps zu entfernen oder zu deaktivieren, die möglicherweise den ordnungsgemäßen Betrieb der SoilMod beeinflussen können.

(Anm.: Bei Benutzung der SoilMod muss z.B. die Gülle-Mist-Kalk-Mod aus dem Modordner genommen werden.)

Wenn die Map richtig für die SoilMod vorbereitet und die „SoilManagement.ZIP“ im Modordner abgelegt wurde, ist die SoilMod in-game nutzbar.

Starte das Spiel und anschließend die Map, die nun für die SoilMod ausgelegt ist. Merke: Es ist durchaus möglich, ein bereits bestehendes Savegame fortzuführen. Allerdings sollte zuerst ausprobiert werden, ob dies auch wirklich funktioniert.

Während die Map lädt, tragen die SoilMod-Skripte verschiedene Informationen in die In-game-Konsole und die „Log.TXT“-File ein. Im Falle eines Problems kann letztere genutzt, um herauszufinden welches Problem aufgetreten ist. Tauchen Probleme in Verbindung mit der SoilMod auf, werden diese dort deutlich angezeigt. 

ACHTUNG: Da die SoilMod 8 (oder 9) neue Spritz-/Befülltypen hinzufügt (einige andere Mods erkennen diese als Fruchttypen, nutzen sie jedoch nicht als solche), kann es Probleme mit der „max 64 fill-types“-Einschränkung des Grundspiels geben. Bitte überprüfe mehrmals die „LOG.TXT“-File auf Warnings/Errors.


Panel zeigt die Bodenbedingungen der momentanen Umgebung an

In der unteren rechten Ecke über dem Panel mit den Fahrzeugdaten zeigt die SoilMod ein Panel an, welches Informationen über den Boden enthält. Die Informationen beziehen sich jedoch nur auf ein 10 x 10 Quadratmeter großes Feld, das die aktuelle Position des Spielers umgibt. Sie werden im Sekundentakt aktualisiert.

Durch Drücken und Halten der „SoilMod: Toggle grid overlay“-Aktion kann das Panel ein- und ausgeschaltet werden (Standardtasten: links Alt + I gedrückt halten)


Grid Heads Up Display

Manchmal ist eine bessere Darstellung der versteckten Eigenschaften einer Umgebung nützlich. Die SoilMod enthält nun ein einfaches „Grid Display“, welches mit farblichen und der Größe angepassten Punkten versehen ist. Diese Punkte stellen die vier folgenden Eigenschaften dar: Boden-pH-Wert, Bodenfeuchtigkeit, N-Versorgung und PK-Versorgung.

Das „Grid Display“ wird mithilfe der „SoilMod: Toggle grid overlay“-Aktion durchgeschaltet (Standardtasten: links Alt + I).

Das SoilMod-Panel zeigt in fettgedruckter Schrift, welche der vier Eigenschaften durch das Grid momentan angezeigt werden.


Das Wachstum, Verwelken inbegriffen, vollzieht sich um Mitternacht an jedem In-game-Tag

Der eigentliche Grund, warum ich diesen Mod erstellt habe (dies reicht zurück bis zu LS 2013), war für mich herauszufinden, wann sich der nächste Wachstumszyklus vollzieht, um in der Lage zu sein, diesen in bestimmter Weise noch zu beeinflussen, obwohl er bereits abgeschlossen war.

Momentan ist es so, dass das Wachstum sämtlicher Früchte in-game jeden Tag um Mitternacht beginnt. Wenn gewünscht, kann dies in der „CareerSavegame.XML“-File des dementsprechenden Savegames geändert werden. Suche hierfür den Abschnitt „fmcSoilMod“.

Eine Verlaufsanzeige bildet den Fortschritt ab, da die „growth update stage“ eine der Größe nach festgelegte Fläche der Map beeinflusst. Dadurch sollen möglichst ein Einfrieren des Spiels sowie Lags minimiert werden.

ACHTUNG: Verwelken ist aktiviert! Wenn das ein Problem sein sollte, spiele auf der langsamsten Zeitstufe und/oder plane genügend Zeit mit ein.

Während des Wachstumszyklus passiert folgendes:
- Früchte (und Unkräuter) wachsen um eine Stufe, sofern das Wachstum nicht durch einen bestimmten Herbizidtyp beeinflusst wird, der entweder das Wachstum unterbricht oder die Früchte verwelken lässt.
- N- und PK-Versorgung sowie Feuchtigkeit werden zu unterschiedlichen Wachstumsstufen verbraucht.
- Schwaden und nicht eingearbeiteter Dünger werden um eine Stufe reduziert (das heißt sie werden langsam aufgelöst).
- Nicht eingearbeiteter Kalk sowie Gülle ziehen langsam in den Boden ein, sind aber vermindert wirksam, wenn sie nicht eingearbeitet werden.
- Kunstdünger erhöht die Versorgungsstufen
- Unkräuter verwelken nach Behandlung mit Herbiziden
- Das vom Spritzen/Düngen abgegebene Wasser erhöht die Feuchtigkeitsstufe im Boden.


Grundlegende Arbeitsabläufe zur Felderpflege

Überprüfe regelmäßig, ob die Felder einen Bedarf an N- und/oder PK-Versorgung sowie Feuchtigkeit benötigen bzw. ob der pH-Wert erhöht werden muss.

Wenn folgende Beobachtungen gemacht wurden, schaffen diese Aufgaben Abhilfe:
- Bei niedriger N-Versorgung: Ausbringen von Flüssigmist (Gülle, Gärrest) oder Kunstdünger NPK oder N, Ausbringen und Einarbeiten (Pflügen/ Grubbern) von Festmist.
- Bei niedriger PK-Versorgung: Ausbringen von Kunstdünger NPK oder PK, Ausbringen und Einarbeiten (Pflügen/ Grubbern) von Festmist.
- Bei wenig Feuchtigkeit: Ausbringen von Wasser und/oder Flüssigdünger (organisch, Kunstdünger) und/ oder Herbiziden (alle Arten möglich) oder auf Regen warten
- Bei niedrigem Boden-pH-Wert: Ausbringen von Kalk
- Bei Auftauchen von Unkräutern: Spritzen von Herbizid (Achtung: nur die Arten verwenden, die die Früchte vertragen) oder Pflügen/ Grubbern.

Warte nun den nächsten Wachstumszyklus ab und wiederhole die Punkte gegebenenfalls.


Boden-pH-Wert und Kalk beeinflussen die Ernteerträge

Die Bodenbedingung bezüglich des pH-Wertes stellt einen neuen Aspekt dieser Mod dar (ausgenommen für diejenigen, die dies bereits kennen). Wenn der Boden zu sauer ist, hat dies erhebliche Ernteeinbußen zur Folge.

Das SoilMod Panel zeigt den durchschnittlichen Boden-pH-Wert der momentanen Umgebung an, NICHT vom gesamten Feld. Behalte es im Auge!

Für optimale Erträge muss der Boden-pH-Wert innerhalb des neutralen Bereichs liegen. Jegliche Werte darunter oder darüber beeinflussen die Erträge, siehe die folgenden Werte. 100% steht für normale Erträge:

5.4 = 20%
5.6 = 70%
5.8 = 80%
6.2 = 90%
6.8 = 100%
7.5 = 90%
8.1 = 80%
8.5 = 50%

(Anm.: Den Werten kann man entnehmen, dass sich die pH-Werte zwischen 6.8 und 7.4 befinden sollten, um 100%ige Erträge zu bekommen. Je saurer der Boden, desto weniger Ertrag. Die Ertragseinbußen sind im alkalischen Bereich dagegen etwas geringer.)

Ausbringen von Kalk erhöht den Boden-pH-Wert. Wird dieser in den Boden eingearbeitet (Pflug/Grubber), ist er wirksamer als wenn er unverarbeitet zum nächsten Wachstumszyklus auf dem Feld verbleibt.

Aufgrund der technischen Begrenzungen des Spiels und der Art, wie das Skript arbeitet, können die pH-Werte stärker hin- und herspringen, als dies in der Realität der Fall ist.

Bei Gebrauch der Standardmaschinen zum Ausbringen von Dünger (Festmist ausgeschlossen) ist es möglich, den Ausbringtyp auf Kalk umzustellen. Die F1-Hilfebox zeigt an, welche Taste hierfür gedrückt werden muss. Achte darauf, dass du dich mit deiner Maschine in der Nähe eines Düngerlagers befindest, um diese Funktion nutzen zu können.


Wasser, Sonne und Regen

Die Bodenfeuchtigkeit wird von Wasser und Wärme beeinflusst.

Wenn Flüssigmist (Gülle, Gärrest), Flüssigdünger oder Herbizid ausgebracht wird, steigert dies die Bodenfeuchtigkeit während des nächtlichen Wachstumszyklus geringfügig. Es gibt zudem die Möglichkeit, Wasser auszubringen.

Schlechtes Wetter, also Regen, erhöht die Bodenfeuchtigkeit ebenfalls. Dies geschieht sofort zu jeder Stunde.
Gutes Wetter, das heißt Temperaturen über 22 Grad, senkt die Bodenfeuchtigkeit um zwölf Uhr mittags.

Während der Ernte beeinflusst die Bodenfeuchtigkeit die Erträge. Siehe dazu folgende Werte:

Feuchtigkeit  --> Ertragserwartung
0%  --> 50%
14%  --> 70%
57%  --> 100%
100%  --> 70%


Fest- und Flüssigmist

Einige Spieler haben sich dahingehend geäußert, lieber zuerst Fest-/Flüssigmist auszubringen und anschließend  mittels Pflug oder Grubber in den Boden einzuarbeiten.

Dies führt nun auch die SoilMod ein. Das Ausbringen von Fest- und Flüssigmist wird die gewünschte Wirkung erst erzielen, wenn diese  „in den Boden gemischt“ werden. Somit wird der Boden besser mit Nährstoffen versorgt und die Erträge während der Ernte gesteigert.

Die Schritte bei der Nutzung von Fest- und Flüssigmist in der SoilMod sehen wie folgt aus:

1. Ausbringen von Fest- oder Flüssigmist auf dem Feld.
2. a) Um die besten Ergebnisse zu erhalten, muss Festmist mit dem Pflug eingearbeitet werden. Diese Variante steigert die N- und PK-Versorgung am stärksten.
2. b) Festmist mit dem Grubber einzuarbeiten ist weniger wirkungsvoll.
3. Bei Flüssigmist macht es keinen Unterschied, ob dieser eingearbeitet wird oder unverarbeitet auf dem Feld verbleibt. Flüssigmist wird die N- und PK-Versorgung erst zum nächsten Wachstumszyklus steigern.

Merke: Festmist, der unverarbeitet auf dem Feld verbleibt, löst sich innerhalb von 3 Tagen auf und wird in diesem Fall die Versorgung mit N und PK NICHT steigern.


Dünger

Es gibt 3 Arten  von Düngern, sowohl in fester als auch in flüssiger Form:

- NPK (3-1-1)
- PK (0-3-3)
- N (5-0-0) (Dieser Typ senkt gleichzeitig den Boden-pH-Wert)

(Anm.: Bei NPK handelt es sich um einen Volldünger, das heißt alle drei Nährstoffe sind enthalten. Die jeweiligen Anteile sind im LS unterschiedlich, können in der Realität aber auch gleich sein, beispielsweise gibt es NPK 15/15/15. Hierbei ist jeder Nährstoff zu jeweils 15% enthalten. Bei PK bringt man nur Phosphor und Kalium aus, bei N nur reinen Stickstoff.)

(Merke: Die Werte sind willkürliche In-game-Angaben und basieren NICHT auf realen Werten.)
Bei Gebrauch der Standardmaschinen zum Ausbringen von Dünger (Flüssigmist ausgeschlossen) ist es möglich, den Ausbringtyp auf jede Düngerart umzustellen. Die F1-Hilfebox zeigt an, welche Taste hierfür gedrückt werden muss. Achte darauf, dass du dich mit deiner Maschine in der Nähe eines Düngerlagers befindest, um diese Funktion nutzen zu können.


Nährstoffversorgung beeinflusst die Erträge

Aufgrund technischer Gründe, die vielleicht seltsam/unrealistisch erscheinen, ist es die verbleibende Nährstoffversorgung während der Ernte, die die Ertragssteigerungen festlegt.

Die Ertragserwartung ausgehend von der N-Versorgung:
x0 = +0%
x1 = +20%
x2 = +50%
x3 = +70%
x4 = +90%
x5 = +100%
x10 = +75%
x15 = +50%

Die Ertragserwartung ausgehend von der PK-Versorgung:
x0 = +0%
x1 = +10%
x2 = +30%
x3 = +80%
x4 = +100%
x7 = +30%

In anderen Worten bedeutet dies, es sollte versucht werden, die Bodenstufen „N x5“ und „PK x4“ zu erreichen, um die besten Ertragssteigerungen während der Ernte zu haben.

(Für zukünftige Versionen: Diese Werte können an die unterschiedlichen Fruchttypen angepasst werden. Allerdings gibt es dies momentan NICHT in der v2.0.x)


Unkräuter und Herbizid – jene tauchen willkürlich auf dem Feld auf

Stellen mit Unkräutern werden ständig auf Feldern auftauchen, da ihre Samen durch Wind verteilt werden. Pflügen, Grubbern oder Säen entfernen sie. Manchmal sind diese Methoden aber nicht möglich, folglich muss Herbizid gespritzt werden.

Die SoilMod besitzt 3 + 3 Herbizidarten: A, B und C sowie AA, BB und CC. Jedes dieser Herbizide tötet Unkräuter ab. Allerdings gibt es einige Früchte, die nur bestimmte Herbizidarten vertragen. Im schlimmsten Fall können Früchte verwelken, wenn sie der falschen Herbizidart ausgesetzt werden.

Gegenwärtig gelten diese Regelungen für Herbizide und Fruchtarten:
- Herbizid B oder C kann angewendet werden bei: Weizen, Gerste, Roggen, Hafer und Reis. 
(Verwende nicht Typ A)
- Herbizid A oder C kann angewendet werden bei: Mais, Raps, OSR, Luzerne, Klee. (Verwende nicht Typ B)
- Herbizid A oder B kann angewendet werden bei: Kartoffeln, Rüben, Sojabohnen, Sonnenblumen.
(Verwende nicht Typ C)

Wenn Unkräuter mit Herbizid behandelt worden sind, verwelken sie und sterben nach einigen Tagen ab. Allerdings können in der Zwischenzeit wieder neue Unkräuter gewachsen sein, es sei denn, Herbizide mit „doppelter Wirkung“ (AA, BB oder CC) sind vorher gespritzt worden. Diese Herbizide verhindern ein Ausbreiten und Keimen von Unkräutern für weitere 3 Tage.

Bei Gebrauch der Standardmaschinen zum Ausbringen von Spritzmitteln (Flüssigmist ausgeschlossen) ist es möglich, den Ausbringtyp auf jede der drei Herbizidarten umzustellen. Die F1-Hilfebox zeigt an, welche Taste hierfür gedrückt werden muss.


Während des Wachstumszyklus

Folgende Effekte/Veränderungen treten während des Wachstumszyklus auf:
- Während die Früchte die Wachstumsstadien 1 – 7 durchlaufen, verbrauchen sie pro Stadium „1N“.
- Wenn sich die Früchte in den Stadien 3 und 5 befinden, verbrauchen sie je „1 PK“.
- Wenn sich die Früchte in den Stadien 2, 3 und 5 befinden, nimmt die Bodenfeuchtigkeit um eine Stufe ab.
- Wenn sich die Früchte im Stadium 3 befinden, nimmt der Boden-pH-Wert um eine Stufe ab.
- Voll ausgewachsene Unkräuter verwelken, wenn der gesamte N im Boden aufgebraucht ist.
- Schwaden/Mist verringert die Menge um 1.


Probleme oder Bugs?

Solltest du bei der Benutzung der SoilMod auf Probleme oder Bugs stoßen, verwende bitte den Support-Thread http://fs-uk.com.  Suche die Mod (und die korrekte Version) im Bereich „Mods“, in der Kategorie „Other – Game Scripts“.


Bekannte Fehler/Bugs:
- Das Spritzen/Streuen eines Dünger-/Herbizidtyps auf dem Feld, ersetzt jeden anderen Dünger-/Herbizidtyp, der sich möglicherweise bereits auf dem Feld befindet.
- Das Wiederbefüllen eines Streuers/einer Spritze stellt diese wieder auf Dünger NPK um, wenn das standardmäßige Dünger-/Spritzmittellager verwendet wird. Abhilfe schaffen hier mehrere Tanks/Lager, sofern der Map-Ersteller diese einbaut, und zwar jeweils für Dünger, für Herbizid und für Kalk.


Quelle: http://fs-uk.com/mods/view/36108/soilmod-soil-management-growth-control-v2-0-x
Version: v2.0.x
geschrieben von: Decker_MMIV
übersetzt von: Beowulf
