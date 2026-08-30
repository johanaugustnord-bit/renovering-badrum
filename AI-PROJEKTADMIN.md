# AI som projektadministratör

Det här repot visar hur AI kan användas för projektadministration i ett fysiskt projekt. GitHub är gemensam system-of-record: Issues beskriver arbete, projektfiler beskriver krav, beslut, budget och kvalitet, och Pull Requests kan användas för kontrollerade förändringar.

Grundprincipen är **agent-per-roll**: byggherren, huvudentreprenören, rörmokaren, elektrikern, snickaren och plattsättaren använder varsin ChatGPT eller Codex som administrativ assistent mot samma repo.

## ChatGPT Work

ChatGPT Work passar när uppgiften handlar om att samla kontext, analysera status, skapa beslutsunderlag och arbeta över flera informationskällor.

Exempel:
- sammanfatta öppna Issues och blockerare
- jämföra offerter
- skapa veckostatus per roll
- identifiera aktiviteter utan ansvarig
- föreslå följd-Issues efter ett beslut
- kontrollera att kvalitetsgrindar är dokumenterade
- skapa beslutsunderlag inför produktval eller ändringar

### Exempelprompt: byggherre

> Gå igenom öppna Issues, budget, tidplan och beslut. Sammanfatta projektläget, vilka beslut jag behöver fatta och vilka tre risker som kan påverka kostnad eller sluttid mest.

### Exempelprompt: huvudentreprenör

> Gå igenom alla öppna Issues. Gruppera dem per yrkesroll, identifiera blockerare och beroenden och skapa en samordningslista för nästa arbetsdag.

### Exempelprompt: yrkesroll

> Läs de Issues som berör VVS. Sammanfatta vad som ska göras, vad som blockerar arbetet och vilken dokumentation som ska lämnas innan nästa yrkesgrupp tar över.

## Codex CLI

Codex CLI passar när projektet finns som ett lokalt Git-repository och AI-agenten ska arbeta direkt med filer och Git-historik.

Typiskt flöde:
1. Klona repot.
2. Starta Codex i repots katalog.
3. Be Codex läsa `AGENTS.md`, relevanta Issues och projektfiler.
4. Låt Codex uppdatera Markdown-filer, checklistor och status.
5. Låt större förändringar ske på branch och via Pull Request.
6. Granska innan merge.

Exempelprompt:

> Läs AGENTS.md och projektfilerna. Jag är elektriker i projektet. Gå igenom relevanta Issues, identifiera vad jag kan starta nu, vad som blockerar mig och vilka uppdateringar jag bör göra i repo:t efter dagens arbete. Ändra inte andra yrkesgruppers ansvar utan att skapa en fråga eller ett Issue.

## Varför detta fungerar

Varje deltagare behöver inte kunna GitHub på expert-nivå. Den egna AI-assistenten kan översätta vanlig projektkommunikation till strukturerade GitHub-uppdateringar.

Exempel:

> "Golvvärmen är installerad men vi kunde inte färdigställa termostaten eftersom väggen inte är klar."

AI-assistenten kan då föreslå att:
- relevant el-Issue uppdateras
- blockeraren kopplas till snickarens Issue
- en restpunkt skapas om det behövs
- huvudentreprenören informeras genom projektstatus

## Ansvarsgräns

AI:n är projektadministratör, inte behörig fackman. Tekniska, regulatoriska och säkerhetskritiska beslut ligger kvar hos respektive ansvarig människa och behörig yrkesroll.
