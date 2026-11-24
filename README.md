# FBI Huisrekening

Afgeschermde maandrekening van het FBI-huis, als GitHub Pages-site.

- `index.html`: overzicht voor de huisgenoten (alleen lezen). Iedereen kiest zijn naam en ziet zijn eigen kosten. Alleen maanden die op definitief staan worden getoond.
- `beheer.html`: hier stelt de beheerder de maand op en publiceert hem. Daarvoor zijn het huiswachtwoord en een eigen GitHub-token nodig (fine-grained, alleen deze repository, Contents: read and write). De token blijft in de browser van de beheerder en staat nooit in de repository.
- `data.json`: alle gegevens, versleuteld met het huiswachtwoord (PBKDF2-SHA256 + AES-GCM). Wordt bijgewerkt door op de beheerpagina op "Publiceer naar site" te klikken.

`index.html` en `beheer.html` worden gemaakt met `fbi_site.py`. Pas ze niet met de hand aan.
