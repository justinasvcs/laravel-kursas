# Laravel: 2 paskaita

## Video

[Paskaita nr. 2 - YouTube](https://www.youtube.com/watch?v=mVG3Y7u0byk)

## Apie ką kalbėjome ir ką nuveikėme

1. MVC ir routes: pakartojame ir užtvirtiname, kuo pabaigėme pirmą paskaitą.

2. Kuriame naują puslapį, kuriame bus išvedami atsiliepimai.

3. Kintamųjų perdavimas į `view()` funkciją bei jų išvedimas naudojamame šablone.

4. Susipažinimas su Laravel klaidos puslapiu ir joje esančiu klaidos aprašymu.

5. Darbas su PHP masyvais, pakartojame, kas tai yra, kaip apibrėžiama ir kaip naudojama.

5.1. Apibrėžiame vieną atsiliepimą kaip masyvą: indeksuotą ir asociatyvų.

5.2. Apibrėžiame daugiau atsiliepimų juos sudėdami į vieną bendrą masyvą kaip atskirus elementus.

6. Trumpas pakartojimas apie PHP ciklus bei naujas ciklas `foreach`.

6.1. Atsiliepimų išvedimas šablone panaudojant `@foreach` metodą. `@if` panaudojimas Blade šablone.

7. Pirma pažintis su controllers.

7.1. Controller klasės `Testimonials` susikūrimas rankiniu būdu arba panaudojant `php artisan make:controller` komandą.

7.2. Logikos persikėlimas į controller'io klasės metodą taip atsikratant anonimės funkcijos šalia route'o.

8. Papildomos `php artisan` komandos: `inspire`, `down`, `up`, `route:list`.

9. Susitvarkome savo puslapį: pasikeičiam nuorodas į vidines, kurias apsirašėm route'uose, atliekam minimalius stiliaus pakeitimus.

10. Platesnė pažintis su Blade šablonų varikliuku ir paveldimumu.

10.1. Pagrindinio šablono susikūrimas ir vidiniai puslapiai panaudojant direktyvas: `@extends`, `@yield`, `@section`.

11. CSS prisiminimas ir papildomi stiliaus pakeitimai.

12. Formos persikėlimas į atsiliepimų puslapį.

## Užduotys

1. Kuriame naują puslapį `Skills`. Jame norime išsivesti savo įgūdžius, galutinis rezultatas šabloniškai gali atrodyti taip:

```
HTML ***** (10 metų)
CSS ***** (10 metų)
JavaScript ***** (5 metai)
PHP ***** (10 metų)
Laravel * (dar tik mokausi...)
```

Kiekvieno įgūdžio įrašo struktūra:

- Kalba / įrankis / įgūdis

- Įvertinimas skaitine reikšme nuo 1 iki 5

- Trumpas komentaras, tekstas

Reikalavimai:

- Panaudoti HTML sąrašą

- Panaudoti CSS žinias ir sava nuožiūra suteikti stilių sukurtam sąrašui (spalvos, dydžiai, pozicijos, etc)

- Panaudoti PHP masyvus

- Panaudoti Blade ciklus

- Įgūdžio įvertinimas turi būti pakeičiamas atitinkamu skaičiumu žvaigždučių

Bonus:

- Vietoj žvaigždučių panaudoti ikonėles iš [Bootstrap](https://getbootstrap.com/docs/3.3/components/) (kuris jau yra įdiegtas) arba prisidėti [FontAwesome](http://fontawesome.io/) (sudėtingiau).

- Vietoj pagrindinio masyvo, kuriame laikomi visi įrašai, panaudoti [Collections](https://laravel.com/docs/5.4/collections).

- Labai vertinu kūrybą ir improvizaciją. Tai bet koks nukrypimas ar papildymas pagal save - labai laukiamas!
