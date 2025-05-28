# Jellyfin Theme Installation Guide

## Method 1: Using Custom CSS (Recommended)

1. **Login to your Jellyfin server** as an administrator

2. **Navigate to Dashboard** → **General**

3. **Find the "Custom CSS" section**

4. **Copy the entire contents** of `theme/theme.css` and paste it into the Custom CSS text area

5. **Click "Save"** at the bottom of the page

6. **Refresh your browser** (Ctrl+F5 or Cmd+Shift+R) to see the changes

## Method 2: Using Browser Extension

You can use browser extensions like Stylus or Stylish to inject the CSS:

1. Install [Stylus](https://add0n.com/stylus.html) for your browser
2. Click the Stylus icon and select "Manage"
3. Click "Write new style"
4. Copy the contents of `theme/theme.css`
5. Set the "Applies to" rules to match your Jellyfin server URL
6. Save and enable the style

## Method 3: Hosting Custom CSS File

If your Jellyfin server allows external CSS:

1. Host the `theme.css` file on a web server
2. In Jellyfin Dashboard → General → Custom CSS, add:
   ```css
   @import url('https://your-server.com/path/to/theme.css');
   ```

## Troubleshooting

- **Theme not loading?** Clear your browser cache and refresh
- **Partial styling?** Make sure you copied the entire CSS file
- **Conflicts?** Disable browser extensions that might interfere (like content blockers)
- **Mobile issues?** The theme is responsive but some mobile apps may not support custom CSS

## Browser Compatibility

This theme works best with:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+

## Notes

- The theme uses modern CSS features like `backdrop-filter` which may not work in older browsers
- Some Jellyfin apps (like mobile/TV apps) don't support custom CSS
- The theme is designed for the web interface only