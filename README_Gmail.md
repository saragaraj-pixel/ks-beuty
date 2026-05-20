Kako poslati rezervacije putem Gmaila

1) Preduvjeti
- PHP hosting (PHP 7.2+)
- Composer (preporučeno) / mogućnost instalacije vendor paketa
- Google račun s omogućenim 2FA i App Password-om

2) Instalacija PHPMailer (preporučeno)
U korijenu projekta (gdje je `send_reservation.php`) pokrenite:

```bash
composer require phpmailer/phpmailer
```

3) Postavljanje Gmail-a
- Omogućite dvostupanjsko potvrđivanje (2FA) na Google računu.
- Kreirajte App password (Vrsta aplikacije: Mail, Uređaj: Other). Kopirajte generirani password.

4) Konfiguracija
- Otvorite `send_reservation.php` i postavite `$smtpUser` na svoju Gmail adresu i `$smtpPass` na App password.
- Postavite `$to` na adresu na koju želite primati rezervacije.

5) Testiranje
- Uploadajte fajlove na hosting (ili instalirajte `vendor` direktorij ako koristite Composer lokalno i potom upload).
- Posjetite stranicu, pošaljite rezervaciju i provjerite dolazak maila.

Napomena: za veću pouzdanost koristite specijalizirane servise (SendGrid, Mailgun) ili OAuth2 autentikaciju za Gmail u produkciji.
