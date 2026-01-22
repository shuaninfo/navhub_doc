---
title: Search
nav_order: 6
parent: Features
---

# Search

NavHub's search helps you find bookmarks instantly. From simple keyword search to AI-powered natural language queries.

## Quick Search

### Opening Search

Multiple ways to access search:

- Press `/` anywhere in NavHub
- Click the search bar
- Press `Ctrl+K` (Windows) or `Cmd+K` (Mac)

### Basic Search

Type keywords to search:

- **Title** — Matches bookmark titles
- **URL** — Matches domains and paths
- **Description** — Matches bookmark descriptions

Results appear instantly as you type.

## Search Syntax

### Tag Filter

Find bookmarks with specific tags:

```
#design          → All bookmarks tagged "design"
#react #tutorial → Tagged with both "react" AND "tutorial"
```

### Folder Filter

Find bookmarks in specific folders:

```
folder:Work       → Bookmarks in "Work" folder
folder:"Side Projects" → Use quotes for spaces
```

### Domain Filter

Find bookmarks from specific sites:

```
site:github.com   → All GitHub bookmarks
site:youtube.com  → All YouTube bookmarks
```

### Date Filter

Find bookmarks by when they were saved:

```
saved:today       → Saved today
saved:week        → Saved this week
saved:month       → Saved this month
saved:2024-01    → Saved in January 2024
```

### Combining Filters

Combine multiple filters:

```
#design folder:Work site:figma.com
→ Design-tagged bookmarks in Work folder from Figma
```

## Full-Text Search

NavHub indexes page content for deeper search:

- Finds keywords mentioned anywhere in the page
- Not just title and description
- Automatic re-indexing when pages update

**Enable in Settings → Search → Full-text indexing**

## AI Search (Pro)

Use natural language to find bookmarks:

### How It Works

Instead of keywords, describe what you're looking for:

| Query | What It Finds |
|-------|---------------|
| "React performance articles" | Articles about React performance |
| "That recipe I saved last month" | Recent cooking bookmarks |
| "YouTube videos about Python" | Python tutorial videos |
| "News about AI from this week" | Recent AI news articles |

### Enabling AI Search

1. Go to Settings → Search
2. Enable **AI Search**
3. Uses AI tokens from your account

### Tips for AI Search

- Be specific about what you want
- Mention time if relevant ("last week", "recently")
- Include context ("for my project", "about cooking")

## Search Results

### Result Display

Each result shows:

- Thumbnail (if available)
- Title
- URL domain
- Tags
- Match highlight

### Sorting Results

Sort results by:

- **Relevance** — Best matches first (default)
- **Date (newest)** — Most recent first
- **Date (oldest)** — Oldest first
- **Title (A-Z)** — Alphabetical
- **Most visited** — Your most accessed

### Actions on Results

From search results, you can:

- Click to open the bookmark
- Right-click for quick actions
- `Enter` opens first result
- Arrow keys navigate results

## Search History

NavHub remembers your recent searches:

- Last 20 searches saved
- Click to repeat a search
- Clear history in Settings

## Search Widget

Add search to your dashboard:

1. Add the **Search widget**
2. Configure search providers
3. Set default search engine
4. Customize appearance

The search widget can search:
- Your NavHub bookmarks
- Web (via Google, DuckDuckGo, etc.)
- Specific sites
- Custom search endpoints

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `/` | Open search |
| `Esc` | Close search |
| `Enter` | Open selected result |
| `↑` `↓` | Navigate results |
| `Ctrl+Enter` | Open in new tab |
| `Tab` | Cycle through filters |

## Tips

1. **Start with `/`** — It's the fastest way
2. **Use tags for precision** — `#` filters are exact
3. **Try AI search** — When keywords don't work
4. **Build search habits** — Consistent tags = better results
