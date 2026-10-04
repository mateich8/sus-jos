# Sus-Jos

Jocul de pe tabla de circ cu 120 de căsuțe, online, pentru până la 10 jucători.

**Joacă aici:** https://mateich8.github.io/sus-jos/

## Cum joci

1. Scrie-ți porecla, alege culoarea pionului și, dacă vrei, pune o poză pe el.
2. Apasă **Partidă nouă**, apoi **Trimite** ca să le dai prietenilor linkul.
3. Cine deschide linkul apasă **Intră în joc**. Nu e nevoie de cont.
4. Când sunteți toți, apăsați **Începe jocul**. Ordinea se trage la sorți.

Dai cu zarul și muți pionul. Dacă te oprești pe o căsuță galbenă de unde pleacă o săgeată, mergi pe săgeată: urci sau cobori, fiecare săgeată cu animația ei. La final ai nevoie de exact cât îți lipsește până la 120: dacă dai mai puțin, înaintezi; dacă dai mai mult, rămâi pe loc.

Dacă stați toți la aceeași masă, **Joc pe un telefon** vă lasă să jucați pe rând pe un singur telefon.

## Cum funcționează

Tabla e poza tablei originale, îndreptată și îmbunătățită (`board.jpg`). Muzica jocului e `audio/circus.mp3`; efectele sonore sunt generate în browser. Din butonul cu difuzor poți opri sunetul sau poți pune altă melodie de pe telefonul tău, care se aude doar la tine.

Mutările trec prin două servere MQTT publice și gratuite (EMQX și HiveMQ), criptate AES-GCM cu o cheie derivată din codul partidei. Doar cine are codul poate citi partida, numele și pozele.

## Imagini

Efectele din animații (racheta, baloanele, umbrela, papagalul, trofeul și altele) sunt [Fluent Emoji](https://github.com/microsoft/fluentui-emoji) de la Microsoft, folosite sub licența MIT (vezi `img/LICENSE-fluentui-emoji.txt`).
