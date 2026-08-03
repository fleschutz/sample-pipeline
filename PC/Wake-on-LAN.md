![Bild](/img/BannerWakeup.jpg)﻿

(Foto: pixabay.com)

Windows 10: Checkliste Wake-On-LAN ⏰
==================

**Wer auf einem entfernten PC arbeiten oder spielen will (z.B. mit Steam Link), muss ihn oft erst mal einschalten. Mit Wake-On-LAN (kurz: WOL) lassen sich ausgeschaltete oder im Energiesparmodus befindliche Rechner aus der Ferne jederzeit wieder einschalten. Theoretisch ist es einfach: sobald die Netzwerkkarte auf UDP-Port 9 ein Netzwerk-Paket mit der eigenen MAC-Adresse erhält (das sogenannte "'Magic Packet"), fährt sie den PC hoch. Mit der folgenden Checkliste umgehen Sie die Stolperfallen in der Praxis.**

... ![Bild](/img/MF.png) *Von Markus Fleschutz*  🕓 *24. November 2019*

1️⃣ IP- und MAC-Adresse notieren
---------------------------------

Vom aufzuweckenden PC werden die MAC-Adresse als auch die IP-Adresse benötigt (bei statischen IP-Adressen die IPv4- oder IPv6-Adresse, andernfalls die Subnet-Adresse). Unter Windows kann man sich beide Adressen unter ***Einstellungen* > *Netzwerk* > *Netzwerk und Internet* > *Ethernet* > *Netzwerkeigenschaften anzeigen*** ausgeben lassen und für später notieren.

2️⃣ Der PC benötigt Strom!
----------------------------

Es hört sich trivial an, aber: wer eine Master-Slave-Steckdose nutzt, muss darauf achten, dass der PC in der Master-Steckdose eingesteckt ist. Auch ein Fußschalter oder Netzschalter trennt den PC im Aus-Zustand dauerhaft vom Strom. Dann kann WOL natürlich nicht funktionieren.

3️⃣ Aktivierung von WOL
------------------------------------

Das BIOS in modernen Motherboards (jünger als 2012) unterstützt WOL und hat auch WOL standardmäßig eingeschaltet. Nur bei Problemen mit WOL sollte man auch im BIOS die Unterstützung überprüfen.

Auch Windows 10 hat WOL mit Magic Packet für Netzwerkkarten standardmäßig aktiviert. Nur bei Problemen mit WOL sollte man die Unterstützung überprüfen.

4️⃣ VPN-Zugang einrichten (optional)
----------------------------------

Wer den Rechner nicht nur aus dem Heimnetzwerk, sondern weltweit aus dem Internet aufwecken möchte, der benötigt einen VPN-Zugang zum heimischen Netzwerk. Dazu wählt man sich in den heimischen Router ein (z.B. bei Fritz!Box-Routern via [http://fritz.box](http://fritz.box)), richtet den VPN-Zugang ein und druckt bzw. speichert die Zugangsdaten.

5️⃣ Anmelde-Bildschirm abschalten (optional)
----------------------

Wird der Rechner per WOL aufgeweckt, dann fährt der PC standardmäßig bis zum Anmeldebildschirm hoch und wartet (ewig) auf Benutzername/Passwort/PIN. Entweder nutzt man dann für die Eingabe Software wie *Remotedesktopverbindung* oder man schaltet den Anmeldebildschirm ab. Dazu unter *Einstellungen* > *Anmeldeoptionen*  ... Passwortabfrage... "Nie" auswählen.

6️⃣ Monitor ausschalten (optional)
--------------------------------------------

Wer öfter WOL nutzt sollte sich angewöhnen, beim Herunterfahren des Rechners auch die Monitore auszuschalten. Denn fährt der Rechner per WOL hoch, können die Monitore ausgeschaltet bleiben und somit die Stromrechnung und die Umwelt schonen. Alternativ kann die Energieverwaltung des Monitors auch so abgeändert werden, dass automatisch nach 5 Minuten der Monitor in Power-Save geht.

7️⃣ WOL-App installieren und einrichten
-----------------------------

Der letzte Schritt und die Frage: von welchem Gerät aus soll aufgeweckt werden?

- Von einem Alexa-fähigen Gerät aus? Dann siehe Link: [Amazon Alexa Skills](https://www.amazon.de/kostenlos-Alexa-Skills/s?ie=UTF8&page=1&rh=n%3A10068460031%2Ck%3Akostenlos)
- Von einem Android-Gerät aus? Dann siehe Link: [Google Play Store](https://play.google.com/store/apps?hl=de)
- Von einem Apple-Gerät aus? Dann siehe Link: [Apple App Store](https://www.apple.com/de/ios/app-store/)
- Von einem Windows-Rechner aus? Dann siehe Link: [ Microsoft Windows Store](https://www.microsoft.com/de-de/store/apps/windows)

Dort nach "Wake on LAN" oder "WOL" suchen und die entsprechende Applikation/Software/Skills installieren. Beim Einrichten der App oder Software wird die IP-Adresse sowie die MAC-Adresse des Rechner benötigt.

Jetzt kann das große Aufwecken beginnen! Viel Spaß damit! ⏰ .