---
title: Bookmark Management
order: 1
---

# Bookmark Management

NavHub's bookmark management system is designed to handle thousands of bookmarks while keeping them organized and easily accessible.

## Adding Bookmarks

### From the Web App

1. Click the **+ Add** button in the top navigation
2. Paste the URL or type it manually
3. NavHub auto-fetches title, description, and thumbnail
4. Add tags and select a folder
5. Click **Save**

### From Browser Extension

1. Navigate to any webpage you want to save
2. Click the NavHub extension icon
3. Edit details if needed
4. Click **Save**

### Quick Add (Keyboard Shortcut)

Press `Ctrl+Shift+S` (Windows) or `Cmd+Shift+S` (Mac) to instantly save the current page.

## Organizing Bookmarks

### Tags

Tags provide flexible, non-hierarchical organization:

- Add multiple tags to any bookmark
- Filter by one or more tags
- Tag suggestions based on content
- Bulk tag editing

**Best practices:**
- Use consistent naming (lowercase, no spaces)
- Create a core set of tags you use regularly
- Let AI suggest tags, then refine

### Folders

Folders provide traditional hierarchical structure:

- Unlimited nesting levels
- Drag-and-drop to move bookmarks
- Folder icons and colors
- Share entire folders (Pro)

### Combining Tags and Folders

Use both for maximum flexibility:
- **Folders** for primary categorization (Work, Personal, Projects)
- **Tags** for cross-cutting concerns (to-read, reference, important)

## Searching Bookmarks

### Quick Search

Press `/` or click the search bar to search:

- **Title** — Matches bookmark titles
- **URL** — Matches domain or path
- **Tags** — Type `#tagname` to filter by tag
- **Folder** — Type `folder:name` to filter by folder

### Full-Text Search

NavHub indexes the content of saved pages:

- Search for keywords mentioned in the page
- Find bookmarks even if the title doesn't match
- Automatic re-indexing when content changes

### AI Search (Pro)

Use natural language to find bookmarks:

- "Articles about React performance"
- "That cooking recipe I saved last month"
- "YouTube videos about machine learning"

## Bookmark Details

Each bookmark stores:

| Field | Description |
|-------|-------------|
| Title | Page title (editable) |
| URL | The webpage address |
| Description | Summary or your notes |
| Thumbnail | Visual preview image |
| Tags | Multiple tags for organization |
| Folder | Single parent folder |
| Created | When you saved it |
| Last visited | When you last clicked it |

## Import & Export

### Importing Bookmarks

NavHub supports importing from:

- **Chrome** — Export HTML from Chrome, import to NavHub
- **Firefox** — Export JSON or HTML, import to NavHub
- **Safari** — Export HTML, import to NavHub
- **Raindrop.io** — Export and import with tags preserved
- **Pocket** — Export HTML, import with tags

[See Import Guide →](../guides/import-bookmarks.md)

### Exporting Bookmarks

Export your bookmarks anytime:

- **HTML** — Standard format, works everywhere
- **JSON** — Full data including metadata
- **CSV** — For spreadsheet analysis

## Tips & Tricks

1. **Use keyboard shortcuts** — `/` to search, `n` to add new
2. **Star important bookmarks** — Quick access from anywhere
3. **Regular cleanup** — Delete broken links, merge duplicate tags
4. **Let AI help** — Enable auto-tagging for new bookmarks
