P44 Script für Steuerung Helios KWL (muss easycontrols 3.0 Firmware drauf haben).
Stellt die Temperatur und Luftfeuchtigkeit der Helios Sensoren in DS bereit.
Stellt die Aktionen Zuhause, Unterwegs, Boost und Boost 30min zur Verfügung um den Lüftungsmodus des Helios KWL Geräts zu ändern.

P44 muss in userlevel 1 laufen (-> Beta-Firmwares)

Erforderliche Hardware:

    Waveshare RS485 to USB Konverter
    Cat6 Kabel

Hardware Konfiguration:
Cat6 Kabel an beiden Seiten je 4 Adern abisolieren, jeweils 2 verdrillen und Aderendhülse draufklemmen.
Auf der einen Seite den Waveshare Adapter anklemmen und in den USB Port der P44 stecken.
Die andere Seite vom Kabel an den Modbus Anschluss des Helios KWL Gerätes anklemmen (s. Helios Handbuch)

Je nachdem an welchen USB Port der P44 man den Waveshare Konverter steckt muss im Script ttyUSB0 in der Zeile mb.connection("/dev/ttyUSB0:19200,8,E,1", "RS232"); angepasst werden!
