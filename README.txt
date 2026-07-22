CESTA DO ISTANBULU – NÁVOD K AKTUALIZACI
========================================

Web je hotový a stačí nahrát celý obsah této složky na hosting.
Soubor index.html musí zůstat v hlavní složce.

JAK PŘIDAT ODKAZ NA FOTOALBUM
-----------------------------
1. Otevři soubor js/content.js.
2. Najdi řádek:
   albumUrl: "",
3. Mezi uvozovky vlož odkaz na Google Fotky:
   albumUrl: "https://photos.app.goo.gl/TVUJ-ODKAZ",

JAK PŘIDAT NOVÝ DEN
-------------------
Upravuje se pouze soubor js/content.js.

Uvnitř days: [ ... ] zkopíruj tento vzor a vlož ho za předchozí den:

    {
      day: 3,
      title: "Svätý Ján → další místo",
      paragraphs: [
        "První odstavec.",
        "Druhý odstavec.",
        "Třetí odstavec."
      ]
    }

DŮLEŽITÉ:
- Mezi jednotlivými dny musí být čárka.
- Mezi odstavci musí být čárka.
- Text každého odstavce musí být mezi uvozovkami.
- Nepoužívej uvnitř textu obyčejné dvojité uvozovky. Nahraď je českými „uvozovkami“.
- Potom nahraj na hosting pouze změněný soubor js/content.js.

STRUKTURA WEBU
--------------
index.html       hlavní stránka
css/style.css    vzhled webu
js/content.js    všechny texty a odkaz na album – TENTO SOUBOR AKTUALIZUJ
js/app.js        vykreslení obsahu – není potřeba upravovat
assets/          ikona webu
