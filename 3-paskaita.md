# Laravel: 3 paskaita

## Video

[Paskaita nr. 3 - YouTube](https://www.youtube.com/watch?v=mLCDjAqWdCA)

## Apie ką kalbėjome ir ką nuveikėme

1. Kintamųjų apibrėžimas routes adresuose, jų panaudojimas.

2. Pastebime pasikartojančią logiką, t.y. keliuose route'uose gražinamas tik view, atitinkantis URL esantį puslapio pavadinimą, todėl pasidarom tik vieną tam skirtą route su kintamuoju ir jam sukuriame `PageController`.

3. Routes faile esantis eiliškumas ir prioritetai.

4. Užduotis: jeigu view neegzistuoja, rodome 404 klaidos puslapį. `View::exists()` ir `abort(404)` metodai.

5. Trumpai apie fasadus: `Route`, `View`.

6. Trumpai apie HTTP statusų kodus: 2xx, 3xx, 4xx, 5xx.

7. Pažintis su `.env` failu, kuriame yra apibrėžtos pagrindinės projekto konfigūracijos konstantos. `APP_DEBUG` konstantos.

8. `PageController` pakeitimas į single action controller `ShowPage`, turintį tik `__invoke` metodą.

9. Prisimenam MySQL, naudodamiesi phpMyAdmin kuriam `testimonials` lentelę.

10. `DB::select('select * from testimonials')` užklausa įrašams iš duomenų bazės paimti.

11. Debug'inimas pasinaudojant išvesties funkcijomis ir matant kintamųjų reikšmes: `dd()`, `var_dump()`.

12. Susipažįstame su Eloquent modeliais ir taip "užpildom" paskutinę dedamąją MVC schemoje.

12.1. Kuriame modelį pasinaudodami CLI: `php artisan make:model Testimonial`

12.2. Modelio metodų panaudojimas: `get()` ir `create()`

12.3. Modelio ypatybių pagal nutylėjimą pakeitimas kitomis reikšmėmis: `$fillable`, `$timestamps`.

## Užduotys

1. Papildyti 2 paskaitos užduotį sukuriant DB lentelę `skills`, modelį `Skill` bei išvedant duomenis pasinaudojus sukurtu modeliu bei metodu `Skill::get()`.

2. Sukurti puslapį, kuriame būtų išvedamas vienas atsiliepimas pagal jo ID panaudojant `Skill::find($id)` metodą. Mums reikės: naujo route su kintamuoju `id`, jau turimame `Skills` controlleryje naujo metodo `getSingle($id)` ir naujo view failo `single-skill.blade.php`.
