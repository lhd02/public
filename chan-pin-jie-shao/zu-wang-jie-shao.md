# Úvod do kabelového zapojení systému

* Tento produkt je určen pro síťová řešení záložního napájení domácnosti. Musí být používán v&nbsp;kombinaci s&nbsp;FV panely, měniči, bateriovými boxy, hlavními ovládacími spínači, spotřebiči, generátory a&nbsp;energetickou sítí.
* V&nbsp;případě výpadku napájení přepne domácí systém ukládání energie do ostrovního provozního režimu. Po obnovení normálního provozu elektrické sítě se domácí systém ukládání energie přepne zpět do režimu připojení k&nbsp;síti. Tím se dosáhne plynulého přepnutí mezi FV úložištěm a&nbsp;generátorem.

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Při síťovém propojení záložního napájení závisí doba ostrovního provozu záložního napájení spotřebiče na kapacitě napájecího zdroje systému FV úložiště. Pokud se&nbsp;ve&nbsp;zdroji napájení systému FV úložiště vyskytne během ostrovního provozu něco neobvyklého (například neobvyklé generování FV energie, nedostatek energie v&nbsp;bateriích a&nbsp;neobvyklé dodávky energie generátorem), stále nebude možné používat záložní napájení spotřebiče.</mark>
* <mark style="color:blue;">Schéma sítě uvádí jako příklad dva měniče. Počet měničů, které lze připojit, závisí na specifikaci zařízení Gateway. Pro více informací viz Tabulka 2-1.</mark>

**Tabulka 2-1**

<table><thead><tr><th width="102" align="center">S/N</th><th width="204">Model</th><th>Počet připojiteln&yacute;ch měničů</th></tr></thead><tbody><tr><td align="center">1</td><td>Sigen Gateway TPLV C30-2</td><td>2 jednotky</td></tr><tr><td align="center">2</td><td>Sigen Gateway C60-2</td><td>2 jednotky</td></tr><tr><td align="center">3</td><td>Sigen Gateway C60 AU</td><td>2 jednotky</td></tr><tr><td align="center">4</td><td>Sigen Gateway TPLV C70-6</td><td>6 jednotek</td></tr><tr><td align="center">5</td><td>Sigen Gateway C120-6</td><td>6 jednotek</td></tr><tr><td align="center">6</td><td>Sigen Gateway C180-9</td><td>9 jednotek</td></tr><tr><td align="center">7</td><td>Sigen Gateway C300-12</td><td>12 jednotek</td></tr><tr><td align="center">8</td><td>Sigen Gateway C600</td><td>30 jednotek</td></tr><tr><td align="center">9</td><td>Sigen Gateway C1200</td><td>50 jednotek</td></tr><tr><td align="center">10</td><td>Sigen Gateway C600-B</td><td>10 jednotek</td></tr><tr><td align="center">11</td><td>Sigen Gateway C1200-B</td><td>20 jednotek</td></tr></tbody></table>

### **Schéma kabelového zapojení záložního systému pro celý dům**

**Jeden měnič (zařízení Gateway má jistič pro připojení inteligentního spotřebiče&nbsp;/ naftového generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00029-单逆-en (2).jpg" alt="" width="563"><figcaption></figcaption></figure>

**Jeden měnič (zařízení Gateway nemá jistič připojený k&nbsp;inteligentnímu spotřebiči&nbsp;/ naftovému generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00029-单逆无智-en.jpg" alt="" width="563"><figcaption></figcaption></figure>

### **Více měničů (zařízení Gateway má jistič pro připojení inteligentního spotřebiče&nbsp;/ naftového generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00029-多逆有智en.png" alt="" width="563"><figcaption></figcaption></figure>

### **Více měničů (zařízení Gateway nemá jistič připojený k&nbsp;inteligentnímu spotřebiči&nbsp;/ naftovému generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00029-多逆无智en.png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="64" align="center">Č.</th><th width="114">Popis</th><th width="65" align="center">Č.</th><th width="295">Popis</th><th width="63">Č.</th><th>Popis</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>FV panel</td><td align="center"><strong>B</strong></td><td>SigenStor EC&nbsp;/ Sigen Hybrid</td><td><strong>C</strong></td><td>SigenStor BAT</td></tr><tr><td align="center"><strong>D</strong></td><td>Gateway</td><td align="center"><strong>E</strong></td><td>Z&aacute;lohovan&aacute; rozvodn&aacute; skř&iacute;ň</td><td><strong>F</strong></td><td>Z&aacute;lohovan&eacute; dom&aacute;c&iacute; spotřebiče</td></tr><tr><td align="center"><strong>G</strong></td><td>Naftov&yacute; gener&aacute;tor</td><td align="center"><strong>H</strong></td><td>Inteligentn&iacute; spotřebiče</td><td><strong>I</strong></td><td>Energetick&aacute; s&iacute;ť</td></tr><tr><td align="center"><strong>J</strong></td><td>mySigen</td><td align="center"><strong>K</strong></td><td>Směrovač</td><td><strong>L</strong></td><td>Ant&eacute;na</td></tr><tr><td align="center"><strong>M</strong></td><td>CommMod</td><td align="center"></td><td></td><td></td><td></td></tr></tbody></table>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Pokud&nbsp;F (zálohovaný domácí spotřebič) zaznamená únik proudu, může to představovat riziko úrazu elektrickým proudem. Aby se předešlo tomuto nebezpečí, musí být mezi&nbsp;D (zařízení Gateway) a&nbsp;F (zálohovaný domácí spotřebič) instalován proudový chránič (RCD).</mark>
* <mark style="color:blue;">Jako záložní zdroj energie pro dlouhodobé ostrovní aplikace může naftový generátor spolupracovat se zařízením Gateway, aby zajistil plynulý přechod mezi fotovoltaikou, skladováním energie a&nbsp;naftovou výrobou.</mark>
* <mark style="color:blue;">Veškerá napájená zařízení v&nbsp;domácnosti majitele lze připojit jako inteligentní spotřebiče. Aby tento produkt přinesl uživatelům co největší užitek, doporučuje se připojit napájená zařízení s&nbsp;vysokým příkonem jako inteligentní spotřebiče (tepelná čerpadla, ohřívače bazénu, sušičky prádla apod.), které lze odpojit, když má systém ukládání energie nízký stav nabití. Ostatní napájená zařízení s&nbsp;nízkým příkonem jsou připojena jako domácí spotřebiče (osvětlení, směrovače apod.)</mark>
* <mark style="color:blue;">Pro komunikaci s&nbsp;měniči se doporučuje používat Fast Ethernet a&nbsp;WLAN. Když u&nbsp;modulu CommMod dojde volný datový limit 4G, uživatelé musí vyměnit SIM kartu.</mark>

### **Schéma kabelového zapojení záložního systému pro část domácnosti**

### **Jeden měnič (zařízení Gateway má jistič pro připojení inteligentního spotřebiče&nbsp;/ naftového generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00030-单逆-en.jpg" alt="" width="563"><figcaption></figcaption></figure>

### **Jeden měnič (zařízení Gateway nemá jistič připojený k&nbsp;inteligentnímu spotřebiči&nbsp;/ naftovému generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00030-单逆无智-en.jpg" alt="" width="563"><figcaption></figcaption></figure>

### **Více měničů (zařízení Gateway má jistič pro připojení inteligentního spotřebiče&nbsp;/ naftového generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00030-EN (1).jpg" alt="" width="563"><figcaption></figcaption></figure>

### **Více měničů (zařízení Gateway nemá jistič připojený k&nbsp;inteligentnímu spotřebiči&nbsp;/ naftovému generátoru)**

<figure><img src="../.gitbook/assets/SSA1OV00030-多逆无智en.png" alt="" width="563"><figcaption></figcaption></figure>

| Č.| Popis| Č.| Popis| Č.| Popis|
|----------|----------|----------|----------|----------|----------|
| **A**| FV panel| **B**| SigenStor EC&nbsp;/ SigenStor AC&nbsp;/ Sigen Hybrid| **C**| SigenStor BAT|
| **D**| Gateway| **E1**| Zálohovaná rozvodná skříň| **E2**| Nezálohovaná rozvodná skříň|
| **F1**| Zálohované domácí spotřebiče| **F2**| Nezálohované domácí spotřebiče| **G**| Naftový generátor|
| **H**| Inteligentní spotřebiče| **I**| Senzor energie| **J**| Energetická síť|
| **K**| mySigen| **L**| Směrovač| **M**| Anténa|
| **N**| CommMod| | | | |

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Pokud má E2 (nezálohovaná rozvodná skříň) ochranu proti úniku proudu, doporučuje se, aby jmenovitý zbytkový provozní proud byl větší nebo roven počtu měničů × 100&nbsp;mA.</mark>
* <mark style="color:blue;">Pokud&nbsp;F1 (zálohovaný domácí spotřebič) zaznamená únik proudu, může to představovat riziko úrazu elektrickým proudem. Aby se předešlo tomuto nebezpečí, musí být mezi&nbsp;D (zařízení Gateway) a&nbsp;F1 (zálohovaný domácí spotřebič) instalován proudový chránič (RCD).</mark>
* <mark style="color:blue;">Jako záložní zdroj energie pro dlouhodobé ostrovní aplikace může naftový generátor spolupracovat se zařízením Gateway, aby zajistil plynulý přechod mezi fotovoltaikou, skladováním energie a&nbsp;naftovou výrobou energie.</mark>
* <mark style="color:blue;">Veškerá napájená zařízení v&nbsp;domácnosti majitele lze připojit jako inteligentní spotřebiče. Aby tento produkt přinesl uživatelům co největší užitek, doporučuje se připojit napájená zařízení s&nbsp;vysokým příkonem jako inteligentní spotřebiče (tepelná čerpadla, ohřívače bazénu, sušičky prádla apod.), které lze odpojit, když má systém ukládání energie nízký stav nabití. Ostatní napájená zařízení s&nbsp;nízkým příkonem jsou připojena jako inteligentní spotřebiče (tepelná čerpadla, ohřívače bazénu, sušičky prádla apod.), které lze odpojit, když má systém ukládání energie nízký stav nabití. Ostatní napájená zařízení s&nbsp;nízkým příkonem jsou připojena jako domácí spotřebiče (osvětlení, směrovače apod.)</mark>
* <mark style="color:blue;">Senzor energie má funkci sběru dat pro body připojení k&nbsp;síti a&nbsp;umožňuje připojení k&nbsp;síti s&nbsp;nulovým odběrem energie. Pro kabelové zapojení záložního systému pro část domácnosti není třeba konfigurovat senzor energie. Pro kabelové zapojení systému řízení připojení k&nbsp;částečnému záložnímu napájení a&nbsp;k&nbsp;síti s&nbsp;nulovým odběrem je nakonfigurován senzor energie.</mark>
* <mark style="color:blue;">Pro komunikaci s&nbsp;měniči se doporučuje používat Fast Ethernet a&nbsp;WLAN. Když u&nbsp;modulu CommMod dojde volný datový limit 4G, uživatelé musí vyměnit SIM kartu.</mark>
