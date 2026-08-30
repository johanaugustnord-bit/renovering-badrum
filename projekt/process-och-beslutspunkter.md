# Process och beslutspunkter

Detta projekt drivs som en enkel stage-gate-process. Varje fas har en tydlig beslutspunkt. Projektet går inte vidare till nästa fas förrän rätt underlag finns, berörda roller har lämnat sin input och byggherren eller utsedd beslutsägare har godkänt nästa steg.

## Översikt

1. Förstudie och nuläge
2. Målbild och krav
3. Entreprenad och budget
4. Projektering och beställning
5. Rivning och verifiering
6. Installationer och underarbete
7. Tätskikt
8. Ytskikt och slutinstallation
9. Slutkontroll
10. Överlämning

Varje fas avslutas med en beslutspunkt: Go, Go med villkor eller No-Go.

## BP0 – Starta projektet

Beslutsfråga: Ska badrumsrenoveringen startas som ett definierat projekt?

Minimikrav:
- syfte och mål finns
- byggherre är identifierad
- preliminär budgetram finns
- projektets GitHub-repo och arbetssätt är etablerade
- roller och åtkomstmodell är definierade

Beslutsägare: Byggherre.

Utfall:
- Go: projektet går till förstudie
- Go med villkor: start tillåts men angivna brister måste stängas
- No-Go: projektet pausas eller omdefinieras

## BP1 – Godkänn nuläge och kravbild

Beslutsfråga: Har vi tillräckligt underlag för att bestämma vad som ska byggas?

Minimikrav:
- mått och nuläge är dokumenterade
- befintliga installationer är kända på tillräcklig nivå
- funktionskrav och estetiska krav är dokumenterade
- preliminär planlösning finns
- öppna osäkerheter är identifierade

Berörda roller: Byggherre, huvudentreprenör, VVS, el, snickare.

AI-stöd per roll:
Varje roll använder sin egen ChatGPT/Codex för att kontrollera att just deras fackområde har tillräckligt underlag och för att skapa eller uppdatera relevanta Issues.

Beslutsägare: Byggherre.

## BP2 – Godkänn budget och entreprenadupplägg

Beslutsfråga: Är omfattning, kostnadsbild och ansvarsfördelning tillräckligt tydliga för att gå vidare?

Minimikrav:
- offerter är jämförda
- entreprenadform och huvudentreprenör är valda
- budget och reserv är beslutade
- ansvar och gränssnitt mellan yrkesroller är dokumenterade
- större avtalsmässiga risker är identifierade

Beslutsägare: Byggherre.

## BP3 – Frisläpp inköp och byggstart

Beslutsfråga: Är projekteringen tillräckligt mogen för beställningar och byggstart?

Minimikrav:
- planlösning är fastställd
- måttkritiska produkter är valda
- VVS- och elprinciper är bekräftade
- kritiska leveranstider är kända
- materiallista är uppdaterad
- beroenden i tidplanen är synliga

Berörda roller: Huvudentreprenör, VVS, el, snickare, plattsättare.

Beslutsägare: Huvudentreprenör rekommenderar; byggherre godkänner större ekonomiska eller funktionella åtaganden.

## BP4 – Godkänn förutsättningar efter rivning

Beslutsfråga: Kan projektet fortsätta enligt plan efter att konstruktioner och installationer blivit synliga?

Minimikrav:
- stomme och underlag är inspekterade
- VVS och golvbrunn är verifierade
- dolda skador eller avvikelser är dokumenterade
- nya Issues finns för upptäckta avvikelser
- budget- och tidplanepåverkan är bedömd

Detta är en kritisk beslutspunkt eftersom verkliga förutsättningar ofta avviker från antaganden före rivning.

Beslutsägare: Huvudentreprenör tillsammans med berörda fackroller; byggherren godkänner större ändringar.

## BP5 – Frisläpp tätskikt

Beslutsfråga: Är underlag, VVS och el färdiga så att tätskikt kan utföras utan att behöva öppnas igen?

Minimikrav:
- dolda VVS-arbeten är verifierade och dokumenterade
- dolda elarbeten är verifierade och dokumenterade
- förstärkningar och underlag är klara
- fall och golvförutsättningar är kontrollerade
- inga öppna blockerande avvikelser finns

Beslutsägare: Huvudentreprenör, med explicit klartecken från VVS, el, snickare och plattsättare inom respektive ansvarsområde.

Varje roll förväntas låta sin egen AI-agent kontrollera öppna Issues och relevant dokumentation före klartecken.

## BP6 – Frisläpp plattsättning

Beslutsfråga: Är tätskiktet komplett, verifierat och dokumenterat innan det täcks?

Minimikrav:
- tätskiktssystem är dokumenterat
- genomföringar, hörn och anslutningar är kontrollerade
- fotodokumentation finns
- relevanta egenkontroller eller intyg finns eller är refererade
- inga blockerande avvikelser återstår

Beslutsägare: Plattsättare ansvarar för sitt utförande; huvudentreprenör verifierar att projektets kvalitetsgrind är passerad.

## BP7 – Godkänn installation och färdigställande

Beslutsfråga: Är ytskikten tillräckligt färdiga och korrekta för slutinstallationer och funktionstest?

Minimikrav:
- kakel och klinker är kontrollerade
- fogar och anslutningar är utförda
- mått för slutinstallationer är verifierade
- restpunkter är dokumenterade

Beslutsägare: Huvudentreprenör.

## BP8 – Godkänn slutkontroll

Beslutsfråga: Är badrummet tekniskt och funktionellt färdigt?

Minimikrav:
- VVS är provat
- el är provad
- ventilation är kontrollerad där relevant
- dörrar, inredning och beslag fungerar
- visuella och funktionella restpunkter är registrerade
- kritiska avvikelser är stängda

Beslutsägare: Byggherre med stöd av huvudentreprenör och vid behov oberoende besiktningsman.

## BP9 – Överlämna och stäng projektet

Beslutsfråga: Är både badrummet och projektets dokumentation färdiga för överlämning?

Minimikrav:
- slutkontroll är godkänd
- garantier och intyg är samlade
- installerade produkter och modeller är dokumenterade
- slutlig budget/prognos är uppdaterad
- kvarvarande restpunkter har ägare och datum
- slutliga beslut är dokumenterade

Beslutsägare: Byggherre.

## Hur beslutspunkter representeras i GitHub

Varje beslutspunkt bör representeras av ett eget Issue med en checklista. Relevanta arbets-Issues länkas till beslutspunkten. Beslutet dokumenteras i Issue-tråden och i `projekt/beslut.md`.

Större förändringar mellan två beslutspunkter kan hanteras med en Pull Request. PR:n fungerar då som ett formellt ändringsförslag med konsekvenser för funktion, kostnad, tid och yrkesgrupper.

En beslutspunkt ska aldrig stängas enbart därför att kalenderdatumet passerats. Den stängs när beslutskriterierna faktiskt är uppfyllda och ett beslut är fattat.

## AI-agenternas roll i processen

Varje mänsklig roll använder sin egen ChatGPT eller Codex som projektadministrativ agent. Inför en beslutspunkt kan respektive agent exempelvis få instruktionen:

> Gå igenom öppna Issues och projektdokument som berör min roll. Bedöm om vi kan ge klartecken till nästa beslutspunkt. Lista först blockerare, därefter risker och till sist vilka underlag som saknas. Uppdatera inte andra rollers bedömningar.

Huvudentreprenörens agent kan sedan sammanställa rollernas status och byggherrens agent kan kontrollera beslutsunderlaget inför Go/No-Go.

Det skapar en distribuerad projektadministration: varje yrkesroll ansvarar för sitt fackområde och sin information, medan GitHub utgör den gemensamma sanningskällan.