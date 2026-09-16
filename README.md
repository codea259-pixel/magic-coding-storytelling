[README.md](https://github.com/user-attachments/files/32271623/README.md)[Uploading # Code Quest

Two story-driven browser games that teach real JavaScript syntax:

- **Pixel Finds Home** — Junior Cadet track (ages 6+): `console.log`, variables, `if`/`else`, loops.
- **Argus-9: The Last Terminal** — Full Crew track (all ages): variables, conditionals, loops, functions, arrays.

Everything is a single self-contained page (`index.html`) — no build step, no dependencies to install, no backend. Learners write real, runnable JavaScript in-browser and get immediate story-driven feedback.

## Play it locally

Just open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge). Double-click the file, or run:

```bash
open index.html      # macOS
start index.html     # Windows
xdg-open index.html  # Linux
```

## Publish it with GitHub Pages

1. Create a new repository on GitHub and add these files (`index.html`, `LESSON-PLAN.md`, `README.md`) to it.
2. Push to the `main` branch.
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
5. Save. GitHub will give you a URL like `https://<your-username>.github.io/<repo-name>/` within a minute or two.

Because the file is named `index.html`, it will load automatically at that root URL.

## Files in this repo

| File | What it is |
|---|---|
| `index.html` | The game itself — both tracks, mission-select screen included. |
| `LESSON-PLAN.md` | A facilitator's guide: session plans, per-level discussion questions, a printable worksheet, and an answer key. |
| `README.md` | This file. |

## How it works

- All code runs client-side in a sandboxed `Function` — nothing is sent to a server.
- Each level defines a `test(code)` function that runs the learner's code against small mock objects (e.g., `helpers.getOxygen()`) and checks the *behavior*, not exact wording, so there's more than one valid solution per level.
- Progress and in-progress drafts are saved per-browser via `localStorage`, separately for each track.

## Customizing

Both tracks' levels, story text, starter code, hints, and pass/fail checks live near the top of the `<script>` block in `index.html`, in the `CREW_LEVELS` and `JUNIOR_LEVELS` arrays. Each level is a self-contained object, so adding a new level means adding a new object to the array and a corresponding node in the progress track (handled automatically from the array length).

## License

Use, remix, and adapt freely for teaching.
README.md…]()
