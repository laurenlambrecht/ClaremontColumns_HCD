# Claremont Columns

A social app concept for Claremont residents to upload photos of places they love in Claremont — or places that could use engineering improvements. Built from a human-centered design (HCD) project: paper prototypes first, then a second iteration based on feedback.

**Live site:** https://laurenlambrecht.github.io/ClaremontColumns_HCD/ 

## What it does

- **Map home** — an illustrated map of Claremont Village. Tap a pin to see every post at that address.
- **Feed** — all posts, newest first.
- **Add a post in four steps** — pick a location (type an address or tap the map), add photos (library or camera), write a caption or question, review and post.
- **Agree and comment** — every post can be agreed with or commented on; replies from city engineers are highlighted.
- **Notifications** — likes, comments, engineer messages, new photos at your location, and what's nearby.
- **Low-effort profile** — username, email/phone, age range, and how long you've lived in Claremont.
- **Featured Posts (iteration 2)** — a rotating spotlight of standout posts, imagined for the city's community-improvement page, so residents see their contributions are valued.
- **Process page** — the sketches and design notes behind each iteration.

## How it's built

Plain HTML, CSS and JavaScript — no frameworks and no build step. Sample posts load on first visit; anything you add (posts, photos, agrees, comments, profile) is saved in your own browser with `localStorage`. There's a "Reset demo data" link on the Profile page.

```
index.html        page shell, header and tab bar
styles.css        all styling
app.js            views, hash router, add flow, storage
data.js           sample locations, posts and notifications
assets/           favicon and process images
```

## Run it locally

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

## Publish with GitHub Pages

1. Push these files to the root of the `ClaremontColumns_HCD` repo.
2. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The site appears at `https://laurenlambrecht.github.io/ClaremontColumns_HCD/` within a minute or two.

## Notes

Sample posts, usernames and engineer replies are made up for the demo. The map is a stylized street grid, not a live map.
