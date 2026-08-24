# Akagera Safari Pokédex

A mobile-first, offline-capable Progressive Web App for recording wildlife encounters in Akagera National Park, Rwanda.

## What is included
- Data-driven wildlife catalogue (75 species)
- Featured wildlife home dashboard
- Search across common/scientific/alternative names and keywords
- Rarity, category and spotted-status filters
- Optional sighting-quality bonuses (+0/+1/+2/+3)
- Optional species-aware group-size bonuses (+0/+1/+2/+3)
- Species-specific behaviour prompts
- Big Five tracker
- Auto-saved local safari sessions and history
- Reopen/undo completed safaris
- Safari summary with best sighting, rarest animal and largest group
- PWA manifest, service worker and installable app shell
- Original app icon
- Image-credit metadata in the data model and credits screen

## Run locally
No build step is required. Serve the folder with any static HTTP server (service workers do not run from `file://`). For example:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## GitHub Pages
1. Create a new GitHub repository.
2. Upload/push the contents of this folder to the `main` branch.
3. In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/root` (or `/docs` if you move the files there).
4. Open the generated GitHub Pages URL on iPhone/Android.
5. Use the browser's **Add to Home Screen / Install app** action.

A GitHub Actions workflow is included at `.github/workflows/pages.yml`. After enabling Pages for the repository, pushes to `main` can deploy automatically through the Pages environment.

## Updating
Push changed files to the same branch. The service worker uses a versioned cache name; increment the `CACHE` value in `sw.js` for a forced cache refresh after major asset changes.

## Images & licensing
Image records include source and licence fields. The initial app uses Wikimedia Commons `Special:FilePath` URLs for photographs where practical, plus several supplied/selected Wikimedia Commons images. Before public commercial deployment, verify each image's current Commons licence and attribution requirements and replace any unresolved image records with a specific licensed file.

The app does not use Pokémon, Nintendo or other Pokémon artwork/trademarks.

## Accuracy note
Wildlife occurrence and rarity are calibrated as safari-game design values, not conservation-status ratings. The species set is based on Akagera's official wildlife information and reputable wildlife references. The official park site currently describes thriving populations of lion, leopard, elephant, rhino and buffalo, common herds of buffalo/impala/zebra/topi, smaller antelope, hippo/crocodile waterways, nocturnal wildlife and more than 480 bird species.

Official source: https://visitakagera.org/
