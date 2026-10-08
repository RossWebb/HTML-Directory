# Customisable 'Essentials' Dashboard

A simple, customizable, offline HTML dashboard for quick access to important resources.

Originally created for VAG (with Google Drive folders and tools), but designed so anyone can turn it into their own personal or team dashboard.

---

## Features

- Clickable tiles that open links in a new tab
- Group resources under custom labels
- Drag-and-drop to reorder tiles or move them between groups
- Edit tile title, URL, and image
- Delete tiles with a red ×
- Auto-remove empty groups
- Editable main dashboard title
- PIN-protected editing (prevents accidental changes)
- **Create Blank Slate** – wipe everything and start fresh
- Export / Import configuration as JSON
- Line breaks in tile titles (Title + Subtitle style)
- Fully offline – works from a local file
- Responsive design (works on phone, tablet, and desktop)

---

## How to Use

1. Download the `VAG-Essentials.html` file
2. Double-click it to open in your browser
3. Click any tile to open the linked resource

### To customize

1. Click **Enter Edit Mode**
2. Enter the PIN (default is `talua26`)
3. You can now:
   - Click **Edit** on a tile to change its title, URL or image
   - Click the red **×** to delete a tile
   - Drag tiles to reorder or move them between groups
   - Click **Edit Label** next to a group name to rename it
   - Click **Add Tile** to create a new resource
   - Click the **✏️ Edit Title** button to change the main heading
   - Click **Create Blank Slate** to clear everything and start from scratch

Editing stays unlocked until you close or reload the page.

---

## Line Breaks in Titles (Title / Subtitle)

When editing or adding a tile title, use a **`+`** character to create a line break.

**Example:**

```
Public Folder+Shared Drive
```

Will display as:

**Public Folder**  
Shared Drive

---

## Sharing with Others

The best way to share is simply to **send the HTML file**.

- The recipient opens the file in their browser
- They can then customize it further
- Their changes are saved in their own browser

> Note: The old “Create Share Link” feature was removed because local `file://` links do not work reliably across different computers.

---

## Export / Import Configuration

If you want to back up or transfer your exact setup:

1. Enter Edit Mode
2. Click **Export Config** → copies JSON to clipboard
3. On another copy of the file, click **Import Config** and paste the JSON

---

## Changing the PIN

Open the HTML file in a text editor and search for:

```js
const editPin = "talua26";
```

Change `"talua26"` to whatever PIN you prefer.

---

## Reset vs Blank Slate

| Button                 | What it does                                      |
|------------------------|---------------------------------------------------|
| **Reset**              | Restores the original VAG default tiles & groups |
| **Create Blank Slate** | Completely clears the dashboard so you can start fresh |

---

## Technical Notes

- Pure HTML + CSS + JavaScript (no frameworks, no internet required after download)
- Configuration is stored in the browser’s `localStorage`
- Maximum of 25 tiles
- Works in all modern browsers

---

## Credits

Created by Ross Webb  
Feedback and error reports welcome: **ross_webb@sil.org**

---

## License

Feel free to use, modify, and share this dashboard.
