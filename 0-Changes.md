

# v2
- Date - 7 Nov 26
- AI Used - Claude
#### Changes List
- Notes interlink via id
- Update interlinked note title in both editor and preview, after title updates, only when specific note containing link opens, not full notes library




# v1 a,b,c
- Date - 5 Nov 26
- AI Used - Claude
#### Changes List
- cross x button to delete note on hover, note moves to delete category or box
- Empty notes at homepage with a small guide note always present, on how it works
- Settings button at top bar, when clicked, it opens these buttons under it, with option to choose which buttons stays at top bar or hidden under settings. Also option to remember these settings in export
- After the (Write|Split|Preview) removed the rename, delete, copy option. Moved the the copy option as a button after the undo redo tab
- Delete image by selecting image
- Removed deleted notes count on top of deleted button
- Better cleaner design for number of notes, instead of (1)
- Typing "-" doesnt convert to bullet, fixed
- Search notes link window, added opttion to widen it




# v0 
- Date - 5 Nov 26
- AI Used - Claude
#### Changes List
- Live version started from mockup V1H2
- Started with live notes, indexedDB, notes saving

- - -




### LIVE VERSION ABOVE
### MOCKUP VERSION BELOW







- - -

# v1h
- Date - 17 Oct 26
- AI Used - Claude
#### Changes List
- Added popup gallery image display

- - -

# v1f & v1g
- Date - 16 Oct 26
- AI Used - Claude
#### Changes List
- Read-only nested sidebar, clean title with hover view of all titles
- Updated header strip layout, added sync scroll here, removed from sidebar bottom
- Sort folders A-Z, Z-A added, then moved to bottom sidebar


- - -

# v1e
- Date - 15 Oct 26
- AI Used - Claude
#### Changes List
- Multi Features present

- - -

# v0 
- Date - 15 Oct 26
- AI Used - Claude
#### Changes List
- Initial build from V18 old version and merged of newsnotes and quick markdown under the WebTools

- - -
- - -


# Detailed Features Till V1e
- Date - 15 Oct 26

## Layout and navigation
- A left icon rail, the sidebar and the editor area, in the Tools Hub look with light and dark themes. The theme is shared with the hub.
- **Resizable sidebar (new):** drag its edge between 220px and 480px. The width is remembered, double-click resets it, and the arrow keys nudge it. The library overlay follows the width.
- On phones the sidebar slides in as a drawer.
- **Jump to note:** Ctrl+K opens a quick switcher.
- **Focus mode:** Ctrl+\ hides the surrounding panels.
- **Outline panel** for the current note, and a **"Linked from"** panel showing the notes that link to it.

## Sidebar
- Notes are grouped into category folders. Each folder has a **rounded count pill (new)**, and each note row shows its title and a snippet line.
- Folders and the flat "all notes" view can be switched. Collapse all and expand all are available, and the open and closed state is remembered.
- Search notes by title.

## Library (full table overlay)
- Search plus filter dropdowns with live counts and removable chips: Category, Subcategory, Subcategory 2, Tags, Author, and **Type (new)**.
- Sortable column headers.
- **Column picker (new):** show or hide columns, reorder by dragging or with ▲▼, Reset columns, and the layout is remembered.
- **Default order (new):** Date, Title, Category, Tags, Type, Author, Summary. Subcategory and Subcategory 2 are hidden by default.
- **Summary column (new)**, and a **fixed-width Title (new)** that is cut off with "…" and shows the full title on hover.
- Clicking a row opens the note. Esc or the browser back button closes the library.

## Editing
- Editor, split and preview views, with a draggable divider between editor and preview. The split is remembered, and sync scroll is YAML-aware.
- **Toolbar:** heading, bold, italic, strikethrough, inline code, code block, link, quote, list, table with a size picker, and a `[[ ]]` note link.
  - **New:** Image (URL), Attach image from folder, Horizontal rule and Clear formatting now sit directly in the bar, with no "More" menu.
  - **New:** undo, redo and **+ Tab** are at the right end.
- Undo and redo history, with Ctrl+B and Ctrl+I shortcuts.
- Typing `[[` opens note autocomplete, including a "create new note" option. Links work in the preview.
- Word count and read time, and a save indicator.

## YAML and properties
- Fields: title, summary, date, type, category, subcategory, subcategory2, tags, author, plus **`tabs` and `id` (new)**. Missing keys are added to older notes when they're opened.
- Property pills in the note header, and a warning when the YAML block is missing or invalid.

## Tabs (new)
- A tab bar appears under the header when a note belongs to a set.
- **+ Tab** offers "New note as tab" (it inherits the category) and "Add existing note", which reuses the Ctrl+K picker.
- × removes a tab. The first tab is the owner and can't be removed, and a set dissolves when fewer than two tabs remain.

## Embeds (new)
- A line that is only a YouTube link becomes a click-to-play card with a thumbnail.
- A line that is only an X link becomes a "Load post" card.

## Images (new)
- **Assets folder button** in the top bar. The folder is remembered in Chrome, Edge and Brave, with a small dot when permission is needed again. Other browsers ask you to pick it each session.
- **Attach image** opens a file picker inside the folder, or you can drag images onto the editor.
- **Size and alignment strip:** click an image in the preview to get S, M, L, Full and left, centre, right. The choice is saved in the alt text, and the last size you picked is used for new inserts.
- Images not found in the folder show a dashed "Image not attached" box.

## Export and import (new)
- The Download menu offers **This note (.md)** or **All notes (.zip)**. The zip holds one `.md` per note plus `settings.json` with your column layout.
- Upload accepts `.md` and `.zip`.
- A zip from your own library updates matching notes. A zip from anywhere else is only added, with ids and tab links remapped. A short message reports the result.

## Saved in your browser
Sidebar width, editor split, folder state, flat view, column layout, last image size, the library id and the assets folder.

## Not in v1e
- Notes are kept in memory, so a reload brings back the sample notes. The zip is how you keep your work until real saving is built.
- Images aren't packed into the zip.
- Sub folders, folder move and rename, and drag and drop aren't built.
- The editable library table from News Notes wasn't ported, by your choice.
- The tab bar is still on top. The top versus bottom decision is pending.