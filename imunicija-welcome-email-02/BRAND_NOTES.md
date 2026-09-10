# IMUNICIJA — Welcome 02: padėkime išsirinkti

Sukurta 2026-09-10. Skirta siųsti praėjus 1 dienai nuo prenumeratos, tik dar nenusipirkusiems ir prenumeratos neatsisakiusiems kontaktams. Jei seka prasideda 20 min. laukimu prieš pirmą laišką, iki šio laiško papildomai laukti 23 val. 40 min. Trečias laiškas planuojamas po 3 dienų nuo prenumeratos; šiame darbe nekuriamas. Gyva automatizacija nekurta.

## Tema ir reference

Tema: Kokia technika praverstų jūsų kasdienybei?
Peržiūros tekstas: Darbui, ryšiui ar laisvalaikiui — atraskite savo kategoriją.

Reference: kliento patvirtintas ../imunicija-welcome-email/newsletter.html ir assets/reference/approved-email-01.jpg. Pirmasis laiškas nepakeistas (SHA256 5a7a925cb91d22181fa81a866855a19e03c6c026ad56a89fba83e5bf6b276dd5). Taikytas brand-dna ir build-reference-email workflow. Tai nuolatinė pasisveikinimo seka, todėl pasirinkimo tema išlaikyta nepriklausoma nuo sezono.

Išlaikyta 600 px lentelinė struktūra, nuo viršaus prasidedantis hero, tikras baltas logotipas, Inter / Arial / Helvetica šriftų kryptis, #20B200 žali stačiakampiai CTA, #333E48 tekstas, #2F3338 kupono kortelė ir poraštė. #F3F5F1 – pagalbinis šviesus atmintinės tonas. Hero fotografija pakartotinai naudojama iš patvirtinto laiško; pakeista HTML antraštė. Trys poreikių blokai su vienu pavyzdiniu produktu: kompiuteriai, telefonai, konsolės. Vaizdai ir CTA veda į kategorijas, ne į pavienius SKU. Apačioje patvirtinto stiliaus nemokamo siuntimo kortelė su vartotojo kodu LABASS.

## Šaltiniai ir vaizdų kilmė

Brand profilis: ../brands/imunicija/BRAND-DNA.md. Pilna naudojamos AI hero fotografijos ir packshotų retušavimo kilmė / promptai: ../imunicija-welcome-email/BRAND_NOTES.md. Šiame etape naujų AI vaizdų negeneruota; naudojamos patvirtintos versijos be IMUNICIJA.LT watermarko. Hero yra AI fotografijos interpretacija, ne dokumentinė produkto būklės nuotrauka. Packshotų vandens ženklo uždengtos sritys anksčiau atkurtos generatyviai.

Oficialus baltas logotipas: https://imunicija.lt/wp-content/uploads/2026/06/Photoroom_20260626_122220-e1782468565525.png
Samsung šaltinis: https://imunicija.lt/wp-content/uploads/2025/12/download-6.webp
Lenovo šaltinis: https://imunicija.lt/wp-content/uploads/2026/09/download-7.png
Nintendo šaltinis: https://imunicija.lt/wp-content/uploads/2025/08/download-31.png

Kategorijos:
- https://imunicija.lt/produkto-kategorija/kompiuteriai/
- https://imunicija.lt/produkto-kategorija/telefonai/
- https://imunicija.lt/produkto-kategorija/konsoles/

Patarimai parašyti kaip pagalba renkantis, ne universalūs techninių parametrų ar garantijos pažadai. Nepateikiamos kainos, likučiai, reitingai, atsiliepimai, konkretus bendras garantijos terminas ar nepatvirtinta kupono galiojimo pabaiga. Pirminiai šaltiniai: https://imunicija.lt/garantija-ir-grazinimas/ ir produktų aprašymai ankstesniame brand tyrime. Pakartotinio tikrinimo metu dalis tiesioginių svetainės užklausų grąžino timeout / redirect klaidas; kategorijos anksčiau patikrintos šioje sesijoje ir pateikiamos dabartinio kontaktų puslapio navigacijoje. Kontaktai patvirtinti per https://imunicija.lt/kontaktai/ : UAB Imunicija, info@imunicija.lt, Geležinkelio g. 6 Vilnius, Pramonės g. 15 Šiauliai.

## Perkėlimas į Omnisend

Tai lokalus peržiūros maketas. Prieš siunčiant įkelti penkis naudojamus assetus į Omnisend / HTTPS talpyklą ir pakeisti src, background, CSS url bei VML src:
- assets/hero-v2.jpg
- assets/brand/logo-white.png
- assets/products/lenovo-x13.jpg
- assets/products/samsung-s21.jpg
- assets/products/nintendo-switch.jpg

LABASS pateikė vartotojas; jo aktyvumas ir kupono taisyklė parduotuvėje čia nekonfigūruoti. Atsisakymo žyma [[unsubscribe_link]] perkelta iš pirmojo laiško; patikrinti jos pakeitimą gavimo teste. Siuntimo sąlygos: užsiprenumeravęs, dar nepirkęs, išėjimas po pirkimo / atsisakymo. Jokie laiškai nesiųsti.

## Galutinė patikra

Desktop 800 × 1000 viewport, apkirptas 600 × 3611 px laiškas; mobile 390 × 3430 px. Patikrinti 800, 390 ir 320 px pločiai: nėra horizontalaus perpildymo, visi vaizdai įkeliami. Abu galutiniai vaizdai peržiūrėti vizualiai. Po pirminės peržiūros sutrumpintos pasikartojančios blokų etiketės į „DARBUI“, „RYŠIUI“, „LAISVALAIKIUI“, 320 px ekrane įdėtas vertikalus nuotraukos / teksto išdėstymas. HTML lentelės role=presentation, visi img turi alt ir dydžius, visi vietiniai assetai egzistuoja, HTML ir TXT nuorodos sutampa (mailto normalizuota). Kuponas LABASS abiejose versijose. Pirmojo patvirtinto HTML SHA256 nepakito. Tai naršyklės patikra; prieš siunčiant atlikti ESP gavimo testą.


## Skirtingi hero kiekvienam laiškui — 2026-09-10

Vartotojo prašymu hero pakeistas į naują, šiam laiškui skirtą produkto fotosesijos interpretaciją. Naudojamas assets/hero-v3.jpg; pilna generacija assets/hero-v3-original.png. Ankstesnė hero-v2.jpg išsaugota archyvui, laiške nebevartojama. Perkeliant į ESP naudoti hero-v3.jpg vietoje ankstesnio hero. HTML / VML nuorodos pakeistos. Naudotas builtin image_gen.imagegen įrankis, ne CLI. Tai AI produkto scenos interpretacija. Tikras logotipas ir laiško tekstas išliko atskirais HTML elementais. Abu esami laiškai vartotojo nurodymu dabar turi skirtingas hero fotografijas.

Generacijos failas: /Users/ugniusstakauskas/.codex/generated_images/01a08a73-d5a8-71a2-a0c1-7be485f9cbeb/exec-d3ffa7bc-95e7-4e96-872f-8c3d5aa63c23.png

Promptas:

Use case: product-mockup. Create a new high-end editorial product campaign photograph for Imunicija electronics. The first reference is the exact product identity and shape to preserve; second reference is ONLY the approved photographic art direction, not a composition to duplicate. Photorealistic premium product photoshoot, understated art direction, true material texture, sophisticated soft window light, deep charcoal with a subtle forest-green undertone, restrained warm neutrals, crisp plausible hardware, honest reflections and contact shadows. No people. No retailer watermark, no added text, no promotional typography, no logo overlays. Preserve authentic manufacturer markings where visible. Portrait 4:5 composition. CRITICAL newsletter composition: the entire upper 42% is a nearly black charcoal green wall with subtle texture, no objects and no bright spots, reserved for HTML white logo/headline. Hero product entirely in lower 48%-87%, within central 66% of image width to survive narrow mobile crop. Product must be recognisable, physically accurate, not floating. Avoid CGI showroom perfection, fake glow, fog, oversaturated green, strange perspective, extra buttons or distorted keyboard/controls. Scene for welcome email 02: white Nintendo Switch OLED with both white Joy-Cons attached, displayed upright naturally supported by its own kickstand on a dark warm walnut console table, directly facing camera at a subtle three-quarter angle, full device clearly visible. Preserve original two controllers, thumbsticks, button layout, black bezels, exact Nintendo Switch logo and colourful gradient screen from product reference. Device centrally positioned in the lower half, spanning about 66% of image width. A quiet high-end residential entertainment corner, deep charcoal forest-green plaster wall above, no TV, no controller duplicates, no dock, no other electronics. Daylight grazing the white controller shells from the right, realistic warm walnut grain, subtle clean specular reflection on glass. One small folded neutral linen textile at far lower left as background detail only. Editorial luxury product still life, honest lens rendition, rich blacks, no theatrics, looks photographed on location.

Hero atnaujinimo QA: desktop ir 390 px mobile vaizdai peržiūrėti su tikru logotipu ir HTML tekstu. Mobilus background-position koreguotas į 25% center, kad būtų išlaikytas produktas kadre. JPG/PNG peržiūros ir ZIP atnaujinti; turinys ir LABASS kodas išliko.


## Šeši poreikiai ir žmogiškesnė hero antraštė

Vartotojo prašymu antras laiškas išplėstas iš 3 į 6 poreikių blokus: darbui ir mokslams, kasdieniam bendravimui, žaidimų vakarams, naršymui ir skaitymui, sportui ir judėjimui, filmams ir serialams. Hero antraštė: „Kokia technika praverstų jums?“ Išlaikyta poreikiams tinkamos technikos idėja.

Papildomi trys packshotai nukopijuoti iš pirmo laiško galutinių, jau retušuotų failų be vandens ženklų; naujų AI generacijų nereikėjo. Papildomos siuntimo priklausomybės: assets/products/acer-iconia.jpg, assets/products/huawei-fit-se.jpg, assets/products/konka-tv.jpg. Vaizdų šaltiniai ir retušo kilmė: ../imunicija-welcome-email/BRAND_NOTES.md. Kategorijų URL perimti iš tame pačiame darbe patikrinto pirmojo laiško: https://imunicija.lt/produkto-kategorija/plansetes/ , https://imunicija.lt/produkto-kategorija/laikrodziai/ , https://imunicija.lt/produkto-kategorija/vaizdo-technika/televizoriai/ . Patarimai bendri pasirinkimo kriterijai; konkrečios įrenginio funkcijos nežadamos.

Šešių poreikių QA: desktop 600 × 4477 px, mobile 390 × 4351 px. Abiejose versijose visos nuotraukos įkeliamos, šeši blokai, nėra horizontalaus perpildymo. Hero tekstas ir pridėtos kortelės peržiūrėti vizualiai. Po pirminės peržiūros įžanga suderinta su platesniu poreikių pasirinkimu. HTML/TXT nuorodos sutampa; vietiniai assetai egzistuoja. JPG/PNG ir ZIP atnaujinti.
