# Wix Forms × CMS — "Connect a form" prototype

An interactive, click-through prototype exploring how a form added in the Wix Editor
lets the user choose where submissions go — **Wix Forms** or a **CMS Collection** — and,
for the CMS path, which collection (e.g. **Recipes**) the form connects to.

It's a single self-contained `index.html` — no build step, no dependencies to install
(Tabler icons load from a CDN).

## Run it

- **Locally:** just open `index.html` in any browser (double-click it).
- **Hosted:** served via GitHub Pages — see the repo's Pages URL.

## The flow

1. Left rail **+** → **Forms** → **Create new Form** (or **Add existing Form**).
2. Modal: **Where should submissions go?** — choose **Wix Forms** or **CMS Collection**.
3. **CMS path:** pick a collection (**Recipes**) → the on-canvas form rebuilds to match the
   collection's fields (Recipe Name, Prep/Cooking Time, Ingredients, Instructions, Photos).
4. The placed form shows a pink **Connected to Recipes** boundary. The Add panel auto-closes;
   the **+** button reopens it.
5. Click the **form**, any **field**, or the **Submit** button to select it (pink frame) and
   open the right-side **Properties** panel:
   - Form → the connected collection (**Recipes Item**).
   - Field → its **Value** binding (e.g. `recipes.recipeName`).
   - Submit → its **Click action** (Submit to Recipes).

## Notes

- Pure HTML/CSS/JS, no framework.
- Built as a design prototype — interactions are mocked, nothing is persisted.
