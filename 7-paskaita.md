# Laravel: 7 paskaita

## Video

[Paskaita nr. 7 - YouTube](https://www.youtube.com/watch?v=Zymgt8pMCR8)

Ok, šįkart nebežinau, kas nutiko su video, kad neįrašė net pilnos minutės. Atrodo, paleidau ir daugiau nieko nebeprimaigiau.

## Apie ką kalbėjome ir ką nuveikėme

1. Įkelto failo validacija, nauja taisyklė `image`.

2. Session flash pranešimai po sėkmingai įvykdyto veiksmo: sukūrimo, atnaujinimo, ištrynimo.

3. Eloquent `orderBy` metodas.

4. Eloquent relationships: `hasOne` ir `hasMany`. 

4.1. Mūsų aplikacijos planavimas ir paruošimas: kiekvienas `User` gali turėti daug `Friend` įrašų, `hasMany` sąryšio taikymas.

4.2. Naujos DB migracijos `friends` lentelės papildymui: `user_id` kaip `foreign key` ir nuoroda į `users` lentelę.

4.3. Naujas DB lentelės stulpelio tipas: `enum`; papildomi metodai: `nullable()`, `default()`, `after()`.

4.4. Migracijos metodo `down()` aprašymas, metodai `dropForeign()` ir `dropColumn()`.

4.5. `FriendsTableSeeder` papildymas.

5. `Auth` serviso metodai: `user()`, `check()`, `id()`.

6. Duomenų pasiėmimas bei pridėjimas naudojant Eloquent relationships ir apribojant prieigą tik prie tų `Friend` įrašų, kurie priklauso prisijungusiam `User`.

7. `where()` metodas norint filtruoti duomenis.

8. `Request` serviso `input()` metodas GET parametrų, esantiems nuorodoje, gavimui ir panaudojimui.

## Užduotys

1. Galimybė filtruoti sąrašą `skills` puslapyje nurodant norimą reitingą skaitine reikšme GET parametruose ir taikant `where` metodą.

2. Rikiuoti `skills` įrašus mažėjimo tvarką pagal reitingą.

3. `User` modelis gali turėti daug `Skill` įrašų: taikyti `hasMany()` sąryšį, pasirašyti naują migraciją `skills` lentelės atnaujinimui.
