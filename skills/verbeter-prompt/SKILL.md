---
name: verbeter-prompt
description: "Verbeter een aangeleverde of direct voorafgaande prompt volgens de officiële OpenAI-richtlijnen, toon de herschreven versie en wacht op akkoord voordat je de onderliggende opdracht uitvoert. Gebruik bij $verbeter-prompt of verzoeken om eerst een prompt te verbeteren en daarna pas uit te voeren."
---

# Verbeter prompt

## Werkwijze

1. Bepaal welke prompt de gebruiker bedoelt. Neem bij "de vorige prompt" de laatste expliciete taakprompt in de conversatie, niet omgevingsmetadata of instructies van het systeem. Vraag om de tekst als meerdere kandidaten plausibel zijn en de keuze niet uit de context blijkt.
2. Bepaal het beoogde resultaat, de relevante context, harde beperkingen en gewenste output. Behoud de bedoeling en alle materiële eisen. Verzin geen feiten, toestemming, toegang of nieuwe inhoudelijke voorwaarden.
3. Herschrijf helder en beknopt. Scheid invoer, taak, beperkingen en output alleen waar dat de uitvoering duidelijker maakt. Benoem een controleerbare voltooiingsvoorwaarde bij meerstapswerk. Vermijd onnodige rollen, rituelen, redundantie en instructies om interne denkstappen te tonen.
4. Baseer OpenAI-specifieke claims op officiële OpenAI-documentatie. Controleer de actuele richtlijn op een officiële OpenAI-site als de gebruiker een actuele vergelijking of onderbouwing vraagt. Kopieer geen lange passages.
5. Toon precies één direct bruikbare, kopieerbare verbeterde prompt. Licht hooguit kort toe welke wezenlijke verduidelijkingen je aanbracht. Vraag om expliciet akkoord met deze versie en beëindig de beurt zonder de onderliggende opdracht uit te voeren.
6. Voer na het akkoord de goedgekeurde opdracht uit. Neem aanvullende wijzigingen van de gebruiker mee. Vraag alleen opnieuw akkoord als de gebruiker de prompt wezenlijk wijzigt of als een afzonderlijke vereiste toestemming nog ontbreekt.

## Uitvoer

Geef de prompt in de taal van de gebruiker, tenzij die een andere taal vraagt. Gebruik deze compacte vorm:

**Verbeterde prompt**

> [De volledige prompt, met passende alinea's of korte lijst bij complexiteit.]

[Eén of twee zinnen over de belangrijkste verbetering, indien nuttig.]

**Akkoord met deze versie?**

Als de gebruiker uitsluitend om herschrijven vraagt, bied dan geen uitvoering van de onderliggende taak aan.

## Referentie

- [OpenAI Prompt engineering](https://developers.openai.com/api/docs/guides/prompt-engineering)
- [OpenAI Reasoning best practices](https://developers.openai.com/api/docs/guides/reasoning-best-practices)
