# Einführung in die Systemverdrahtung

* Dieses Produkt ist für Netzszenarien von Notstromsystemen für Haushalte ausgelegt. Es muss in Verbindung mit PV-Modulen, Wechselrichtern, Batterien/Akkus, Hauptschaltern, Lasten, Generatoren und Stromnetzen verwendet werden.
* Bei einem Stromausfall schaltet das Energiespeichersystem des Haushalts in den netzunabhängigen Betriebsmodus. Sobald das Stromnetz wieder normal funktioniert, schaltet das Energiespeichersystem des Haushalts wieder in den netzabhängigen Modus. Dadurch wird ein nahtloser Wechsel zwischen PV-Speicher und Generator erreicht.

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Bei einem Notstromnetz hängt die Dauer des netzunabhängigen Betriebs der Notstromlast von der Stromversorgungskapazität des PV-Speichersystems ab. Bei Anomalien in der Stromversorgung des PV-Speichersystems während des netzunabhängigen Betriebs (unter anderem abnormale PV-Stromerzeugung, unzureichende Batterieleistung und anomale Stromversorgung des Generators) kann kein Reservestrom genutzt werden.</mark>
* <mark style="color:blue;">Das Netzwerkdiagramm zeigt zwei Wechselrichter als Beispiel. Die Anzahl der anschließbaren Wechselrichter hängt von der Gateway-Spezifikation ab. Weitere Informationen finden Sie in Tabelle 2-1.</mark>

**Tabelle 2-1**

<table><thead><tr><th width="75">Seriennr.</th><th>Modell</th><th>Anzahl der anschließbaren Wechselrichter</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Sigen Gateway HomeMax SP</td><td>3 Einheiten</td></tr><tr><td><strong>2</strong></td><td>Gateway Home SP</td><td>1 Einheit</td></tr><tr><td><strong>3</strong></td><td>Gateway Home SP 12K</td><td>2 Einheiten</td></tr><tr><td><strong>4</strong></td><td>Sigen Gateway SP AU</td><td>2 Einheiten</td></tr><tr><td><strong>5</strong></td><td>Sigen Gateway HomeMax TP</td><td>2 Einheiten</td></tr><tr><td><strong>6</strong></td><td>Sigen Gateway Home TP</td><td>1 Einheit</td></tr><tr><td><strong>7</strong></td><td>Sigen Gateway TP AU</td><td>2 Einheiten</td></tr><tr><td><strong>8</strong></td><td>Sigen Gateway HomeMax TP CN</td><td>2 Einheiten</td></tr><tr><td><strong>9</strong></td><td>Sigen Gateway Home TP 30K</td><td>1 Einheit</td></tr><tr><td><strong>10</strong></td><td>Sigen Gateway Home TP 30K CN</td><td>1 Einheit</td></tr></tbody></table>

### Verdrahtungsplan für die vollständige Notstromversorgung

**Einzelner Wechselrichter (Gateway verfügt über den Schutzschalter für den Anschluss der intelligenten Last/des Dieselgenerators)**

![](../.gitbook/assets/SSA1OV00029-单逆-DE.png)

**Einzelner Wechselrichter (Gateway verfügt nicht über den Schutzschalter,** **der an die intelligente Last/den Dieselgenerator angeschlossen ist)**

![](../.gitbook/assets/SSA1OV00029-单逆无智-de.png)

**Mehrere Wechselrichter (Gateway verfügt über den Schutzschalter für den Anschluss der intelligenten Last/des Dieselgenerators)**

![](../.gitbook/assets/SSA1OV00029-多逆-DE.png)

**Mehrere Wechselrichter (Gateway verfügt nicht über den Schutzschalter, der an die intelligente Last/den Dieselgenerator angeschlossen ist)**

![](../.gitbook/assets/SSA1OV00029-多逆无智-DE.png)

<table><thead><tr><th width="81">Nr.</th><th>Beschreibung</th><th width="78">Nr.</th><th>Beschreibung</th><th>Nr.</th><th>Beschreibung</th></tr></thead><tbody><tr><td><strong>A</strong></td><td>PV-Modul</td><td><strong>B</strong></td><td>SigenStor EC/SigenStor AC /Sigen Hybrid</td><td><strong>C</strong></td><td>SigenStor BAT</td></tr><tr><td><strong>D</strong></td><td>Gateway</td><td><strong>E</strong></td><td>Notstrom-Verteilertafel</td><td><strong>F</strong></td><td>Haushaltslasten mit Notstrom</td></tr><tr><td><strong>G</strong></td><td>Haushaltslasten mit Notstrom</td><td><strong>H</strong></td><td>Intelligente Verbraucher</td><td><strong>I</strong></td><td>Stromnetz</td></tr><tr><td><strong>J</strong></td><td>mySigen</td><td><strong>K</strong></td><td>Router</td><td><strong>L</strong></td><td>Antenne</td></tr><tr><td><strong>M</strong></td><td>CommMod</td><td></td><td></td><td></td><td></td></tr></tbody></table>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Wenn B = Sigen Hybrid ist C optional.</mark>
* <mark style="color:blue;">Wenn F (Notstromverbraucher) ein Leck aufweist, besteht Stromschlaggefahr. Um diese Gefahr zu vermeiden, muss zwischen D (Gateway) und F (Notstromverbraucher) ein Fehlerstromschutzschalter (RCD) installiert werden.</mark>
* <mark style="color:blue;">Als Reserveenergiequelle für langfristige netzunabhängige Anwendungen kann der Dieselgenerator zusammen mit dem Gateway einen reibungslosen Übergang zwischen Photovoltaik, Speicherung und Dieselgenerierung gewährleisten.</mark>
* <mark style="color:blue;">Alle Stromgeräte im Heim des Eigentümers können als intelligente Verbraucher angeschlossen werden. Um sicherzustellen, dass dieses Produkt den größtmöglichen Nutzen für die Benutzer bringt, wird empfohlen, die Hochleistungsgeräte als intelligente Lasten (Wärmepumpen, Poolheizungen, Wäschetrockner usw.) anzuschließen, die abgeschaltet werden können, wenn das Energiespeichersystem nur noch über eine geringe Leistung verfügt. Andere Geräte mit niedrigem Leistungsbedarf sind als Haushaltslasten (Lampen, Router usw.) angeschlossen.</mark>
* <mark style="color:blue;">Es wird empfohlen, schnelles Ethernet und WLAN zur Kommunikation mit Wechselrichtern zu verwenden. Wenn der kostenlose 4G-Datenverkehr von CommMod aufgebraucht ist, muss der Nutzer die SIM-Karte austauschen.</mark>

### **Verdrahtungsplan für die partielle Notstromversorgung**

**Einzelner Wechselrichter (Gateway verfügt über den Schutzschalter für den Anschluss der intelligenten Last/des Dieselgenerators)**

![](../.gitbook/assets/SSA1OV00030-单逆-DE.png)

**Einzelner Wechselrichter (Gateway verfügt nicht über den Schutzschalter, der an die intelligente Last/den Dieselgenerator angeschlossen ist)**

![](../.gitbook/assets/SSA1OV00030-单逆无智-DE.png)

**Mehrere Wechselrichter (Gateway verfügt über den Schutzschalter für den Anschluss der intelligenten Last/des Dieselgenerators)**

![](../.gitbook/assets/SSA1OV00030-多逆-DE.png)

**Mehrere Wechselrichter (Gateway verfügt nicht über den Schutzschalter, der an die intelligente Last/den Dieselgenerator angeschlossen ist)**

![](../.gitbook/assets/SSA1OV00030-多逆无智-DE.png)

| Nr.    | Beschreibung                 | Nr.    | Beschreibung                            | Nr.    | Beschreibung                  |
| ------ | ---------------------------- | ------ | --------------------------------------- | ------ | ----------------------------- |
| **A**  | PV-Modul                     | **B**  | SigenStor EC/SigenStor AC /Sigen Hybrid | **C**  | SigenStor BAT                 |
| **D**  | Gateway                      | **E1** | Notstrom-Verteilertafel                 | **E2** | Nicht-Notstrom-Verteilertafel |
| **F1** | Haushaltslasten mit Notstrom | **F2** | Haushaltslasten ohne Notstrom           | **G**  | Dieselgenerator               |
| **H**  | Intelligente Verbraucher     | **I**  | Leistungssensor                         | **J**  | Stromnetz                     |
| **K**  | mySigen                      | **L**  | Router                                  | **M**  | Antenne                       |
| **N**  | CommMod                      |        |                                         |        |                               |

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Wenn B = Sigen Hybrid ist C optional.</mark>
* <mark style="color:blue;">Wenn E2 (Verteilertafel) ohne Rückspeisung über Leckstromschutz verfügt, wird empfohlen, dass der Nenn-Restbetriebsstrom größer oder gleich der Anzahl der Wechselrichter × 100 mA ist.</mark>
* <mark style="color:blue;">Wenn F1 (Notstromverbraucher) ein Leck aufweist, besteht Stromschlaggefahr. Um diese Gefahr zu vermeiden, muss zwischen D (Gateway) und F1 (Notstromverbraucher) ein Fehlerstromschutzschalter (RCD) installiert werden.</mark>
* <mark style="color:blue;">Als Reserveenergiequelle für langfristige netzunabhängige Anwendungen kann der Dieselgenerator zusammen mit dem Gateway einen reibungslosen Übergang zwischen Photovoltaik, Speicherung und Dieselstromerzeugung gewährleisten.</mark>
* <mark style="color:blue;">Alle Stromgeräte im Heim des Eigentümers können als intelligente Verbraucher angeschlossen werden. Um sicherzustellen, dass dieses Produkt den größtmöglichen Nutzen für die Benutzer bringt, wird empfohlen, die Hochleistungsgeräte als intelligente Lasten (Wärmepumpen, Poolheizungen, Wäschetrockner usw.) anzuschließen, die abgeschaltet werden können, wenn das Energiespeichersystem nur noch über eine geringe Leistung verfügt. Andere Geräte mit niedrigem Leistungsbedarf sind als Haushaltslasten (Lampen, Router usw.) angeschlossen.</mark>
* <mark style="color:blue;">Der Leistungssensor verfügt über Datenerfassung am Netzanschlusspunkt, um einen Nullstrom-Netzanschluss zu erreichen. Für die partielle Notstrom</mark>-<mark style="color:blue;">Systemverdrahtung: der Leistungssensor muss nicht konfiguriert werden. Für die Verdrahtung der partiellen Notstromversorgung und der Nullstrom-Netzanschlusssteuerung: der Leistungssensor ist konfiguriert.</mark>
* <mark style="color:blue;">Es wird empfohlen, schnelles Ethernet und WLAN zur Kommunikation mit Wechselrichtern zu verwenden. Wenn der kostenlose 4G-Datenverkehr von CommMod aufgebraucht ist, muss der Nutzer die SIM-Karte austauschen.</mark>
