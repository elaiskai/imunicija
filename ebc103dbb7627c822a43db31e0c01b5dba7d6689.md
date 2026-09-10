# IMUNICIJA — Welcome 03: priminimas ir pagalba

Sukurta 2026-09-10. Tema: Dar renkatės? Padėsime.
Peržiūros tekstas: Jūsų nemokamo siuntimo kodas — LABASS.

## Vieta sekoje

Trečias laiškas po 3 dienų nuo registracijos, t. y. praėjus 2 dienoms po antro laiško. Siųsti tik prenumeratos neatsisakiusiems kontaktams, kurie dar nenupirko. Po pirkimo ar atsisakymo likusią welcome seką nutraukti. Automatizacija šiame darbe nekonfigūruota, laiškai nesiųsti.

## Reference ir turinys

Vartotojo nurodytas reference – patvirtintas pirmasis laiškas: ../imunicija-welcome-email/newsletter.html; jo JPG kopija assets/reference/approved-email-01.jpg. Pirmojo ir antrojo laiškų failai nekeičiami. Taikomi brand-dna, build-reference-email ir imagegen skillai. Tema pagal patvirtintą planą: ramus priminimas, atsakymai į tris pirkimo klausimus ir kvietimas sugrįžti į parduotuvę. Tai nuolatinės sekos laiškas, todėl sezoninės datos ir terminai nereikalingi.

Išlaikytas 600 px email konteineris, Inter / Arial / Helvetica, oficialus baltas logotipas, nuo viršaus prasidedantis hero, #20B200 ryškūs žali stačiakampiai CTA, #333E48 tekstas ir #2F3338 kupono / poraštės blokai. Papildomi reference tonai #253C29 ir #22612E; šviesus pagalbos fonas #F3F5F1. Pagrindinis CTA – PERŽIŪRĖKITE NAUJĄ PAPILDYMĄ. Antrinis – REIKIA PAGALBOS RENKANTIS? Kuponas LABASS pateiktas vartotojo; nenurodytas galiojimo terminas, teritorija, minimali suma ar tik pirmojo užsakymo sąlyga.

Šešios kategorijos iliustruotos ankstesniais packshotais be vandens ženklų. Tai kategorijų pavyzdžiai, ne tvirtinimas, kad šie SKU yra naujai įkelti ar vis dar turimi. Neįtrauktos kainos, reitingai, atsiliepimai ar skubos pažadai.

## Faktai ir šaltiniai

Brand DNA: ../brands/imunicija/BRAND-DNA.md. Logotipo, packshotų šaltiniai ir ankstesnio watermark retušo promptai: ../imunicija-welcome-email/BRAND_NOTES.md.
- https://imunicija.lt/naujos-prekes/ – pakartotinai gautas naujai įkeltų prekių puslapis. Jame produktų aprašymuose pateikiama būklė, garantijos terminas ir komplektacija. Šie laukai pagrindžia trumpus FAQ atsakymus; bendras universalus garantijos terminas nežadamas.
- https://imunicija.lt/garantija-ir-grazinimas/ – oficiali sąlygų nuoroda iš svetainės navigacijos; tiesioginis pakartotinis fetch šį kartą neveikė.
- https://imunicija.lt/kontaktai/ – ankstesnėje šios sesijos peržiūroje patikrinti kontaktai; pakartotinis fetch šį kartą neveikė. Kontaktinė informacija ir kategorijų nuorodos perimtos iš patvirtinto pirmo laiško.
- https://imunicija.lt/privatumo-politika/ – reference privatumo nuoroda.

## Omnisend perkėlimas

Tai lokalus peržiūros maketas. Prieš siuntimą įkelti naudojamus vaizdus į Omnisend / patvirtintą HTTPS talpyklą ir pakeisti src, background, CSS url bei VML src. Failai:
- assets/hero.jpg
- assets/brand/logo-white.png
- assets/products/samsung-s21.jpg
- assets/products/lenovo-x13.jpg
- assets/products/nintendo-switch.jpg
- assets/products/acer-iconia.jpg
- assets/products/huawei-fit-se.jpg
- assets/products/konka-tv.jpg

Patikrinti LABASS aktyvumą parduotuvėje bei tikras sąlygas. [[unsubscribe_link]] perkelta iš patvirtinto laiško, tikrame gavimo teste patikrinti jos pakeitimą. Hero yra AI fotosesijos interpretacija, ne konkretaus parduodamo vieneto būklės dokumentacija. Gamintojo logotipas nuotraukoje atskiras nuo tikro IMUNICIJA logotipo, uždėto HTML elementu.

## Ankstesnių laiškų kontrolė

imunicija-welcome-email HTML SHA256: 124fcf18b7a105b303a001b74bf558e8293a4251cb76d9e045da8ff9ffb641eb
imunicija-welcome-email-02 HTML SHA256: 42b2ace4d051e577e4b3f36509e1db5d6420c680a2ecdee78a9aceee76bafc8e

## Hero generacija

Naudotas builtin image_gen.imagegen įrankis, ne CLI. Pirma reference – tikras retušuotas Samsung Galaxy S21 packshotas, antra – patvirtinto pirmo laiško hero fotosesijos kryptis. Nauja telefono kompozicija atskira nuo ThinkPad ir Nintendo hero. Galutiniai failai assets/hero.jpg ir assets/hero-original.png.

Generacijos šaltinis: /Users/ugniusstakauskas/.codex/generated_images/01a08a73-d5a8-71a2-a0c1-7be485f9cbeb/exec-9779327e-b333-47c8-bdcb-663ae7d3fbe0.png

Promptas:

Use case: product-mockup. Create one new high-end editorial product photograph for Imunicija's third welcome email. Reference 1 is product identity: graphite Samsung Galaxy S21 5G, use ONLY the rear-facing phone from this packshot as the single hero object. Reference 2 is approved campaign art direction, not a composition to copy. A single graphite Samsung Galaxy S21 standing naturally and leaning slightly against a low warm limestone block on a refined dark walnut tabletop. Rear of phone faces camera at a subtle three-quarter angle so the true three vertically aligned camera lenses, integrated camera housing, flash, Samsung marking, thin edge and correct rounded proportions remain accurate. No second phone, no laptop, no console, no invented attachments. Premium product campaign photographed on location, soft raking window light from the left with restrained warm edge highlights, real glass reflections, fine natural texture on graphite back, limestone pores and walnut grain, convincing physical contact shadow. Deep charcoal forest-green plaster wall, understated luxury, calm cinematic light with no fog or theatrical glow, no plastic CGI gloss. Composition portrait 4:5: entire upper 43% is very dark empty charcoal-green wall reserved for a white HTML logo and two-line headline. Phone large enough to be clear, positioned centrally between 48% and 87% of image height, entirely inside the central 55% width so mobile cropping preserves it. Surface and subtle out-of-focus unbranded closed notebook only in lower 15%. No people, plants, extra devices, cables, ornamental objects, watermark, retailer name, promotional text or logo overlays. Keep authentic manufacturer marking small and natural. Expensive professional product photograph with honest detail and modest depth of field; entire phone in focus.

## Galutinė patikra

Desktop JPG/PNG 600 × 3659 px, renderinta 800 × 1000 viewport. Mobile JPG/PNG 390 × 3856 px. Patikrinti 800, 390 ir 320 px pločiai: horizontalios slinkties nėra, visi img įkeliami. Desktop kategorijų kortelės vienodo 312 px aukščio. Abi galutinės peržiūros vizualiai patikrintos. Korekcijų etape pašalinta besikartojanti kodo įvedimo instrukcija virš kupono. Patikrintos HTML/TXT nuorodos, img alt/matmenys, vietinių assetų egzistavimas, lentelių role=presentation, JS/formų nebuvimas, visi trys hero keliai (HTML, CSS, VML). Pirmo ir antro laiškų HTML hash nepakito. Tai naršyklės patikra, ne visų email klientų sertifikavimas; prieš siuntimą atlikti Omnisend gavimo testą.

Garantijos CTA korekcija: tekstinė nuoroda pakeista pilno FAQ pločio ryškiai žaliu #20B200 stačiakampiu „GARANTIJA IR GRĄŽINIMAS →“, tamsus tekstas, 49 px aukštis, 16 px vertikalus paddingas. URL išliko oficialus garantija-ir-grazinimas puslapis. Desktop/mobile patikrinta vizualiai, horizontalios slinkties nėra. Naujos peržiūros 600 × 3696 ir 390 × 3892 px.

## Trečio laiško savita kompozicija

Vartotojas paprašė paįvairinti trečią laišką, nes jis buvo per panašus į pirmą. Maketas perdarytas: baltas header su tikru tamsiu logotipu; dalintas hero su tekstu kairėje ir Samsung fotosesijos fragmentu dešinėje (CSS kadravimas, naujas vaizdas negeneruotas); asmeniškas komandos laiškas; kompaktiška šviesiai žalia LABASS juosta; trys atskiros numeruotos klausimų kortelės; tamsi naujo papildymo sekcija; sutrumpinta poraštė. Pakartotas 6 kategorijų tinklas pašalintas. Planas, garantijos ir pagalbos stačiakampiai žali CTA bei LABASS išliko. Pirmas ir antras patvirtinti laiškai neredaguoti. Papildomas fonas #EAF4E4 – maketo tonas.

Dabartinės siuntimo priklausomybės tik 3: assets/hero.jpg, assets/brand/logo-dark.png, assets/brand/logo-white.png. Likę packshotai archyve nebenaudojami.

Naujos kompozicijos QA: 600 × 2267 px desktop ir 390 × 2717 px mobile. Patikrinti 800/390/320 px ekranai be horizontalaus perpildymo; visos img priklausomybės įkeliamos. Abi galutinės peržiūros peržiūrėtos. Po pirmos peržiūros sumažintas desktop hero vertikalus paddingas, kad pradžia būtų kompaktiškesnė. HTML/TXT nuorodos suderintos; garantijos CTA išliko žalias stačiakampis. Desktop JPG tiksliai apkirptas pagal 600 px email konteinerį, pašalinant 24 px išorinį viršutinį tarpą. ZIP atnaujintas.

## Patikslinimas: hero ir produktų blokas išlaikomi

Vartotojo patikslinimu grąžintas pilno pločio ankstesnis Samsung hero su baltu logotipu bei 6 kategorijų / produktų nuotraukų blokas (3 × 2 desktop). Savitas stilius taikomas tik turiniui po hero: asmeniška įžanga, šviesus LABASS kuponas, numeruotos klausimų kortelės, atskiras naujo papildymo CTA. Ankstesnio dalinto hero ir balto header nebeliko. Siuntimui vėl naudojami 8 assetai: assets/hero.jpg, assets/brand/logo-white.png ir visi 6 assets/products/*.jpg pagrindiniai failai; logo-dark.png nebenaudojamas.


### Galutinė patikra po išdėstymo grąžinimo
Paliktas pilno pločio hero ir šešių kategorijų blokas su produktų nuotraukomis. Naujas stilius pritaikytas tik turiniui po hero: įžangai, LABASS kodo juostai, atsakymų kortelėms ir baigiamosioms sekcijoms. Patikrintas desktop ir mobile vaizdas, vietiniai paveikslėliai bei HTML ir TXT nuorodų atitiktis. Aktualūs JPG: desktop 600 × 3335 px, mobile 390 × 3815 px.


### Kategorijų bloko ir informacinės sekcijos atnaujinimas
Kategorijų blokas perdarytas į dviejų stulpelių, trijų eilių baltas korteles šviesiame fone. Kiekviena turi numerį, kategorijos pavadinimą, esamą produkto nuotrauką be watermarko ir ryškų stačiakampį CTA. Prieš footerį pridėtas informacinis pasirinkimo gidas: paskirtis, suderinamumas ir dydis, su kontaktiniu CTA. Tai bendri pasirinkimo patarimai, ne nauji pardavėjo pažadai. Hero ir LABASS pasiūlymas išsaugoti. Po vizualinės peržiūros supaprastinta kategorijų antraštė. Desktop (800 px viewport, apkirpta iki 600 × 4610 px) ir mobile (390 × 4571 px) patikrinti: 6 kortelės, paveikslėliai užkrauti, horizontalaus persipildymo nėra. HTML ir TXT nuorodos sutampa. Vietinius assetus prieš siuntimą reikia talpinti ESP / viešame HTTPS serveryje; ši versija yra lokali peržiūra.
