<p align="center">
  <img src="assets/icon128.png" alt="Bookmark Keep logo" width="96" />
</p>

# Bookmark Keep

Bookmark Keep is a Chrome, Firefox, and Edge side panel extension for organizing and finding bookmarks faster.

### Chrome

[![Chrome Users](https://img.shields.io/chrome-web-store/users/fblbobhgdajahefnbkpbdeienmpnhado)](https://chromewebstore.google.com/detail/bookmark-keep/fblbobhgdajahefnbkpbdeienmpnhado)
[![Chrome Rating](https://img.shields.io/chrome-web-store/rating/fblbobhgdajahefnbkpbdeienmpnhado)](https://chromewebstore.google.com/detail/bookmark-keep/fblbobhgdajahefnbkpbdeienmpnhado)
[![Chrome Version](https://img.shields.io/chrome-web-store/v/fblbobhgdajahefnbkpbdeienmpnhado)](https://chromewebstore.google.com/detail/bookmark-keep/fblbobhgdajahefnbkpbdeienmpnhado)

### Firefox

[![Firefox Downloads](https://img.shields.io/amo/dw/bookmark-keep)](https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep/)
[![Firefox Users](https://img.shields.io/amo/users/bookmark-keep)](https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep/)
[![Firefox Version](https://img.shields.io/amo/v/bookmark-keep)](https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep/)

### Edge

[![Edge Listing](https://img.shields.io/badge/Edge-Coming%20Soon-0078D7?logo=microsoftedge&logoColor=white)](https://microsoftedge.microsoft.com/addons/detail/bookmark-keep/ijdbpjibkibglmodalmcgclicblemkbh)

## Feature Highlights

- Full bookmark tree with fast expand/collapse controls
- Live search with highlights, wildcard support (`*`), and query shortcuts
- Filters and views (duplicates, empty folders, newest/oldest, domain view)
- Tags with quick tagging workflows and tag-based search
- Multi-select with bulk actions (open, move, tag, delete)
- Drag and drop reordering, including cross-folder moves
- Smart drop suggestions for where new URLs should be saved & rule-based logic
- Light and dark appearance modes with localized UI

## Privacy

- No browsing-history API permission required
- No page-content access required
- No third-party API calls required

## Detailed Feature Breakdown

### Bookmark Tree & Organization

- Full hierarchical bookmark tree in the browser sidebar
- Expand/collapse individual folders plus one-click collapse/expand all
- Recursive bookmark/folder stats badges (optional via settings)
- Pin folders to the top of their parent folder for quicker access
- Context menu on every item (`Edit`, `Move`, `Open`, `Sort`, `Duplicate folder`, `Delete`, etc.)
- Folder sorting tools:
  - Sort folders A-Z / Z-A
  - Sort bookmarks A-Z / Z-A / newest / oldest
  - Optional recursive bookmark sorting across subfolders

### Search, Query Syntax & Autocomplete

- Live search across title and URL
- Highlighted text matches
- Wildcard support (`*`) in text/domain/tag matching
- Fuzzy-match fallback when direct matching is weak
- Search command autocomplete with `>` prefixes for:
  - `is` filters
  - `filter` commands
  - `view` commands
- Built-in query aliases (localized) such as:
  - `>is:duplicate-url`, `>is:duplicate-title`
  - `>is:empty`, `>is:untitled`, `>is:nested`, `>is:tagged`, `>is:untagged`
  - `>filter:domain`
  - `>view:domain`, `>view:domain-most`, `>view:newest`, etc.
  - `>tag:<name>` and `>-tag:<name>` (include/exclude tag terms)

### Filters & Views (Non-Destructive)

- Filters:
  - Duplicate URLs
  - Duplicate titles
  - Tagged bookmarks
  - Empty folders
  - Untitled bookmarks
  - Deeply nested folders (3+ levels)
  - Domain filter
- Views:
  - By domain
  - By domain (most bookmarks first)
  - By newest
  - By oldest
  - Follow current tab domain
  - Sorted folders only
  - Sorted folders + bookmarks
  - Privacy mode (blurs titles/URLs in the sidebar)
- View/filter state is applied without rewriting bookmark data

### Tags

- Create, edit, and delete tags
- Optional color-only tags or name + color tags
- Attach/detach tags for single or multi-selected bookmarks
- Filter/search using tag query syntax (`>tag:`, `>-tag:`, `>is:tagged`, `>is:untagged`)
- Context menu quick-tagging with recently used tags:
  - Up to 3 recent tags shown inline
  - Click to toggle on/off for the current bookmark (or current selection)
  - Long labels are truncated safely in menus

### Multi-Select & Bulk Actions

- Checkbox multi-select across bookmarks
- Shift-click range selection
- Bulk open in tabs/windows/tab groups/incognito (with safety confirmation)
- Bulk move
- Bulk tag
- Bulk delete with count confirmation

### Tabs & Tab Groups Integration

- Sidebar `Tabs` section with collapsible buckets:
  - Pinned tabs
  - Tab groups
  - Open tabs
- Click tab rows to focus the existing tab/window
- Tab and tab-group row context menus support bookmarking/closing selections
- Tab group actions:
  - Save tab group as a new bookmark folder
  - Save tab group into an existing folder
  - Copy all URLs
  - Close the group (with confirmation)
- Toolbar actions for:
  - Bookmark all open tabs
  - Bookmark pinned tabs

### Drag & Drop

- Drag bookmarks/folders to reorder or move between folders
- Multi-item drag with count ghost
- Drop zones above/below/inside with visual indicators
- Drag external URLs into folders to bookmark immediately
- Drag bookmarks to Smart Drop Zone for suggestion-based placement

### Smart Drop Zone & Bookmark Rules

- Drop URL(s) to get ranked folder suggestions
- Ranking signals include:
  - Exact URL matches
  - Same-domain bookmark density
  - Folder keyword relevance
  - Learned behavior from prior saves
  - Recent save destinations
- Confidence labels and “why this folder” explanations
- One-click “save with rule” for domain routing
- Bookmark rules management UI:
  - Match types: domain equals, URL contains, title equals, title contains
  - Set target folder
  - Optional tags to auto-apply
  - Auto-save behavior
  - Enable/disable, reorder, edit, delete bookmark rules

### Recently Added

- Dedicated “Recently Added” section with favicon, relative time, and folder path
- Click path to jump to the bookmark in-tree
- Configurable recent count (10 / 25 / 50 / 100)

### Keyboard & Safety

- Keyboard navigation:
  - `ArrowUp` / `ArrowDown` to move focus
  - `ArrowRight` / `ArrowLeft` to expand/collapse or navigate parent/child
  - `Enter` to open bookmark or toggle folder
  - `Delete` / `Backspace` for selected-item deletion
- Mouse modifiers for open behavior:
  - `Cmd/Ctrl+Click` opens in new tab
  - `Shift+Click` opens in new window (or tab fallback)
- Large-open confirmation threshold (configurable)
- Confirmations for destructive operations (delete, close group, etc.)

### Runtime Behavior

- Reacts to external bookmark changes (create/remove/update/move)
- Reacts to tab/tab-group lifecycle changes in near real time
- Works without third-party network APIs or page-content access

## Detailed Options

### Views

| View option                          | What it does                                                         | Search shortcut        |
| ------------------------------------ | -------------------------------------------------------------------- | ---------------------- |
| `View by Domain`                     | Groups bookmarks by website domain.                                  | `>view:domain`         |
| `View by Domain (Most Bookmarks)`    | Groups by domain and sorts groups by bookmark count (highest first). | `>view:domain-most`    |
| `View by Sorted Folder`              | Sorts folders alphabetically, keeps bookmark order.                  | `>view:sorted-folders` |
| `View by Sorted Folders & Bookmarks` | Sorts folders and bookmarks A-Z inside each folder.                  | `>view:sorted-all`     |
| `View by Newest`                     | Shows bookmarks from newest to oldest.                               | `>view:newest`         |
| `View by Oldest`                     | Shows bookmarks from oldest to newest.                               | `>view:oldest`         |
| `Follow Current Tab`                 | Shows bookmarks matching the active tab domain.                      | `>view:follow-tab`     |
| `Privacy Mode`                       | Blurs titles and URLs in the sidebar.                                | `>view:privacy`        |

### Filters

| Filter option           | What it does                                  | Search shortcut                        |
| ----------------------- | --------------------------------------------- | -------------------------------------- |
| `Find duplicate URLs`   | Bookmarks that share the same URL.            | `>is:duplicate-url`                    |
| `Find duplicate titles` | Bookmarks that share the same title.          | `>is:duplicate-title`                  |
| `Tagged bookmarks`      | Bookmarks that have at least one tag.         | `>is:tagged`                           |
| `Filter by domain`      | Prefills `domain:` and supports wildcard `*`. | `>filter:domain` then a domain pattern |
| `Empty folders`         | Folders with no bookmarks inside.             | `>is:empty`                            |
| `Untitled bookmarks`    | Bookmarks with no title set.                  | `>is:untitled`                         |
| `Deeply nested`         | Folders buried 3+ levels deep.                | `>is:nested`                           |

### Settings Options

#### Features

| Setting                | What it does                                                                 | Values                  | Default |
| ---------------------- | ---------------------------------------------------------------------------- | ----------------------- | ------- |
| `Tabs`                 | Shows or hides the tabs section in the sidebar.                              | On / Off                | Off     |
| `Pinned Tabs`          | Shows or hides pinned tabs in the tabs section.                              | On / Off                | Off     |
| `Grouped Tabs`         | Shows or hides tab groups in the tabs section (Chrome only).                 | On / Off (Chrome only)  | Off     |
| `Open Tabs`            | Shows or hides regular open tabs in the tabs section.                        | On / Off                | Off     |
| `Recently Added`       | Shows or hides the Recently Added bookmarks section.                         | On / Off                | On      |
| `Recently added count` | Controls how many recent bookmarks are shown when Recently Added is enabled. | `10`, `25`, `50`, `100` | `10`    |
| `Drop zone`            | Shows or hides the drop target used for URL auto-suggest save flows.         | On / Off                | On      |
| `Show Counts`          | Shows or hides bookmark and folder counts in lists.                          | On / Off                | On      |

#### Look & Feel

| Setting                    | What it does                                                                   | Values                                                                                                                           | Default                |
| -------------------------- | ------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- | ---------------------- |
| `Language`                 | Overrides the extension UI language independently of browser language.         | `Use browser language` or one of: `de`, `en_CA`, `en_US`, `es`, `fr`, `fr_CA`, `it`, `ja`, `ko`, `nl`, `pt_BR`, `zh_CN`, `zh_TW` | `Use browser language` |
| `Appearance`               | Chooses whether the extension follows system colors or forces light/dark mode. | `System`, `Light`, `Dark`                                                                                                        | `System`               |
| `Theme`                    | Changes bookmark/folder icon styling set.                                      | `Default`, `Classic`, `Bookmark Keep`                                                                                            | `Default`              |
| `Density`                  | Adjusts list spacing and compactness.                                          | `Default`, `Comfortable`, `Compact`                                                                                              | `Default`              |
| `Sync with tab zoom`       | Matches sidebar text size to the active tab zoom level.                        | On / Off                                                                                                                         | On                     |
| `Auto-close in fullscreen` | Automatically closes the sidebar when a page enters fullscreen mode.           | On / Off                                                                                                                         | On                     |

#### Other

| Setting                           | What it does                                                           | Values                                   | Default |
| --------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------- | ------- |
| `Large open warning`              | Sets the confirmation threshold before opening many bookmarks at once. | `5`, `10`, `25`, `50`, `100` bookmarks   | `5`     |
| `Reset info and warning messages` | Re-shows previously dismissed informational/warning notices.           | Button action (resets dismissed notices) | N/A     |

## Screenshots

### Overview

| Light                                                           | Dark                                                          |
| --------------------------------------------------------------- | ------------------------------------------------------------- |
| ![Bookmark Keep light mode](assets/screenshots/en_US/light.png) | ![Bookmark Keep dark mode](assets/screenshots/en_US/dark.png) |

### Feature Gallery

| Tree                                                  | Filters                                                | Views                                              |
| ----------------------------------------------------- | ------------------------------------------------------ | -------------------------------------------------- |
| ![Tree view](assets/screenshots/en_US/light/tree.gif) | ![Filters](assets/screenshots/en_US/light/filters.png) | ![Views](assets/screenshots/en_US/light/views.png) |

| Manage Tags                                                    | Manage Rules                                                     |
| -------------------------------------------------------------- | ---------------------------------------------------------------- |
| ![Manage tags](assets/screenshots/en_US/light/manage-tags.png) | ![Manage rules](assets/screenshots/en_US/light/manage-rules.png) |

## Locales

- 🇺🇸 English (`en_US`)
- 🇨🇦 English (`en_CA`)
- 🇩🇪 Deutsch (`de`)
- 🇪🇸 Español (`es`)
- 🇫🇷 Français (`fr`)
- 🇨🇦 Français (`fr_CA`)
- 🇮🇹 Italiano (`it`)
- 🇯🇵 日本語 (`ja`)
- 🇰🇷 한국어 (`ko`)
- 🇳🇱 Nederlands (`nl`)
- 🇧🇷 Português (`pt_BR`)
- 🇨🇳 简体中文 (`zh_CN`)
- 🇹🇼 繁體中文 (`zh_TW`)

## Report A Bug

Open an issue here:

- https://github.com/bookmarkkeep/bookmarkkeep-issues/issues

When filing, include:

- Browser (`Chrome`, `Edge`, or `Firefox`) and version
- Extension version
- OS
- Reproduction steps
- Expected vs actual behavior
- Screenshot/screen recording when possible

## Useful Links

- Website: https://bookmarkkeep.app
- Chrome Web Store listing: https://chromewebstore.google.com/detail/bookmark-keep/fblbobhgdajahefnbkpbdeienmpnhado
- Firefox Add-ons listing: https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep
- Edge Add-ons listing: https://microsoftedge.microsoft.com/addons/detail/bookmark-keep/ijdbpjibkibglmodalmcgclicblemkbh
