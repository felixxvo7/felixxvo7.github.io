# Felix Vo, Portfolio Site

A single page portfolio built as one self contained `index.html`. No build step, no dependencies. Just the file and your browser.

## Publish it to felixxvo7.github.io

Since your username is `felixxvo7`, this becomes your main GitHub Pages site, live at `https://felixxvo7.github.io`. The repo name has to match your username exactly.

### Option A, through the GitHub website

1. Create a new repository named exactly `felixxvo7.github.io` and make it Public.
2. On the new repo page, click "uploading an existing file".
3. Drag in `index.html` and commit.
4. Wait about a minute, then open `https://felixxvo7.github.io`.

That is it. For a repo named `username.github.io`, Pages turns on automatically from the `main` branch.

### Option B, through the terminal

```bash
# put index.html in an empty folder, then from inside that folder:
git init
git add index.html
git commit -m "Add portfolio site"
git branch -M main
git remote add origin https://github.com/felixxvo7/felixxvo7.github.io.git
git push -u origin main
```

If Pages does not switch on by itself, go to the repo, Settings, Pages, and set the source to the `main` branch, root folder.

## Editing later

Everything lives in `index.html`. The parts you are most likely to touch:

- Text content sits in plain HTML in the `<body>`. Search for the words you want to change.
- Colors are defined once at the top in the `:root` block (the `--forest`, `--beige`, `--gold` variables). Change them there and the whole site follows.
- The hero animation is the `node graph` script near the bottom. Adjust `COUNT` for more or fewer dots.

## A note on a custom domain

If you ever buy a domain like `felixvo.com`, add it under Settings, Pages, Custom domain, and the site moves over with no other changes.
