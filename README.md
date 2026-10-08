# Swimify – GitHub Pages -versio

Tämä on suoraan selaimessa ajettava Swimify-TV-grafiikka. Se ei tarvitse PowerShell-palvelinta eikä Cloudflarea.

## GitHub Pages

1. Luo GitHub-repository.
2. Lataa `index.html` repositoryn juureen.
3. Avaa **Settings → Pages**.
4. Valitse **Deploy from a branch**, branch `main` ja kansio `/ (root)`.
5. Tallenna.

GitHub Pages käyttää repositoryn juuressa olevaa `index.html`-tiedostoa sivun aloitustiedostona.

## Tärkeä huomio

Swimify GraphQL -avain on tässä client-side-versiossa selaimen JavaScriptissä. Se tarkoittaa, että julkisessa GitHub-repositoryssä avain on käyttäjien nähtävissä. Lisäksi Swimifyn GraphQL-palvelimen pitää sallia selainpyynnöt GitHub Pages -originista CORSilla.

Jos selain näyttää CORS-virheen, tämä suora GitHub Pages -ratkaisu ei voi kiertää sitä ilman välipalvelinta/proxyä.
