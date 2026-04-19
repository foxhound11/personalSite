# bharat.md Personal Site

A fast, simple, and distastefully-free static personal site.

## Architecture

This site is built using **plain HTML and CSS**. It has absolutely zero dependencies, no build steps, and no framework overhead. It leverages modern semantic HTML and CSS variables for a clean, typography-focused, "markdown-esque" design.

- `index.html` - Home Page
- `about.html` - About Page
- `work.html` - Work Page
- `notes.html` - Notes Page
- `styles.css` - Global Styles

## Deployment

Deploying this site is instantaneous on any static host.

### Vercel
1. Go to your Vercel Dashboard and click **Add New... > Project**
2. Import this repository (`foxhound11/personalSite`).
3. Vercel will automatically detect it as a static site. No build command or output directory is needed.
4. Click **Deploy**.

### Netlify
1. Go to your Netlify Dashboard and click **Add new site > Import an existing project**.
2. Select GitHub and authorize the repository (`foxhound11/personalSite`).
3. Leave the build command empty and the publish directory as the root.
4. Click **Deploy site**.

## Adding New Notes / Posts

Because this is a pure static site, adding a new note is simple:

1. Create a new HTML file (e.g., `my-new-post.html`), copying the basic structure from `notes.html`.
2. Write your content using standard HTML (`<h1>`, `<h2>`, `<p>`).
3. Add a link to your new file inside the `notes.html` index list:
```html
<div class="note-card">
    <h3><a href="my-new-post.html">My New Post Title</a></h3>
    <p>A short preview of the post goes here.</p>
</div>
```

If you prefer pure Markdown in the future, you can simply rename this to an Astro project or drop in a small library like `marked.js` inside `notes.html`. For now, it stays intentionally simple and completely static.
