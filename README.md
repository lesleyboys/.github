# Gedeelde GitHub-instellingen Lesley Boys

Herbruikbare workflows voor alle repos van `lesleyboys`, zodat dezelfde taak niet in elke repo apart staat.
Er staan hier geen geheimen: die blijven in de repo die de workflow aanroept (`secrets: inherit`).

| Workflow | Wat |
|---|---|
| [`supabase-backup.yml`](.github/workflows/supabase-backup.yml) | Wekelijkse, versleutelde back-up van een Supabase-project naar de gedeelde Drive en als artifact |
| [`supabase-wakker-houden.yml`](.github/workflows/supabase-wakker-houden.yml) | Houdt een gratis Supabase-project actief met `lb_ping` |

Gebruik altijd een vaste versie (`@v1`). Een wijziging die aanroepers kan breken krijgt een nieuwe tag (`v2`).
Hoe je ze aanroept staat bovenin elk bestand.

| Repo | Project | Back-up (schema's) | Wakker houden |
|---|---|---|---|
| club-lesleyboys | lb-kern | public auth storage clock video | ja |
| stem (ook socio) | lb-stem | public auth socio | ja |
| fideles | lb-fideles | public | ja |
| ai-brug | lb-ai | public | ja |
| esports | lb-esports | eigen `backup.yml` | – |
