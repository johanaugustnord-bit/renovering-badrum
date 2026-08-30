# Roller, ansvar och AI-stöd

Projektet bygger på principen **en mänsklig roll + en egen AI-assistent**. Varje part förväntas använda sin egen ChatGPT eller Codex för att administrera sitt arbete i samma GitHub-repository.

Det betyder att AI inte ersätter yrkesansvaret. Den hjälper respektive roll att hålla Issues, dokumentation, beslut, status och överlämningar aktuella.

## Byggherre

Ansvar:
- målbild, omfattning och budget
- större ändringsbeslut
- val av entreprenör och huvudleverantörer
- slutligt godkännande

AI-stöd:
- sammanfatta projektstatus
- jämföra offerter och alternativ
- kontrollera budget- och tidplanepåverkan
- skapa beslutsunderlag
- identifiera öppna frågor som kräver beslut

## Huvudentreprenör

Ansvar:
- samordning av arbetsordning och resurser
- hantering av beroenden mellan yrkesgrupper
- avvikelsehantering
- kvalitetsgrindar och överlämning

AI-stöd:
- läsa alla öppna Issues och identifiera blockerare
- skapa daglig/veckovis samordningsstatus
- hitta beroenden mellan VVS, el, snickeri och plattsättning
- skapa nya Issues när avvikelser upptäcks
- kontrollera att föregående moment är dokumenterat innan nästa startar

## Rörmokare / VVS

Ansvar:
- vatten och avlopp
- golvbrunn
- anslutningar för WC, tvättställ, dusch och blandare
- provning och dokumentation

AI-stöd:
- uppdatera VVS-Issues
- dokumentera observationer efter rivning
- skapa frågor om saknade mått eller produktdata
- sammanställa vilka VVS-punkter som blockerar nästa yrkesgrupp
- förbereda överlämning till snickare/plattsättare

## Elektriker

Ansvar:
- elmatning
- belysning, uttag och eventuell golvvärme
- provning och dokumentation

AI-stöd:
- hålla el-Issues och checklistor uppdaterade
- identifiera beroenden till snickeri och plattsättning
- sammanställa materialbehov
- dokumentera färdigställande och öppna restpunkter

## Snickare / bygg

Ansvar:
- rivning och återuppbyggnad
- väggar, tak och konstruktion
- förstärkningar och underlag

AI-stöd:
- dokumentera vad som upptäcks efter rivning
- skapa avvikelse-Issues
- kontrollera vilka installationer som måste vara klara innan väggar stängs
- uppdatera fotodokumentation och status inför överlämning

## Kakelsättare / plattsättare

Ansvar:
- kontroll av underlag
- tätskikt
- plattsättning, fogning och avslut

AI-stöd:
- kontrollera att kvalitetsgrindar före tätskikt är uppfyllda
- hålla material- och leveransfrågor aktuella
- dokumentera dolda moment
- skapa restpunkter vid avvikelser

## Målare

Ansvar där målade ytor ingår:
- förarbete
- rätt målningssystem
- färdigställande av specificerade ytor

AI-stöd:
- dokumentera färg-/produktval
- hålla sina Issues uppdaterade
- rapportera blockerare eller avvikelser

## Leverantör / materialansvarig

Ansvar:
- produktinformation
- order och leveransdatum
- restnoteringar och produktbyten
- garanti- och artikelinformation

AI-stöd:
- uppdatera `inkop/materiallista.md`
- bevaka leveranser och restnoteringar
- föreslå alternativa produkter när något utgår eller blir försenat
- dokumentera konsekvenser för budget och tidplan

## Besiktningsman / oberoende kontroll

Ansvar:
- kontroll mot avtal och krav
- identifiera avvikelser och restpunkter
- dokumentera resultat

AI-stöd:
- omvandla besiktningsanteckningar till tydliga Issues
- gruppera avvikelser per ansvarig roll
- följa upp att kritiska punkter stängs före slutleverans

## Princip: varje roll uppdaterar sin del

Varje roll förväntas använda sin egen ChatGPT eller Codex för att:

1. läsa relevanta Issues innan arbetet startar
2. dokumentera vad som har gjorts
3. registrera avvikelser direkt
4. uppdatera status och blockerare
5. skapa nya Issues när nytt arbete upptäcks
6. uppdatera relevanta projektfiler
7. lämna en tydlig överlämning till nästa roll

På så sätt blir GitHub den gemensamma sanningen medan varje deltagare har sin egen AI-projektassistent.

## RACI

| Aktivitet | Byggherre | Huvudentreprenör | VVS | El | Snickare | Plattsättare | Besiktning |
|---|---|---|---|---|---|---|---|
| Mål och budget | A/R | C | I | I | I | I | I |
| Planering och samordning | C | A/R | C | C | C | C | I |
| VVS-installation | I | A | R | I | C | C | I |
| Elinstallation | I | A | I | R | C | C | I |
| Underlag/stomme | I | A | C | C | R | C | I |
| Tätskikt/plattsättning | I | A | C | I | C | R | I |
| Ändringsbeslut | A/R | C | C | C | C | C | I |
| Slutkontroll | A | R | C | C | C | C | R |

R = Responsible, A = Accountable, C = Consulted, I = Informed.
