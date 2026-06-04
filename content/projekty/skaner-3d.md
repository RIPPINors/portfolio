---
title: "Skaner oparty o infrastrukturę drukarki 3D"
date: 2026-05-15
github_url: "https://github.com/twoj-profil/skaner-3d"
summary: "Projekt mechatroniczny wykorzystujący kinematykę drukarek 3D (paski zębate vs śruby pociągowe) do precyzyjnego skanowania przestrzennego. Sterowanie oparte na mikrokontrolerach i modelowanie w MATLABie."
tags: ["Mechatronika", "Kinematyka", "MATLAB", "Hardware"]
draft: false
---

<div class="bg-blue-50 border-l-4 border-blue-600 p-4 mb-6">
    <p class="text-sm font-mono text-blue-800 m-0"><strong>Status projektu:</strong> Zakończony (Wiosna 2026) <br>
    <strong>Promotor:</strong> dr inż. Adam Myszkowski</p>
</div>

### Założenia projektowe

Celem projektu było przekształcenie standardowej infrastruktury mechanicznej znanej z drukarek 3D w precyzyjny skaner przestrzenny. Wykorzystałem do tego płaskie schematy inżynierskie, aby poprawnie zamodelować układ.

Podczas analizy napędów kluczowe było zdefiniowanie parametrów silników krokowych. W dokumentacji technicznej skupiłem się na wyznaczeniu oporu uzwojenia ($R$), momentu bezwładności ($J$), stałej momentu ($K_t$) oraz współczynnika tłumienia wiskotycznego ($B$).

### Kinematyka układu

Analiza porównawcza obejmowała dwa typy przeniesienia napędu:
* **Paski zębate (CoreXY / Cartesian):** Szybsze pozycjonowanie głowicy skanującej, lecz podatne na rezonanse.
* **Śruby pociągowe:** Większa rozdzielczość na osi Z, kluczowa przy gęstym próbkowaniu detali.
