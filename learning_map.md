# Project Leaf Learning Map

A step-by-step roadmap to learn the technologies needed to build **Project Leaf**: a local-first, privacy-focused EPUB reader.

---

## Phase 0: Set Up Your Workshop (1 day)

Install:

- Rust (`rustup`)
- Visual Studio Code
- Git
- Node.js LTS
- Tauri prerequisites

Initialize your repository:

```bash
git init project-leaf
```

---

## Phase 1: Learn Enough Rust (3–5 days)

Learn:

- Variables
- Functions
- Structs
- Enums
- `Option<T>`
- `Result<T, E>`
- `match`
- Ownership and borrowing
- Reading and writing files

Resource:

- **The Rust Book** (Chapters 1–8)

Mini exercises:

- Read a file
- Copy a file
- Parse JSON
- Store data in a struct

Goal:

> Build tiny CLI tools comfortably.

---

## Phase 2: Learn Tauri Basics (2–3 days)

Learn:

- Project structure
- `src-tauri/`
- Commands (`#[tauri::command]`)
- Permissions
- Build process

Goal:

> Click button → Rust function runs → returns text

---

## Phase 3: Learn Frontend Basics (3–4 days)

Learn:

### HTML

- Layout
- Buttons
- Forms

### CSS

- Flexbox
- Grid
- Spacing
- Typography
- Dark mode

### TypeScript

- Variables
- Functions
- Interfaces
- Async/await
- Event listeners

Optional:

- Learn **Svelte**

---

## Phase 4: EPUB Rendering

Integrate:

- `epub.js`

Learn:

- Load a book
- Render chapters
- Navigate pages
- Track current location

Goal:

> Import an EPUB and display chapter 1

---

## Phase 5: Library Management

Learn:

- App data storage
- File copying
- Metadata extraction
- Generate IDs
- Track file paths

Store:

- Books
- Covers
- Metadata

---

## Phase 6: SQLite

Use:

- `rusqlite`

Learn:

- Create tables
- Insert records
- Query records
- Update records

Store:

- Books
- Reading progress
- Settings

---

## Phase 7: Highlights + Notes

Learn:

- Text selection in `epub.js`
- EPUB CFI (Canonical Fragment Identifier)
- Saving highlight anchors

Store:

- Highlight text
- Position
- Notes
- Timestamps

---

## Phase 8: Sync (Later)

Start simple:

- Sync app folder using **Syncthing**

Avoid:

- Building custom networking immediately

Goal:

> Private sync without server complexity

---

# First Week Goal

Build this:

```text
Create Tauri app
→ Add file picker
→ Select EPUB
→ Load with epub.js
→ Show book on screen
```

Once this works:

> **Project Leaf officially exists.**
