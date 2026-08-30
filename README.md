# Renovering badrum

Det här är ett publikt demonstrationsprojekt som visar hur GitHub kan användas för att styra en fysisk badrumsrenovering – inte bara mjukvaruutveckling.

## Syfte

Projektet ska visa hur GitHub kan fungera som gemensam projektmiljö för:

- planering och aktiviteter
- krav och målbild
- beslut och ändringshistorik
- budget och inköp
- dokumentation och kvalitetskontroll
- samarbete mellan beställare, hantverkare och AI-agenter

Tanken är att projektets aktuella sanning alltid ska gå att hitta här, i stället för att spridas mellan mejl, sms, kalkylblad och muntliga överenskommelser.

## Så används GitHub i projektet

| GitHub-funktion | I badrumsrenoveringen |
|---|---|
| Repository | Projektets gemensamma kunskapsbas |
| Issues | Aktiviteter, frågor, risker och beslut som kräver åtgärd |
| Projects | Visuell planering och status |
| Pull requests | Föreslagna större förändringar innan de godkänns |
| Commits | Spårbar historik över vad som ändrats |
| Markdown-filer | Krav, budget, beslut och kvalitetsplan |
| AI-agent | Projektadministratör, sammanfattare och analytiker |

## Projektstruktur

- `projekt/krav.md` – målbild, funktionella krav och avgränsningar
- `projekt/budget.md` – budgetstruktur och prognos
- `projekt/tidplan.md` – faser, beroenden och milstolpar
- `projekt/beslut.md` – beslutslogg
- `projekt/kvalitet.md` – kvalitetskontroller och dokumentation
- `inkop/materiallista.md` – produkter, material och beställningsstatus
- `leverans/slutkontroll.md` – slutbesiktning och överlämning

## Exempel på arbetsflöde

1. Ett behov eller problem skapas som ett Issue.
2. Ansvarig och nästa steg tydliggörs.
3. Om frågan innebär en större förändring dokumenteras förslaget separat och kan hanteras via Pull Request.
4. När beslut fattas uppdateras relevant projektdokumentation.
5. Commit-historiken visar exakt vad som ändrats och när.
6. Ett GitHub Project kan användas för status som `Planerat`, `Beslut krävs`, `Beställt`, `Pågår`, `Kontroll` och `Klart`.

## AI som projektadministratör

En AI-agent som ChatGPT eller Codex kan arbeta ovanpå repot och exempelvis:

- sammanfatta aktuell projektstatus
- hitta blockerande aktiviteter
- jämföra offerter eller produktalternativ
- skapa inköpslistor
- kontrollera om dokumentation saknas inför nästa byggmoment
- föreslå nya Issues
- skriva veckorapporter
- identifiera beslut som ännu inte dokumenterats

Exempelprompt:

> Gå igenom badrumsprojektet. Sammanfatta vad som är klart, vilka beslut som väntar, vilka aktiviteter som blockerar tidsplanen och vilka tre saker som bör göras härnäst.

## Projektfaser

1. Förstudie och nuläge
2. Krav och design
3. Offerter och val av entreprenörer
4. Inköp
5. Rivning
6. VVS, el och underarbete
7. Tätskikt
8. Ytskikt och installation
9. Kvalitetskontroll
10. Slutbesiktning och överlämning

## Varför detta exempel?

GitHub förknippas ofta med kod, men dess grundmodell handlar egentligen om att hantera förändring, arbete, beslut, dokumentation och samarbete över tid. En badrumsrenovering gör det tydligt att samma modell fungerar även för ett konkret, fysiskt projekt.
