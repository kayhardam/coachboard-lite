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

## Nog open

Te beslissen voor of in fase 1. De voorstellen komen uit mijn mockup van 2 november.

- **Claude zichtbaar in de commits?** In kayhardam.dev niet (17 oktober 2026), in Coachboard wel. Voorstel voor Lite: wel, omdat de werkwijze hier het verhaal is.
- **Styling:** Tailwind (voorstel, staat in de vacatures) of CSS met tokens, zoals in mijn andere projecten.
- **Bouwen en hosten:** Vite, en Cloudflare zoals mijn andere sites. De mockup noemde Pages; mijn sites draaien op Workers.
- **Scope van fase 1:** één veld, spelers slepen, één pijl, delen via de link. De mockup liet bewust weg: stappen, talen, QR-code, versies van links en groottebudgetten. Voorstel: het groottebudget toch houden, want Core Web Vitals staan in de vacatures.
