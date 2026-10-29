DEPLOYMENT — BRGY SISIG
==================================================

1. SUPABASE (once)
   SQL Editor → New query → paste all of setup.sql → Run.
   Expect: "Success. No rows returned."
   setup.sql does NOT go into the GitHub repo.

2. GITHUB REPO — upload everything except setup.sql
   and this readme, keeping the folders:

     index.html            (repo root — the POS)
     manifest.json         (repo root — makes it installable)
     icon-192.png          (repo root — home-screen icon)
     icon-512.png          (repo root — splash / store icon)
     version.json          (repo root — in-app updater)
     dashboard/index.html  (owner dashboard)
     queue/index.html      (customer queue screen)
     selftest/index.html   (deployment self-test — delete after sign-off)

   Then add sw.js WITHOUT uploading a file:
     Add file → Create new file → name it sw.js → paste the
     contents copied from the deployer → Commit changes.
     Without sw.js the POS cannot be reopened offline.

3. GITHUB PAGES
   Settings → Pages → Branch: main, folder: / (root) → Save.
   Allow 1–2 minutes for the first build.

URLS
  POS:       https://BRGYSISIG.github.io/BRGY-SISIG/
  Dashboard: https://BRGYSISIG.github.io/BRGY-SISIG/dashboard/
  Self-test: https://BRGYSISIG.github.io/BRGY-SISIG/selftest/
  Queue:     https://BRGYSISIG.github.io/BRGY-SISIG/queue/


  Business ID:    2baaaf5e-da82-50b3-8810-9fa9a897d24b

Template version 7.11.0
