# ESP-Telegram-Projekt-Dokumentation
### Bauer, Polichetti 3CHIT 11/06/2023

### Einführung
Dies ist die Dokumentation für das ESP-Telegram-Projekt, das uns von Professor Höbert im Rahmen der Aktivitätenwoche vorgestellt wurde. Das Projekt ermöglicht die Integration eines ESP32-Mikrocontrollers mit Telegram, um IoT-Anwendungen zu entwickeln. Diese Dokumentation beschreibt den Lösungsweg, den wir gegangen sind, um das Projekt erfolgreich umzusetzen.

### Lösungsweg
*Schritt 1*: ESP32-Setup
Zunächst haben wir den ESP32 vorbereitet, indem wir die erforderlichen Bibliotheken  installiert haben. Wir haben die Arduino-IDE verwendet, um den Code für den Mikrocontroller zu schreiben und hochzuladen. Dabei haben wir uns an die offizielle Dokumentation von Arduino und den ESP32-Bibliotheken orientiert.

*Schritt 2*: Telegram-Bot erstellen
Um mit Telegram zu kommunizieren, haben wir einen Telegram-Bot erstellt. Dafür haben wir die Telegram-Bot-API genutzt und die erforderlichen Schritte zur Bot-Erstellung befolgt. Wir haben einen eindeutigen Bot-Token erhalten, den wir später im ESP32-Code verwenden.

*Schritt 3*: ESP32 mit Telegram verbinden
Um den ESP32 mit Telegram zu verbinden, haben wir die "UniversalTelegramBot"-Bibliothek verwendet. Wir haben den Bot-Token und die SSID/Passwort-Kombination unseres WLANs in den Code eingefügt. Anschließend haben wir die Telegram-Bot-API genutzt, um eingehende Nachrichten abzurufen und Befehle zu verarbeiten.

*Schritt 4*: Befehle verarbeiten und Aktionen ausführen
Um die empfangenen Telegram-Befehle zu verarbeiten, haben wir eine Funktion im Code implementiert, die die Nachrichten analysiert und entsprechende Aktionen auf dem ESP32 ausführt. Je nach Anwendung konnten wir verschiedene Befehle definieren, um beispielsweise LEDs ein- oder auszuschalten oder Sensordaten abzurufen.

*Schritt 5*: Feedback an den Benutzer senden
Um dem Benutzer Feedback auf seine Befehle zu geben, haben wir die Funktionen der Telegram-Bot-API genutzt, um Nachrichten an den Benutzer zurückzusenden. Dies ermöglichte es dem Benutzer, den Status seiner Aktionen zu überprüfen und entsprechende Bestätigungen oder Fehlermeldungen zu erhalten.

### Anleitung zur erfolgreichen Verwendung

Schließe den ESP32 an deinen Computer an und öffne die Arduino-IDE.
Installiere die erforderlichen Bibliotheken für den ESP32 und Telegram. Beachte dabei die offizielle Dokumentation.
Erstelle einen neuen Telegram-Bot und erhalte den Bot-Token.
Öffne das ESP32-Telegram-Projekt in der Arduino-IDE.
Passe den Code an und füge den Bot-Token sowie deine WLAN-SSID und das Passwort hinzu.
Lade den Code auf den ESP32 hoch.
Verbinde den ESP32 mit der Stromquelle und dem WLAN-Netzwerk.
Starte den Telegram-Client auf deinem Smartphone oder Computer und öffne den erstellten Bot.
Sende Befehle an den Bot, um Aktionen auf dem ESP32 auszuführen.
Überprüfe das Feedback des Bots, um den Status der Aktionen zu sehen.

### Zusätzliche Hinweise
Achte darauf, dass der ESP32 mit dem WLAN-Netzwerk verbunden ist, um die Kommunikation mit Telegram zu ermöglichen.
Überprüfe die Serielle Konsole der Arduino-IDE, um Fehlermeldungen oder Debugging-Informationen anzuzeigen.

### Quellen
[1] Telegram Bot API (2023) Bot API Introduction. Available at: https://core.telegram.org/bots/api (Accessed: June 11th, 2023).

[2] Telegram: Control ESP32/ESP8266 Outputs (Arduino IDE). Available at: (https://randomnerdtutorials.com/telegram-control-esp32-esp8266-nodemcu-outputs/) (Accessed: June 11th, 2023).
