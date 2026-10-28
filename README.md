# Jellyfin Netflix Theme

A Netflix-inspired CSS theme for Jellyfin Web, with dark surfaces, Netflix-red accents, responsive styling, image-safe poster effects, and progress indicators.

> **Scope:** This is a CSS theme, not a Jellyfin plugin. It only affects clients that render Jellyfin Web and load the custom stylesheet. Native client screens may ignore CSS entirely or only apply some rules. See the [official Jellyfin CSS customization documentation](https://jellyfin.org/docs/general/clients/css-customization/).

## Install the theme

### Option A — Server-wide (recommended)

1. Sign in to Jellyfin as an administrator.
2. Open **Dashboard → General → Branding** (the exact menu label can vary by Jellyfin version).
3. Find **Custom CSS code**.
4. Add this import line. If you already have custom CSS, preserve it and add the import rather than replacing unrelated rules.

```css
@import url("https://913aycltfm.github.io/jellyfin-netflix-theme/jellyfin-netflix-theme.css");
```

5. Save, then fully reload Jellyfin Web on each device. In a desktop browser, use a hard refresh if old styles remain cached.

### Option B — Per-user CSS

Some Jellyfin versions provide a custom CSS field under **User Settings → Display**. Add the same import there if you want the theme applied through that setting. Check whether **Disable server-provided custom CSS code** is enabled; if it is, the server-wide import may be ignored for that user. Avoid loading conflicting theme imports in both places.

## Troubleshooting

- **The website looks unchanged:** Open the stylesheet URL directly in the affected browser to confirm it loads. Then check that the import URL is spelled exactly as shown above and that the device has internet access to GitHub Pages.
- **Only some devices change:** CSS applies only to clients that use Jellyfin Web and honor custom CSS. It cannot guarantee a matching look in every native TV/mobile interface.
- **Some controls remain blue:** Jellyfin selectors and player controls vary by version and playback mode. Share a screenshot and the Jellyfin server/client version so the exact element can be targeted instead of adding broad CSS overrides.
- **Changes do not appear:** Save the settings, close/reopen the client, and clear its cache where possible. A browser hard refresh can help.
- **Images or layout look wrong:** Temporarily remove other custom CSS imports to check for conflicts. Keep a copy of your previous CSS before editing.

## Project files

- `jellyfin-netflix-theme.css` — theme stylesheet.
- `index.html` and `site.css` — project website.

## GitHub Pages

For **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, then branch `main` and folder `/(root)`. Save and wait for deployment.

- Project website: https://913aycltfm.github.io/jellyfin-netflix-theme/
- Stylesheet: https://913aycltfm.github.io/jellyfin-netflix-theme/jellyfin-netflix-theme.css

## Theme details

- Dark backgrounds and white/gray text.
- Netflix-red accents for common buttons, focus states, watched progress, and Live TV guide indicators.
- Preserves original artwork without filters or forced image ratios.
- Responsive refinements, keyboard focus visibility, and reduced-motion support.

## License

Choose and add a license before redistributing this theme. Respect the licenses and attribution requirements of any upstream code or assets incorporated.
