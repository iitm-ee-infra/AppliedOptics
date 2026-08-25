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

Wait about a minute, then reload the live site. If it looks unchanged, hard-reload
the page (Ctrl-Shift-R, or Cmd-Shift-R on a Mac) to get past your browser cache.

## Previewing your changes first

You can see the site on your own machine before pushing anything. This needs
[Docker](https://docs.docker.com/get-docker/) installed -- nothing else, and in
particular no Ruby.

```bash
./build.sh --serve
```

Then open <http://localhost:4000/AppliedOptics/>. Leave it running while you
work: edit a file, save, and refresh the browser to see the change. Press
Ctrl-C to stop.

The first run takes a few minutes while it downloads the build tools. After
that it starts in seconds.

## What to edit

| To change | Edit |
|---|---|
| Page text | `index.md`, `members.md`, `research.md`, `publications.md`, `facilities.md`, `gallery.md`, `involve.md` |
| Photos and images | `assets/img/` |
| Menu, header, footer | `_includes/` |

Never edit `_site/`. It is the generated output, it is not part of the
repository, and it is rebuilt from scratch on every push.

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

Ask Nitin Chandrachoodan <nitin@ee.iitm.ac.in> if anything here is unclear or
the site does not update.
