# Service stub – hantverksmarknad för Björn

Detta är en konceptstub för en agentdriven marknadsplats för hantverkare. Syftet är inte att bygga hela tjänsten, utan att bevisa ett sammanhängande flöde från kundbehov till kvalificerad leverantör och projektöverlämning.

## Kärnflöde

1. Kund eller Björn beskriver behovet.
2. Tjänsten normaliserar uppdraget till ett strukturerat `JobRequest`.
3. Leverantörskatalogen matchar yrkesroll, geografi, kompetens och tillgänglighet.
4. Verifieringslagret kontrollerar kända behörigheter/certifieringar och företagsstatus.
5. En shortlist skapas.
6. En RFQ skickas till utvalda leverantörer eller deras AI-agenter.
7. Offerter tas emot i ett standardformat.
8. Björn jämför pris, omfattning, villkor, kapacitet och verifierad historik.
9. Kunden väljer leverantör.
10. Det valda uppdraget lämnas över till ett privat GitHub-projekt med Issues, roller och beslutspunkter.
11. Efter leverans kan faktura, referens och utfall kopplas tillbaka till leverantörsprofilen.

## Avgränsning i stubben

Stubben modellerar följande resurser:

- `Provider` – företag/hantverkare
- `Capability` – yrkesroll och kompetens
- `Verification` – verifierad status från extern källa
- `Availability` – när och var leverantören kan ta jobb
- `JobRequest` – strukturerat kundbehov
- `RFQ` – offertförfrågan
- `Quote` – offert
- `ProjectHandoff` – överlämning till privat projekt
- `Reference` – verifierad referens efter utfört jobb
- `InvoiceEvidence` – bevis på verkligt genomfört och fakturerat uppdrag

## Viktig princip

Tjänsten ska inte själv avgöra om en yrkesperson är juridiskt behörig. Den ska lagra källa, kontrolltidpunkt och verifieringsresultat så att Björn och kunden kan fatta beslut på spårbart underlag.

## E.164

Varje deltagande människa, företag eller agent kan i en senare version ha en E.164-baserad identitet/routingadress. E.164 används då som stabil identifierare för att nå rätt människa eller agent, medan själva transporten kan vara telefoni, messaging, API eller annan agentkommunikation.

## API

Se `api/openapi.yaml` för ett minimalt REST-kontrakt.

## Demo

`data/providers.json` innehåller fiktiva leverantörer för att kunna demonstrera matchning utan att använda verkliga företag.