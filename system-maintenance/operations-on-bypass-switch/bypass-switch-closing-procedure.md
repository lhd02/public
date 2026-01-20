# Ohituskytkimen sulkemismenettely

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Kun Gatewayn verkon kontaktorin epänormaali toiminta estää virransyötön kuormalle, sulje ohituskytkin ja syötä kuorma suoraan verkosta.</mark>

### Vaiheet

1. Tarkista, että sähköverkko syöttää virtaa normaalisti.
2. Katkaise virta, kuten kohdassa [_Virran katkaisu._](../power-off/)
3. Katso laitteen tarrassa ilmoitettu viiveaika ja odota ilmoitettu aika. Kun aika on kulunut, poista ohituskytkimen lukitusrengas ja kytke ohituskytkin päälle.

<figure><img src="../../.gitbook/assets/retaining-ring.png" alt="" width="325"><figcaption></figcaption></figure>

{% include "../../.gitbook/includes/warning.md" %}

* <mark style="color:orange;">Laitteessa on jäännösvirtaa ja se on kuuma heti virran katkaisun jälkeen. Laitteen käyttö heti virran katkaisun jälkeen voi johtaa sähköiskuun tai palovammoihin.</mark>
* <mark style="color:orange;">Laitteessa on korkea jännite. Käytä eristäviä käsineitä, kun kytket kytkimen päälle.</mark>

{% include "../../.gitbook/includes/caution.md" %}

<mark style="color:purple;">Ohituskytkimen kytkemisen jälkeen älä kytke päälle invertteriin ja Gatewayn generaattoriin liitettyä pienkatkaisijaa. Muussa tapauksessa sähköverkon liitäntä latautuu, mikä aiheuttaa sähköiskun vaaran.</mark>

4. Kytke päälle SPD:hen liitetty pienkatkaisija.
5. Kytke päälle sähköverkkoon liitetty pienkatkaisija.
6. Kytke päälle kotitalouskuormien varavoimaan liitetty pienkatkaisija.
7. Sulje laitteiston ovi.
