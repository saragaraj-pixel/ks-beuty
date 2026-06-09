Formspree - brzo slanje formi bez servera

1) Napravite Formspree formu
- Otvorite https://formspree.io i prijavite se (ili registrirajte).
- Kreirajte novi form, kopirajte vaš `form ID` (format: `f/xxxxx`).

2) Postavite `index.html`
- U `index.html` ažurirajte form action na:

  https://formspree.io/f/yourFormID

  (zamijenite `yourFormID` stvarnim ID-jem iz Formspree-a)

- Form sadrži već `name` atribute i skriveni redirect na `thank-you.html`.

3) Testiranje
- Otvorite stranicu (lokalno ili na hostingu) i pošaljite rezervaciju.
- Formspree će poslati potvrdu i, ovisno o postavkama računa, proslijediti email na adresu povezanu s Formspree.

4) Opcije
- Ako želite da primate poruke direktno na svoj e-mail bez potvrde korisnika, provjerite Formspree plan i postavke (besplatni plan može zahtijevati potvrdu).
- Možete uključiti i recaptcha ili dodatna polja koju Formspree podržava.

5) Ako želite, ja mogu:
- Zamijeniti `yourFormID` u `index.html` ako mi date taj ID.
- Ukloniti `send_reservation.php` (nije više potreban) ili ostaviti kao backup.

*** KRAJ ***
