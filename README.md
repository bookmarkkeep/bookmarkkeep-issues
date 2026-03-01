<p align="center">
  <img src="assets/icon128.png" alt="Bookmark Keep logo" width="96" />
</p>

# Bookmark Keep

Bookmark Keep is a Firefox & Chrome side panel extension for organizing and finding bookmarks faster.

[![Chrome Users](https://img.shields.io/chrome-web-store/users/STORE_ID)](https://chromewebstore.google.com/detail/STORE_ID)
[![Chrome Rating](https://img.shields.io/chrome-web-store/rating/STORE_ID)](https://chromewebstore.google.com/detail/STORE_ID)
[![Chrome Version](https://img.shields.io/chrome-web-store/v/STORE_ID)](https://chromewebstore.google.com/detail/STORE_ID)

[![Firefox Downloads](https://img.shields.io/amo/dw/bookmark-keep)](https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep/)
[![Firefox Users](https://img.shields.io/amo/users/bookmark-keep)](https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep/)
[![Firefox Version](https://img.shields.io/amo/v/bookmark-keep)](https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep/)

## Privacy

- No browsing-history API permission required
- No page-content access required
- No third-party API calls required

## Feature Highlights

- Full bookmark tree with fast expand/collapse controls
- Live search with highlights, wildcard support (`*`), and query shortcuts
- Filters and views (duplicates, empty folders, newest/oldest, domain view)
- Tags with quick tagging workflows and tag-based search
- Multi-select with bulk actions (open, move, tag, delete)
- Drag and drop reordering, including cross-folder moves
- Smart drop suggestions for where new URLs should be saved & rule-based logic
- Light and dark appearance modes with localized UI

## Detailed Options

### Views

| View option                          | What it does                                                         | Search shortcut                                |
| ------------------------------------ | -------------------------------------------------------------------- | ---------------------------------------------- |
| `View by Domain`                     | Groups bookmarks by website domain.                                  | `>view:domain`                                 |
| `View by Domain (Most Bookmarks)`    | Groups by domain and sorts groups by bookmark count (highest first). | `>view:domain-most`                            |
| `View by Sorted Folder`              | Sorts folders alphabetically, keeps bookmark order.                  | `>view:sorted-folders`                         |
| `View by Sorted Folders & Bookmarks` | Sorts folders and bookmarks A-Z inside each folder.                  | `>view:sorted-all`                             |
| `View by Newest`                     | Shows bookmarks from newest to oldest.                               | `>view:newest`                                 |
| `View by Oldest`                     | Shows bookmarks from oldest to newest.                               | `>view:oldest`                                 |
| `Follow Current Tab`                 | Shows bookmarks matching the active tab domain.                      | `>view:follow-tab`                              |
| `Privacy Mode`                       | Blurs titles and URLs in the sidebar.                                | `>view:privacy`                                |

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

| Setting              | What it does                                                                   | Values                                                                                       | Default                |
| -------------------- | ------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- | ---------------------- |
| `Language`           | Overrides the extension UI language independently of browser language.         | `Use browser language` or one of: `de`, `en_CA`, `en_US`, `es`, `fr`, `fr_CA`, `ja`, `pt_BR` | `Use browser language` |
| `Appearance`         | Chooses whether the extension follows system colors or forces light/dark mode. | `System`, `Light`, `Dark`                                                                    | `System`               |
| `Theme`              | Changes bookmark/folder icon styling set.                                      | `Default`, `Classic`, `Bookmark Keep`                                                        | `Default`              |
| `Density`            | Adjusts list spacing and compactness.                                          | `Default`, `Comfortable`, `Compact`                                                          | `Default`              |
| `Sync with tab zoom` | Matches sidebar text size to the active tab zoom level.                        | On / Off                                                                                     | On                     |

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

- en_US
- en_CA
- de
- es
- fr
- fr_CA
- it
- ja
- ko
- nl
- pt_BR
- zh_CN
- zh_TW

## Report A Bug

Open an issue here:

- https://github.com/bookmarkkeep/bookmarkkeep-issues/issues

When filing, include:

- Browser (`Chrome` or `Firefox`) and version
- Extension version
- OS
- Reproduction steps
- Expected vs actual behavior
- Screenshot/screen recording when possible

## Useful Links

- Website: https://bookmarkkeep.app
- Chrome Web Store listing: https://chromewebstore.google.com/
- Firefox Add-ons listing: https://addons.mozilla.org/en-CA/firefox/addon/bookmark-keep
