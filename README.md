# Notes App (HTML, CSS & JavaScript)

A simple notes app built with **vanilla JavaScript**. Create notes, edit them directly on the page, delete them with one click, and your notes are saved in the browser with `localStorage`, so they are still there after a refresh. **No backend, no database, no framework.**

🔗 **Live Demo:** https://muhammaduzairkhalid15.github.io/Notes-App-JavaScript-LocalStorage-Uzi-Solutions/
💻 **Repository:** https://github.com/MuhammadUzairKhalid15/Notes-App-JavaScript-LocalStorage-Uzi-Solutions

> ⭐ If this helped you, a star on the repo means a lot!

## ✨ Features

- ➕ Create a new note with one click
- ✏️ Edit notes directly on the page (`contenteditable`)
- 🗑️ Delete a note with the trash icon
- 💾 Notes are saved automatically in `localStorage` and survive page refreshes
- ⏎ Pressing Enter adds a line break inside a note
- 🎨 Clean purple-to-blue gradient UI

> Note: notes are stored only in your own browser. Clearing the browser data or switching browsers will remove them.

## 🔧 Built With

- **HTML5**
- **CSS3**: flexbox, gradients
- **JavaScript (vanilla)**: DOM manipulation, event delegation, `localStorage`

## 📂 Project Structure

```
Notes-App-JavaScript-LocalStorage-Uzi-Solutions/
├── index.html
├── style.css
├── script.js
└── images/
    ├── notes.png
    ├── edit.png
    └── delete.png
```

## 🚀 Getting Started

1. Clone the repository
   ```
   git clone https://github.com/MuhammadUzairKhalid15/Notes-App-JavaScript-LocalStorage-Uzi-Solutions.git
   ```
2. Open `index.html` in your browser and click **Create Notes**.

## 🧠 How Saving Works

```js
function updateStorage() {
    localStorage.setItem("notes", notesContainer.innerHTML);
}
```

The whole notes container is saved as HTML. On page load, `showNotes()` reads it back and puts it on the page.

## 💡 What I Practiced

- Making any element editable with `contenteditable`
- Saving and loading data with `localStorage`
- Creating elements with `createElement` and `appendChild`
- Event delegation: one click listener on the container handles every delete icon
- Handling keyboard events

## 🔜 Next Steps

- Save on every `input` event instead of `keyup`
- Only override Enter inside notes, so keyboard users can press Enter on the Create button
- Store notes as JSON instead of raw HTML
- Add timestamps, search and note colors

## 🙌 Credits

Based on the Notes App tutorial by GreatStack, rebuilt for practice.

## 📬 Feedback

Suggestions are welcome. Open an issue or reach out on LinkedIn!
