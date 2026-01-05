# React-like State Diffing & Reconciliation — Demo

A tiny, self-contained todo app that demonstrates manual state diffing and DOM reconciliation using plain JavaScript. The demo lives in [index.html](index.html).

## Features

- Simple todo list UI implemented with direct DOM manipulation.
- Naive diffing between `oldTodoState` and the new state to detect added, deleted, and updated items.
- Demonstrates how a reconciliation step can minimize DOM updates.

## How it works (brief)

- The page keeps two arrays: the current `todoState` and the previous `oldTodoState`.
- `updateState(newTodos)` computes added, deleted and updated items by comparing IDs and serializing objects to detect changes.
- For each change it calls small DOM helper functions: add, remove, or update a todo element.

## Usage

1. Open [index.html](index.html) directly in your browser.
2. Or serve the folder and visit the page (recommended for some browsers):

```bash
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```


## License

- MIT — feel free to reuse for learning or demos.
