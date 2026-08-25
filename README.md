# Applied Optics Group website

Published at <https://ee.iitm.ac.in/AppliedOptics>

Pushing to `main` rebuilds and republishes the site automatically, usually
within a minute. There is nothing to upload and no server to log into.

## Updating the site

```bash
git clone git@github.com:iitm-ee-infra/AppliedOptics.git
cd AppliedOptics
# edit the files you need
git add -A
git commit -m "describe what you changed"
git push
```

Wait about a minute, then reload the site. If it looks unchanged, hard-reload
the page (Ctrl-Shift-R, or Cmd-Shift-R on a Mac) to get past your browser cache.

## What to edit

| To change | Edit |
|---|---|
| Page text | `index.md`, `members.md`, `research.md`, `publications.md`, `facilities.md`, `gallery.md`, `involve.md` |
| Photos and images | `assets/img/` |
| Menu, header, footer | `_includes/` |

Never edit `_site/` -- it is generated, and your changes there will be
overwritten on the next push.

When linking to a page or image, use `relative_url` so the path works both
locally and on the live site:

```liquid
<img src="{{ '/assets/img/members/yourname.jpg' | relative_url }}">
```

A plain `/assets/img/...` will break on the live site.

## Checking whether it worked

Open the **Actions** tab in this repository. The most recent "Deploy to
Self-Hosted" run should show a green tick. A red cross means the site did not
update -- click the run to see why.

You can also redeploy without changing anything: Actions -> "Deploy to
Self-Hosted" -> "Run workflow".

## Known gaps

`index.md` references three images that were never added to the repository:
`assets/img/oct_focus.jpg`, `diffractive_focus.jpg` and `metaoptics_focus.jpg`.
Add files with those names to `assets/img/` and they will appear.

## Help

Ask Nitin Chandrachoodan if anything here is unclear or the site does not
update.
