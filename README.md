# logintest

Proof of concept: "Logga in med Microsoft" som skriver ut vilken e-postadress användaren loggade in med. En enda HTML-fil (`index.html`) med MSAL.js, ingen backend.

## Kom igång

1. Registrera en app i Microsoft Entra (portal.azure.com → Microsoft Entra ID → App registrations → New registration).
2. Lägg till en redirect-URI av typen **Single-page application (SPA)**, t.ex. `http://localhost:8000/`.
3. Klistra in appens **Application (client) ID** i `index.html` i stället för `DITT-CLIENT-ID`.
4. Starta en lokal server och öppna http://localhost:8000/:

   ```bash
   python3 -m http.server 8000
   ```

Ska sidan ligga på GitHub Pages lägger du till den adressen (t.ex. `https://fjellandermedia.github.io/logintest/`) som ytterligare redirect-URI.
