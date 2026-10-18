# Jellyfin Netflix Theme

A Netflix-inspired, CSS-only theme for Jellyfin with a dark interface, red accents, subtle poster hover effects, image-safe styling, responsive adjustments, and red Live TV program-guide progress indicators.

## Files

- `jellyfin-netflix-theme.css` — stylesheet to import into Jellyfin.
- `index.html` and `site.css` — GitHub Pages project website.

## Install the theme

In Jellyfin, open **Dashboard → General → Custom CSS** and add:

```css
@import url("https://913aycltfm.github.io/jellyfin-netflix-theme/jellyfin-netflix-theme.css");
```

Save and reload the Jellyfin web interface.

## Publish the project website with GitHub Pages

1. Open this repository's **Settings**.
2. Select **Pages** in the left sidebar.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**, then click **Save**.
5. Wait a few minutes for the website to publish.

The expected website address is https://913aycltfm.github.io/jellyfin-netflix-theme/ . The expected stylesheet address is https://913aycltfm.github.io/jellyfin-netflix-theme/jellyfin-netflix-theme.css .

## Theme highlights

- Dark, cinematic surfaces with Netflix-red (`#e50914`) accents.
- Hover effects for poster cards on devices with a mouse or trackpad.
- Preserves native image presentation; does not force image ratios or apply filters.
- Red progress styling for playback and common Live TV guide progress/current-time selectors.
- Mobile and tablet refinements, visible keyboard focus, and reduced-motion support.

## Notes

This project is CSS-only and does not add JavaScript to Jellyfin itself. Jellyfin web selectors can change between releases, and some clients do not use the server's web CSS. Verify behavior on your Jellyfin version and devices.

## License

Choose and add a license before redistributing this theme. Respect the licenses and attribution requirements of any upstream code or assets you incorporate.
