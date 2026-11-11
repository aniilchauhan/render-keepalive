# render-keepalive

A tiny GitHub Actions cron that pings a Render web service every 10 minutes so the free tier never spins down.

Change `HEALTH_URL` in `.github/workflows/keepalive.yml` to point at another service. The workflow fails if the endpoint does not return HTTP 200, so a broken deploy shows up in the Actions tab.
