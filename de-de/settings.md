Über die Sidebar "Settings" können verschiedene Einstellungen für den Host und Matrix getätigt werden. Im Folgenden werden alle Möglichkeiten erklärt:

## Host
###  Basic Settings 

**Boot Animation**  
Zeigt beim ersten Verbindungsaufbau der Matrix eine Bootanimation an.
Diese nutzt die Draw API. Die bootanimation.json befindet sich im Ordner "config" und kann beliebig verändert werden.

**Switch Animation**  
Die aktiviert eine Wechselanimation zwischen den Apps. Hierbei wird die alte App heruntergedimmt und die neue hochgedimmt.

**Color Switch**  
Eine andere Form der Wechselanimation. Hier löscht ein farbiger Balken die aktive App von der Matrix.

**Uppercase Letters**  
Diese Funktion wandlelt alle Texte in Großbuchstaben um.

**Remove Accents**  
Einige Sprachen verwenden Akzente die die Matrix nicht darstellen kann. Diese Funktion ersetzt diese mit lesbaren Zeichen.

**Verbose Log**  
Diese Funktion erweitert den Log. Dies ist vorallem Hilfreich bei Bugreports.

**Analytics**  
Diese Funktion erlaubt die Übergabe der IP-Adresse an den AWTRIX Cloud Server. Es werden keine weiteren Einstellungen oder Informationen gesendet.
Anhand dieser IP Adresse kann ich einsehen in welchem Land AWTRIX läuft und wieviele insgesamt. Diese Information wird nicht an dritte weitergegeben und nicht gespeichert.
Die Information wird temporär zur Laufzeit meines Servers gehalten, und wird komplett gelöscht sobald ein AWTRIX Host länger als 10min offline ist.  
P.S. Jeder normale Webseiten Aufruf, Email-Versand und auch die Downloads der Icons hinterlässt am jeweiligen Server immer die IP-Adresse. Bei AWTRIX könnt ihr aber bestimmen ob ich diese zur Auswertung nutzen darf. Dies hilft mir zu sehen wie verbreitet mein Projekt bisher ist, dadurch kann ich AWTRIX auf bestimmte Länder anpassen und es motiviert mich natürlich massiv euch immer mehr Funktionen zu bieten.

**Textcolor**  
Hier kannst du die globale Textfarbe bestimmen.
Trage entweder deine gewünschte Farbe im Format rgb(R,G,B) ein oder nutze den Colorpicker auf der rechten Seite

**Brightness**  
Hier wird die Helligkeit der Matrix festgelegt. Bitte bedenke: Je heller die Matrix, desto mehr Strom wird verbraucht und desto wärmer wird sie. 

!> Die Matrix kann bei höchster Helligkeitsstufe und komplett weißen Pixeln bis zu 75 Watt beanspruchen!

**App Duration**
Legt die Zeit fest, wie lange eine App angezeigt wird, bevor zur Nächsten gewechselt wird.

**Scroll speed**
Mit diesem Wert wird angebegen nach wievielen Millisekunden der Text um eine Y-Position verschoben wird. Ein niedriger Wert lässt den Text schneller scrollen, sorgt allerdings auch für eine höhere CPU Auslastung.

**Update interval**
Dieser wert gibt an, nach wievielen Sekunden alle Apps ihre Daten aktualisieren.

**Volume**
Stellt die Lautstärke des angeschlossenen DFPlayer ein.

**Timezone Offset (UTC)**
Dies stellt die Differenz zur UTC Zeitzone ein.

### Communication

#### Webserver
**Port**   
ändert den Port über den das AWTRIX Webinterface aufgerufen wird

**Enable Login**  
Aktiviert die Anmeldemaske des AWTRIX Webinterfaces

**Login Password**  
Das Passwort für die Anmeldemaske (Standard: **awtrix**)

#### MQTT
Aktiviert den MQTT Client. Weitere Einstellungen sind selbsterklärend.

### Matrix connection
Du kannst die Matrix entweder über WiFi oder USB betreiben. Wenn du ein schwaches oder überlastetes WiFi hast, versuche bitte die Kommunikation der Matrix über USB an, um Ruckeln zu vermeiden. 

### Premium
Diese Kategorie bietet tolle Funktionen die nur durch den Kauf eines Premium Schlüssels freigeschaltet werden. Diesen erhälst du bei mir im Shop.
Durch den Kauf eines Schlüssels unterstützt du mich bei der weiteren Entwicklung von AWTRIX und beim bezahlen meiner anfallenden Kosten wie z.b Servermiete, Kauf von neuen Bauteilen usw.

**AWTRIX Cloud**  
Aktiviert die Anbindung an die AWTRIX Cloud. Weitere Informationen dazu findest du [hier](/de-de/cloud.md).  
Nach der Aktivierung erhälst du einen Token den du für die externe Ansteuerung benötigst. Mit "Revoke Token" kannst du dir jederzeit einen neuen erstellen lassen.

**Fritz!Box Call Monitor**  
Wer eine FritzBox der Firma AVM sein eigen nennt, kann mit dieser Funktion die FritzBox in AWTRIX einbinden, so dass beispielsweise über einen eingehenden Anruf oder die Rufnummer des Anrufenden informiert wird.
Gib hierzu die IP Adresse der Fritzbox an und richte, wenn gewünscht, noch das Telefonbuch ein. Wenn ein Telefonbuch hinterlegt ist, zeigt AWTRIX bei einem Anruf den passenden Namen an, ansonsten die Telefonnummer.   Du kannst entweder ein Telefonbuch aus der FritzBox exportieren und [in eine JSON umwandeln](http://www.utilities-online.info/xmltojson/) oder in das Editor Fenster einfügen oder, wenn das nicht klappt, dein Telefonbuch manuell erstellen. Dazu musst du nur für jede Nummer eine neue Zeile verwenden. Der Aufbau ist sehr einfach:
``` BASH
01514875965=Blueforcer
01603262987=Günther
06185772637=Herbert
usw..
```