---
author: Lektion 10
date: MMMM dd, YYYY
paging: "%d / %d"
---

# Lektion 10

Hej och välkommen!

## Agenda

1. Frågor och repetition
2. Introduktion till Agile och Scrum
3. Gruppövningar
4. Eget arbete med handledning

---

# Gruppövning 1

Låtsas att ni får i uppgift att bygga en e-handelsplattform (webbplats) för en bokaffär. Övningen går ut på att sätta upp ett GitHub repository med issues.

Börja med att skapa ett repository på GitHub och att bjuda in alla i gruppen. Fortsätt med att skapa kort förklarande user stories. Dessa skall sedan beskrivas i mer detalj. Till en början kan det exempelvis se ut såhär (user stories):

- Som användare vill jag kunna söka efter produkter för att hitta specifika varor jag är intresserad av
- Som användare vill jag få upp rekommendationer på varor baserat på tidigare sökningar
- Som användare vill jag se vilka produkter som är populära
- (ni skall lägga till fler här)

Sedan, för att utveckla på dessa user stories kan ni följa denna mall (den innehåller ett exempel som ni skall byta ut):

```markdown
## Beskrivning

Som användare vill jag kunna söka efter produkter för att hitta specifika varor jag är intresserad av.

## Acceptanskriterier

- [ ] Sökfältet ska vara synligt på alla sidor
- [ ] Sökningen ska fungera på produktnamn och beskrivning
- [ ] Resultaten ska visas i en lista med pagination
- [ ] Max 10 resultat per sida visas
- [ ] Tomma sökresultat ska visa ett användarvänligt meddelande

## Tekniska noter

- Implementera sökfunktion med ElasticSearch
- Caching av vanliga sökresultat
- Felhantering vid timeout

## Definition of Done

- [ ] Koden är skriven och testad
- [ ] Dokumentation är uppdaterad
- [ ] Pull request är skapad
- [ ] Code review är genomförd
- [ ] Alla tester går igenom
```

Tänk på att det egentligen inte finns några rätta svar. Ni bestämmer själva vilka issues som är passande. Ni skall dock försöka få de så bra, tydliga och värdefulla som möjligt. Fyll i mallen för alla user stories ni har skapat.

Alla dessa user stories skall läggas in som issues på GitHub.

Ni har inte än kunskaper inom webb, men kan ändå bygga kriterier utan att specificera tekniska detaljer.

---

# Gruppövning 2

Ni har fått in följande bug-reports:

- När användaren klickar på "Lägg till i kundvagn" visas ingen bekräftelse.
- När användaren besöker webbplatsen första gången så visas inga produkter
- Användare kan beställa fler produkter än vad som finns i lager

Skapa GitHub issues för alla dessa buggar. Ni får hitta på vissa saker då buggarna inte är riktiga. Försök, så mycket det går, att koppla dessa till era tidigare skapade issues. Hitta gärna på egna buggar också.

Använd följande mall (den innehåller ett exempel som skall bytas ut):

```markdown
## Beskrivning av buggen

När användaren klickar på "Lägg till i kundvagn" visas ingen bekräftelse.

## Steg att återskapa

1. Gå till valfri produktsida
2. Klicka på "Lägg till i kundvagn"
3. Observera att ingen bekräftelse visas

## Förväntat beteende

En bekräftelse ska visas när produkten läggs till i kundvaggen.

## Faktiskt beteende

Ingen bekräftelse visas, användaren är osäker på om produkten lades till.

## Miljö

- Browser: Chrome 121.0
- OS: Windows 11
- Skärmstorlek: 1920x1080

## Extra information

- Felet uppstår konsekvent
- Produkten läggs till korrekt, endast bekräftelsen saknas
```

---

# Gruppövning 3

Ni har fått in några "feature requests" från användare:

- Implementera dark-mode för sidan och knappar för att bytta mellan det och light-mode
- Visa liknande produkter när man besöker en specifik produkt
- Implementera "hover" funktionalitet som visar en kort beskrivning av produkter

Skapa GitHub issues för alla dessa feature requests. Ni får hitta på vissa saker då ni inte har ett riktigt projekt att jobba med. Försök, så mycket det går, att koppla dessa till era tidigare skapade issues. Hitta gärna på andra requests om ni vill.

Använd följande mall (den innehåller ett exempel som skall bytas ut):

```markdown
## Funktionsbeskrivning

Implementera dark mode för hela webbplatsen.

## Motivation

Många användare föredrar dark mode, särskilt vid användning nattetid.

## Föreslagen implementation

- [ ] Lägg till toggle för dark/light mode
- [ ] Skapa variabler för färgteman
- [ ] Spara användarens preferens lokalt
- [ ] Respektera systemets färgtema som default

## Påverkan

- UI/UX components
- Färgschema
- Användarinställningar

## Alternativa lösningar

- Automatisk dark mode baserat på tiden på dygnet
- Endast följa systemets inställningar
```
