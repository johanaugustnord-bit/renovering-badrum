# Accessmodell

Ett GitHub-baserat projekt kan organiseras med olika nivåer av transparens. Vilken modell som är bäst beror på projektets storlek, avtal, personuppgifter och hur många externa parter som deltar.

## Modell A – helt öppet

Alla deltagare ser samma repository och samma Issues.

Fördelar:
- maximal transparens
- enklast administration
- alla AI-assistenter kan läsa samma projektkontext
- färre informationssilor
- lättare att förstå beroenden mellan yrkesroller

Nackdelar:
- alla ser även kommersiella diskussioner
- personuppgifter och känsliga bilagor kräver extra disciplin
- vissa leverantörer kan få mer information än de behöver

Denna modell passar väl för demonstrationsprojektet `renovering-badrum`.

## Modell B – rollbaserad åtkomst

Projektets kärna är gemensam, men känsligare information separeras.

Exempel på gemensamt innehåll:
- krav
- tidplan
- tekniska beslut
- arbets-Issues
- beroenden
- kvalitetsgrindar
- materialstatus

Exempel på begränsat innehåll:
- fullständiga offerter
- avtal
- personuppgifter
- interna kostnadskalkyler
- betalningsinformation
- tvister eller kommersiella förhandlingar

Det begränsade innehållet kan ligga i ett separat privat repository, en skyddad dokumentyta eller ett annat system med tydligare behörighetsstyrning.

## Rekommenderad hybridmodell

För ett verkligt byggprojekt är en hybridmodell ofta bäst:

1. **Gemensamt projekt-repo** – alla relevanta roller har läsåtkomst och kan se projektets operativa sanning.
2. **Rollspecifika skrivbehörigheter** – varje yrkesroll uppdaterar främst sina egna Issues och dokumentationsdelar.
3. **Privat kommersiellt repo eller dokumentyta** – byggherre och huvudentreprenör hanterar offerter, avtal och känslig ekonomi separat.
4. **AI-assistenter följer samma behörigheter som användaren** – en elektrikers Codex ska inte få mer åtkomst än elektrikern själv.

## Princip för AI-agenter

Varje användares ChatGPT eller Codex ska arbeta inom samma åtkomstgränser som den mänskliga rollen.

Det innebär exempelvis:

- byggherrens AI kan få läsa budget, offerter och beslutsunderlag
- huvudentreprenörens AI kan läsa samordningsinformation och tekniska beroenden
- rörmokarens AI läser relevanta VVS-Issues och gemensam projektinformation
- elektrikerns AI läser elrelaterade Issues och nödvändiga beroenden
- leverantörens AI behöver normalt bara produkt-, order- och leveransinformation

AI får alltså inte bli en bakväg runt projektets behörighetsmodell.

## Viktig begränsning i GitHub

GitHub-behörigheter är i grunden starkast på repository- och organisationsnivå. Om man behöver mycket finmaskig åtkomst till enskilda filer eller kommersiella dokument är det ofta bättre att separera informationen i flera repos eller använda en kompletterande dokumentplattform.

## För demonstrationen

Det publika `renovering-badrum` visar den öppna modellen eftersom syftet är pedagogiskt. Dokumentet beskriver samtidigt hur samma arbetssätt kan utvecklas till en rollbaserad modell i ett verkligt projekt.
