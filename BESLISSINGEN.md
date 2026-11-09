# Beslissingen

Elke keuze in drie regels: wat, waarom en het alternatief. Nieuwe keuzes komen onderaan, met datum. Verandert een keuze, dan komt er een nieuwe die naar de oude verwijst; de oude blijft staan.

## B1. Coachboard opnieuw bouwen, klein en in React

*9 november 2026*

- **Wat:** Coachboard Lite: de kern van Coachboard (één veld, spelers slepen, pijlen, delen via de link), opnieuw gebouwd in React en TypeScript.
- **Waarom:** React en TypeScript staan in de vacatures die ik wil. Omdat ik het product al ken, gaat mijn tijd naar de techniek en de keuzes, niet naar uitzoeken wat het moet doen.
- **Alternatief:** Coachboard zelf ombouwen van Svelte naar React. Dat is groter, en het werkt al goed in Svelte.

## B2. Daarna het veld als WordPress-blok

*9 november 2026*

- **Wat:** Na Lite wordt het veld een blok voor de WordPress-blokeditor.
- **Waarom:** De blokeditor is zelf React, dus het component kan mee. WordPress met de blokeditor staat ook in de vacatures, en een club kan zo een aanval op de eigen site zetten.
- **Alternatief:** Alleen Lite (dan blijft WordPress een gat), of alleen het blok (dan bouw ik binnen de opzet van WordPress en maak ik zelf minder keuzes).

## B3. Claude verkent, Figma beslist

*9 november 2026*

- **Wat:** Ontwerpvarianten verken ik met Claude op het canvas. De gekozen variant gaat naar Figma, en daar werk ik hem af. Er wordt gebouwd vanuit Figma.
- **Waarom:** Verkennen gaat met AI snel. Kiezen en afwerken doe ik zelf, in het gereedschap dat teams gebruiken, en zo is er een Figma-bestand om te laten zien.
- **Alternatief:** Alleen Figma (langzamer verkennen), of alleen het Claude-canvas (geen Figma-bestand en geen overdracht zoals in een team).

## B4. Werkwijze en beslissingen staan openbaar in deze repo

*9 november 2026*

- **Wat:** [WERKWIJZE.md](WERKWIJZE.md) en dit bestand zijn openbaar. In kayhardam.dev blijft `docs/` lokaal, zoals het was.
- **Waarom:** Wie mijn werk bekijkt, ziet niet alleen de code, maar ook hoe ik kies en hoe ik AI gebruik.
- **Alternatief:** Lokaal houden en op de site samenvatten. Dan is er minder om te laten zien.

## B5. Claude staat in de commits

*9 november 2026*

- **Wat:** Commits van Claude staan op mijn naam, met mijn noreply-adres. Onderaan staat Claude als co-auteur, met een link naar de sessie, zoals in Coachboard.
- **Waarom:** De werkwijze is hier het verhaal (B4). Wie de geschiedenis leest, ziet bij elke commit dat AI meedeed, en de pull request zegt wie wat deed.
- **Alternatief:** Geen vermelding, zoals in kayhardam.dev. Dan staat het AI-verhaal alleen in [WERKWIJZE.md](WERKWIJZE.md) en de pull requests.

## B6. Tailwind 4, zuinig gebruikt

*9 november 2026*

- **Wat:** Styling met Tailwind 4. De tokens staan in `@theme`, en een rij klassen die terugkomt, staat één keer in een klein component. Geen UI-kit.
- **Waarom:** Tailwind staat in de vacatures en wil ik leren. De tokens blijven CSS-variabelen en sluiten aan op de variabelen in Figma (B3).
- **Alternatief:** CSS Modules met tokens, zoals in mijn andere projecten. Geen afhankelijkheid, maar dan blijft Tailwind een gat.

## B7. Bouwen, testen en hosten zoals in Coachboard

*9 november 2026*

- **Wat:** React met Vite, zonder framework erbovenop. Testen met Vitest, en met Playwright en axe. Cloudflare Workers serveert alleen de gebouwde bestanden: Workers Builds zet `main` live en geeft elke branch een eigen preview-adres.
- **Waarom:** Dit ken ik al uit Coachboard, dus mijn tijd gaat naar React en Tailwind. Een bord heeft geen server nodig, en met de preview probeer ik elke pull request op mijn telefoon.
- **Alternatief:** Cloudflare Pages, zoals mijn mockup noemde: dat wijkt af van mijn andere sites, en Workers kan meer. Of Next.js, dat een server meebrengt die Lite niet nodig heeft.

## B8. Fase 1: de kern, met een budget

*9 november 2026*

- **Wat:** Eén veld, spelers verplaatsen (slepen en aantikken), één pijl en delen via de link, met een groottebudget in `npm run verify`. Slepen en de stand van het bord doe ik met React zelf, zonder bibliotheek. Nog niet: het toetsenbord (komt in een latere fase), stappen, talen, de QR-code en versies van links.
- **Waarom:** Dit is de kern van Coachboard. Het budget hoort bij Core Web Vitals, die in de vacatures staan, en met aantikken werkt het bord ook zonder slepen (WCAG 2.5.7). Zonder bibliotheek leer ik React zelf, niet een laag erbovenop.
- **Alternatief:** Het budget pas in stap 6 (meten), alleen slepen, of een bibliotheek voor slepen.
