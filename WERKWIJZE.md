# Werkwijze

Hoe ik Coachboard Lite bouw, met AI. Kort gezegd: AI verkent en bouwt, ik kies en controleer, en ik schrijf op waarom.

> AI versnelt mijn werk. Ik gebruik het om sneller te proberen, niet om minder te snappen.

## Wie doet wat

| Wie | Doet |
|---|---|
| Ik | Bepaal het doel, kies tussen opties, keur teksten goed, lees elke pull request en voeg hem samen. |
| Claude (claude.ai) | Zet opties naast elkaar, verkent ontwerpen op het canvas en schrijft concepten. |
| Claude Code | Bouwt in een branch, draait de controles en opent een pull request met uitleg. |
| Figma | Het gekozen ontwerp. Daaruit wordt gebouwd. |
| GitHub | Pull requests, CI en de geschiedenis. |

## Elke stap gaat zo

1. **Doel.** Wat moet het opleveren, en wanneer is het klaar?
2. **Opties.** Twee of drie manieren, met voor- en nadelen.
3. **Keuze.** Ik kies. De keuze komt in [BESLISSINGEN.md](BESLISSINGEN.md): wat, waarom en het alternatief.
4. **Ontwerp.** Alleen als de stap een scherm heeft: verkennen op het Claude-canvas, afmaken in Figma.
5. **Bouwen.** Claude Code werkt in een branch `fase-N-<naam>`, in kleine commits.
6. **Controleren.** De machine: typecheck, tests, build, toegankelijkheid en budget. Ik: de code lezen en het op mijn telefoon proberen.
7. **Vastleggen.** In de pull request: wat AI maakte, wat ik veranderde en wat ik controleerde.

## Afspraken met AI

- Teksten komen van mij. AI stelt voor, ik keur goed. Een ontbrekende tekst wordt gevraagd, niet verzonnen.
- Niets komt op `main` zonder mijn review. Claude Code zet niets live.
- Een commit pas als alle controles groen zijn.
- Code die ik niet kan uitleggen, gaat er niet in.
- Commentaar in de code zegt waarom, niet wat.
- Wat we bewust niet bouwen, is ook een keuze en staat in het log.

## Wat ik vastleg

- **[BESLISSINGEN.md](BESLISSINGEN.md):** elke keuze in drie regels, met datum.
- **Pull requests:** wat AI maakte, wat ik veranderde en wat ik controleerde. Het sjabloon staat in `.github/pull_request_template.md`.
- **Metingen:** groottes en Lighthouse per fase, zoals in Coachboard en kayhardam.dev.
