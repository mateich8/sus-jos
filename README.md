# Sus-Jos

Jocul de pe tabla de circ cu 120 de căsuțe, online, pentru până la 10 jucători.

**Joacă aici:** https://mateich8.github.io/sus-jos/

## Cum joci

1. Scrie-ți porecla, alege culoarea pionului și, dacă vrei, pune o poză pe el.
2. Apasă **Partidă nouă**, apoi **Trimite** ca să le dai prietenilor linkul.
3. Cine deschide linkul apasă **Intră în joc**. Nu e nevoie de cont.
4. Când sunteți toți, apăsați **Începe jocul**. Ordinea se trage la sorți.

Dai cu zarul și muți pionul. Dacă te oprești pe o căsuță galbenă de unde pleacă o săgeată, mergi pe săgeată: urci sau cobori. Câștigă primul care ajunge exact pe 120.

Dacă stați toți la aceeași masă, **Joc pe un telefon** vă lasă să jucați pe rând pe un singur telefon.

## Cum funcționează

Pagina e un singur fișier HTML. Mutările trec prin două servere MQTT publice și gratuite (EMQX și HiveMQ), criptate AES-GCM cu o cheie derivată din codul partidei. Doar cine are codul poate citi partida, numele și pozele.
