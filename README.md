# Sus-Jos

Jocul de pe tabla de circ cu 120 de căsuțe, online, pentru până la 10 jucători.

**Joacă aici:** https://mateich8.github.io/sus-jos/

## Cum joci

1. Scrie-ți porecla, alege culoarea pionului și, dacă vrei, pune o poză pe el.
2. Apasă **Partidă nouă**, apoi **Trimite** ca să le dai prietenilor linkul.
3. Cine deschide linkul apasă **Intră în joc**. Nu e nevoie de cont.
4. Când sunteți toți, apăsați **Începe jocul**. Ordinea se trage la sorți.

Dai cu zarul și muți pionul. Dacă te oprești pe o căsuță galbenă de unde pleacă o săgeată, mergi pe săgeată: urci sau cobori, fiecare săgeată cu animația ei. La final ai nevoie de exact cât îți lipsește până la 120: dacă dai mai puțin, înaintezi; dacă dai mai mult, rămâi pe loc.

Mai sunt câteva reguli, pe care le poți opri înainte de start:

- **Căsuța ocupată:** dacă ajungi pe o căsuță unde stă deja cineva, zarul se anulează. Te întorci unde erai și trece rândul.
- **Căsuțe surpriză:** șase căsuțe ascunse. La două mai arunci o dată, la două stai o tură, la două schimbi locul cu cineva.
- **Aruncarea automată:** dacă nu arunci 30 de secunde, jocul aruncă pentru tine.

În timpul jocului poți trimite reacții și fraze rapide care apar deasupra pionului tău. La final vezi statisticile partidei și clasamentul pe toate partidele jucate cu același cod. Fiecare își poate pune o culoare, o poză și un accesoriu pe pion.

Dacă stați toți la aceeași masă, **Joc pe un telefon** vă lasă să jucați pe rând pe un singur telefon. Din butonul **Trimite** apare și un cod QR, ca să intre cine e lângă tine. Pe telefon poți pune Sus-Jos pe ecranul principal, ca aplicație.

## Cum funcționează

Tabla e poza tablei originale, îndreptată și îmbunătățită (`board.jpg`). Muzica jocului e `audio/circus.mp3`; efectele sonore sunt generate în browser. Din butonul cu difuzor poți opri sunetul sau poți pune altă melodie de pe telefonul tău, care se aude doar la tine.

Mutările trec prin două servere MQTT publice și gratuite (EMQX și HiveMQ), criptate AES-GCM cu o cheie derivată din codul partidei. Doar cine are codul poate citi partida, numele și pozele.

## Imagini

Efectele din animații, reacțiile și accesoriile pionilor sunt [Fluent Emoji](https://github.com/microsoft/fluentui-emoji) de la Microsoft, folosite sub licența MIT (vezi `img/LICENSE-fluentui-emoji.txt`). Codul QR e generat cu [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) de Kazuhiko Arase (MIT).
