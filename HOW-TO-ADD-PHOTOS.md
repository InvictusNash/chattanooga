# Adding staff photos — no HTML editing required

Your travel guide automatically looks for a photo for each person. You add or
change a photo simply by **uploading an image file with the right name** into
the `assets/people/` folder of your GitHub repository. You never touch the
HTML, and only people you've given access to your repo can do it.

---

## How the automatic photo system works

For every staff member, the guide tries to load a file named after them:

    assets/people/<firstname-lastname>.png

- All lowercase
- A single dash `-` between first and last name
- `.png` on the end

If that file exists, their photo shows (a round headshot when you tap their
name). If it doesn't exist yet, they just show a colored circle icon instead —
nothing breaks.

So "adding a photo" = "uploading a correctly-named PNG." That's it.

---

## The exact filenames for everyone who still needs a photo

Upload each of these into `assets/people/` :

    assets/people/jared-tuitel.png
    assets/people/audrey-richter.png
    assets/people/mary-berger.png
    assets/people/jesse-lackey.png
    assets/people/melina-degolyer.png
    assets/people/pressley-poteete.png
    assets/people/jaania-raj.png
    assets/people/clare-hankins.png

(Already done: robert-tate, damoniece-lowe, chantel-bell, julie-tucker.)

Tip: square-ish photos look best, since they're shown in a circle. Any
reasonable size works; a few hundred pixels wide is plenty.

---

## Step-by-step (all in your web browser)

1. Go to your repository on github.com.
2. Click into the `assets` folder, then the `people` folder.
3. Click **Add file → Upload files**.
4. Drag in your photo(s). **Rename each file first** so it matches the list
   above exactly (e.g. `jared-tuitel.png`).
5. Click **Commit changes**.
6. Wait about a minute for GitHub Pages to refresh, then reload your guide.
   The new photo appears.

To **replace** a photo later, upload a new file with the same name — it
overwrites the old one.

---

## Why only YOU can do this

GitHub Pages is a "static" site — there's no live server that accepts uploads
from visitors. The only way to change what's published is to commit a file to
the repository, and **only people you've added as collaborators on the repo can
commit.** Everyone else can view the guide but cannot change it. So this
ability is gated by your GitHub account by default — you don't have to set up
anything extra.

---

## What to upload to GitHub (one time)

Upload the entire contents of this `site` folder to your repository:

    index.html
    assets/  (logos + the people/ photo folder)

Then in **Settings → Pages**, set the source to your `main` branch / root, and
your guide is live. After that, the only thing you'll ever upload again is the
occasional new photo into `assets/people/`.
