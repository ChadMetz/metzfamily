# Metz Family

A simple family website for **metzfamily.online**, built as a static site for GitHub Pages.

## Files
- `index.html` — homepage
- `styles.css` — responsive design
- `CNAME` — custom domain configuration

## Add a family photo
Create an `images` folder, add a family image such as `family.jpg`, then replace the `.photo-placeholder` block in `index.html` with:

```html
<img src="images/family.jpg" alt="The Metz family">
```

Then add this to the CSS:

```css
.photo-card img { width:100%; display:block; aspect-ratio:4/3; object-fit:cover; }
```

## Publish with GitHub Pages
In the repository, open **Settings → Pages** and choose **Deploy from a branch**, then select `main` and `/ (root)`.

The included `CNAME` points the site to `metzfamily.online`. Configure the domain's web DNS records for GitHub Pages separately; keep all iCloud Mail MX/TXT/CNAME mail records in place.
