##  Description
This project implements a simplified web browser history system in C.
The browser supports multiple tabs and page navigation using a circular
doubly linked list (with sentinel) and stacks for history management.

##  Data Structures
- **Page** – contains ID, URL (max 50 chars), and dynamically allocated description
- **Tab** – contains ID, pointer to current page, BACKWARD stack, FORWARD stack
- **Browser** – circular doubly linked list of tabs + pointer to current tab

##  Supported Commands
- `NEW_TAB` – create and switch to a new tab
- `CLOSE` – close current tab (except tab 0)
- `OPEN <ID>` – switch to a specific tab
- `NEXT` / `PREV` – navigate between tabs
- `PAGE <ID>` – open a page in current tab
- `BACKWARD` / `FORWARD` – navigate page history
- `PRINT` – display tab IDs and current page description
- `PRINT_HISTORY <ID>` – display full history of a tab
