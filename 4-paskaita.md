# Laravel: 4 paskaita

## Video

[Paskaita nr. 4 - YouTube](https://www.youtube.com/watch?v=rTgMSUL_91w)

## Apie ką kalbėjome ir ką nuveikėme

1. 2 ir 3 paskaitos savarankiškų užduočių aptarimas.

2. `TestimonialsController` papildymas metodu `getSingle()`, jam skirtas view `single-testimonial.blade.php` bei route `testimonials/{id}` aprašymas.

3. Route parametrų formato apibrėžimas naudojant `where()` metodą ir [regular expressions](http://regexr.com).

3.1. Paprasčiausios regex taisyklės: `[0-9]+`(skaičius), `[a-z]+` (žodis mažosiomis raidėmis - lowercase), `[A-Z]+` (žodis didžiosiomis raides - uppercase), `[A-Za-z]+` (žodis naudojant tiek mažąsias, tiek didžiąsias raides).

4. CRUD intro: create, read, update, delete. Pagrindinės operacijos dirbant su duomenimis. 

5. Pradedam darbą nuo pradžių su nauju įrašo tipu: draugai/friends bei aptarimas, kokia bus eiga.

5. DB migrations.

5.1. DB lentelių struktūros aprašymas naudojantis migracijomis ir komanda `make:migration`. 

5.2. CLI komandos norint dirbti su migracijomis: `migrate`, `migrate:reset`, `migrate:status`, `migrate:rollback`.

6. DB seeders: automatinis lentelių užpildymas su jau apibrėžtais ar atsitiktinai sugeneruotais duomenimis.

6.1. Seeders klasės sukūrimo komanda: `make:seeder`.

6.2. Duomenų bazės užpildymas pasinaudojant seederių komandomis: `db:seed`, `db:seed --class=FriendsTableSeeder`.

7. Resource controller'io kūrimas: `make:controller FriendsController --resource` arba papildomai galima iškart nurodyti ir modelį, kuris bus sugeneruotas `make:controller FriendsController --resource --model=Friend`.

8. Resource controllerio metodų apžvalga.

9. Route naujas metodas `Route::resource`, kuris yra tiesiogiai susijęs su resource tipo controlleriu ir automatiškai sukuria kelis atskirus route'us.

10. `route()` funkcija, generuojanti adresą bei named routes panaudojant metodą `name()`.

11. Formos submit'as, `$request` objektas, `$request->all()` metodas POST duomenims pasiimti.

12. Request'o duomenų validacija pasinaudojant controllerio metodu `validate()` bei apsibrėžiant taisykles.

13. Validacijos klaidų išvedimas pasinaudojant `$errors->all()`.

14. CSRF atakos ir jų prevencija panaudojant token'o field'ą formoje.

## Užduotys

1. Pabaigti `FriendsController` metodą `index` ir panaudoti `Friend` modelį įrašams iš DB gauti, sukurti šabloną `friends/list.blade.php` bei išsivesti duomenis.

2. Pabaigti `FriendsController` metodą `show` ir atvaizduoti vieną įrašą šablone `friends/show.blade.php`.
