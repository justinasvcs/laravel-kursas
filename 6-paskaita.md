# Laravel: 6 paskaita

## Video

[Paskaita nr. 6 - YouTube](https://www.youtube.com/watch?v=SYMJO3kUbSk)

## Apie ką kalbėjome ir ką nuveikėme

1. Users ir passwords reset migrations pakeitimai grąžinant indeksų metodus ir konfigūracijos pakeitimas: AppServiceProvider pridedam `Schema::defaultStringLength(191)`, [plačiau apie problemą](https://laravel-news.com/laravel-5-4-key-too-long-error)

2. Teorija: autentifikacija ir autorizacija

3. Auth middleware taikymas resource controllerio `__construct` metode (visas controlleris reikalauja, kad būtų prisijungęs vartotojas)

4. Vartotojų seeder'is, `Hash` servisas, slaptažodžių hashinimas

5. Teorija: hashinimas ir encryptinimas

6. Request objekto kūrimas, į kurį perkeliamos draugo formos validacijos taisyklės. Requesto klasės type-hint'as metodo argumentuose

7. Įrašų paruošimas puslapiavimui su `paginate` ir `simplePaginate` metodais bei nuorodų išvedimas šablone

8. `php artisan route:list` komanda

9. Collections, `collect` helperis, palyginimas su masyvais ir jiems skirtomis funkcijomis, kurios yra built-in pačiam PHP

10. Friend formos iškėlimas į atskirą failą ją padarant universalią create/edit formoms

10.1. `@include` direktyva, `old()` funkcija

11. Failo įkėlimas, saugojimas bei atvaizdavimas. `Storage` servisas.

## Užduotys

Ruošiama.
