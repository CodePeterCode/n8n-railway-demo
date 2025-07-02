# n8n Railway Demo

## Deploy to Railway

1. Fork this repo.
2. Skapa projekt i Railway via **Deploy from GitHub** → välj din fork.
3. Koppla din Neon-databas under "Plugins → PostgreSQL" i Railway.
4. Gå till Settings → Variables och fyll i:

N8N_EXTERNAL_URL=https://<din-railway-subdomain>
NODE_ENV=production
N8N_RUNNERS_ENABLED=true
GENERIC_TIMEZONE=Europe/Stockholm
TZ=Europe/Stockholm
N8N_ENCRYPTION_KEY=<lång-hemlig-nyckel>

bash
Kopiera
Redigera

5. Klicka "Rollback & Redeploy".

## Använda

◾ Öppna n8n-webb i Railway.  
◾ Skapa Gmail OAuth-cred — använd redirect URL:
https://<din-railway-subdomain>/rest/oauth2-credential/callback