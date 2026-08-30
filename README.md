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
- `projekt/roller-och-ansvar.md` – byggherre, huvudentreprenör, yrkesroller och RACI
- `AI-PROJEKTADMIN.md` – hur ChatGPT Work och Codex CLI används i projektadministrationen
- `AGENTS.md` – arbetsregler för Codex och principen agent-per-roll
- `inkop/materiallista.md` – produkter, material och beställningsstatus
- `leverans/slutkontroll.md` – slutbesiktning och överlämning

## Agent-per-roll

Projektet bygger på att varje mänsklig roll kan ha sin egen AI-assistent. Byggherre, huvudentreprenör, rörmokare, elektriker, snickare, plattsättare och andra deltagare förväntas kunna använda sin egen ChatGPT eller Codex för att administrera sitt arbete mot samma repo.

AI-assistenten kan läsa relevanta Issues, uppdatera status, dokumentera avvikelser, skapa följdaktiviteter och lämna en tydlig överlämning till nästa roll. Yrkesansvaret ligger fortfarande hos människan; AI:n fungerar som projektadministrativt stöd.

## Exempel på arbetsflöde

1. Ett behov eller problem skapas som ett Issue.
2. Ansvarig roll och nästa steg tydliggörs.
3. Rollens egen ChatGPT eller Codex läser relevant projektkontext och hjälper till att hålla Issue och dokumentation aktuella.
4. Om frågan innebär en större förändring dokumenteras förslaget separat och kan hanteras via Pull Request.
5. När beslut fattas uppdateras relevant projektdokumentation.
6. Commit-historiken visar exakt vad som ändrats och när.
7. Ett GitHub Project kan användas för status som `Planerat`, `Beslut krävs`, `Beställt`, `Pågår`, `Kontroll` och `Klart`.

## AI som projektadministratör

Se `AI-PROJEKTADMIN.md` för praktiska exempel med ChatGPT Work och Codex CLI.

Exempelprompt:

> Gå igenom badrumsprojektet utifrån min roll. Sammanfatta vad jag ansvarar för, vad som blockerar mitt arbete, vilka Issues jag bör uppdatera och vad nästa yrkesroll behöver veta innan överlämning.

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
