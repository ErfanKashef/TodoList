# Mini Task Manager

A lightweight and responsive **Task Management App** built with **Next.js 13 (App Router)** and **shadcn/ui**, featuring **Dark/Light theme**, **Dialog-based task addition**, **Search**, **Filter**, and **LocalStorage persistence**.

## Features

- **Add Task via Dialog**: Add tasks with title and priority selection
- **Inline Validation**: Displays a red error message if the title is empty
- **Toggle Task**: Mark tasks as completed or not completed
- **Delete Task**: Remove tasks easily
- **Priority Sorting**: Tasks sorted by priority (High > Medium > Low) and completion status
- **Search Tasks**: Filter tasks by title
- **Filter Tasks**: Show All / Active / Completed tasks
- **Dark/Light Mode**: Toggle theme with intuitive icons (Sun/Moon)
- **LocalStorage**: Automatically saves tasks to persist after page reload
- **Responsive UI**: Modern and clean interface with Tailwind CSS

## Requirements

- Node.js 18+
- **pnpm** (or npm)
- Next.js 13+

## Installation

1. Clone the repository:

```bash
git clone <your-repo-url>
cd <your-project-folder>
```

2. Install dependencies:

```bash
pnpm install
```

3. Start the development server:

```bash
pnpm dev
```
## The app will run on http://localhost:3000.

4. Project Structure
app/
  layout.tsx          ← ThemeProvider for Dark/Light mode
  page.tsx            ← Parent component: manages state, search, filter, theme toggle, localStorage
components/
  AddTaskDialog.tsx   ← Dialog for adding tasks with validation
  TaskList.tsx        ← Renders task list with sorting and toggle/delete functionality
  TaskItem.tsx        ← Individual task item with toggle, delete, and priority badge
  ThemeToggle.tsx     ← Dark/Light theme toggle button with icon
types/
  task.ts             ← Type definitions for Task and Priority

5. How to Use
## 1.Click Add Task → Dialog opens
## 2.Enter task title and select priority
## 3.Click Add Task or press Enter
## 4.If the title is empty, a red error message is displayed
## 5.Toggle tasks as completed or delete tasks as needed
## 6.Use the search input to filter tasks by title
## 7.Use the All / Active / Completed buttons to filter tasks
## 8.Click the Dark/Light toggle button to switch themes

6. Technical Notes

## All interactive components use use "client"
## State is managed at the page.tsx level to reduce unnecessary re-renders
## LocalStorage is used for task persistence
## shadcn/ui + Tailwind CSS for a modern, responsive, dark-mode-ready interface
## Inline validation avoids browser alerts, showing errors directly under the input

# TodoList
