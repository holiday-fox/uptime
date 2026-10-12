# uptime

Checks the FIB campsite sites every 5 minutes from GitHub Actions. A site counts as down if it doesn't return 200 after 3 attempts 20 seconds apart. When a check fails, the run fails and GitHub emails whoever last edited the cron schedule.

Public on purpose: Actions minutes are free for public repos.

Edit the `SITES` list in `.github/workflows/uptime.yml` to add or remove sites. Run it by hand from the Actions tab (`workflow_dispatch`).
