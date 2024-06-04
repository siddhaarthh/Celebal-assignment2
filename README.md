# To-Do List Application

This is a simple, minimalist To-Do List application built with React and styled using Tailwind CSS. It allows you to add, remove, and mark tasks as completed, with your tasks saved in the browser's local storage for persistence across sessions.

## Features

- Add new tasks
- Remove existing tasks
- Mark tasks as completed or active
- Filter tasks by all, active, or completed
- Persist tasks using local storage

## Getting Started

Follow these steps to set up and run the project locally.

### Prerequisites

- Node.js and npm installed on your machine

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/avayyyyyyy/Todo-List-Celebal-assignment2
   cd Todo-List-Celebal-assignment2
   ```

2. **Install dependencies**

   Run the following command to install the necessary dependencies:

   ```bash
   npm install
   ```

3. **Set up Tailwind CSS**

   Install Tailwind CSS:

   ```bash
   npm install -D tailwindcss
   npx tailwindcss init
   ```

   Update `tailwind.config.js` with:

   ```js
   /** @type {import('tailwindcss').Config} */
   module.exports = {
     content: ["./src/**/*.{js,jsx,ts,tsx}"],
     theme: {
       extend: {},
     },
     plugins: [],
   };
   ```

   Add Tailwind's directives to `src/index.css`:

   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

### Running the Application

Start the development server with:

```bash
npm start
```

This will launch the application in your default web browser. You should see the To-Do List interface where you can start adding your tasks.

## Usage

### Adding a Task

1. Enter a task description in the input field.
2. Click the "Add Task" button.

### Removing a Task

1. Click the "Remove" button next to the task you want to delete.

### Marking a Task as Completed

1. Click the "Complete" button next to the task you want to mark as completed.
2. To mark a completed task as active again, click the "Undo" button.

### Filtering Tasks

1. Click the "All" button to see all tasks.
2. Click the "Active" button to see only active (not completed) tasks.
3. Click the "Completed" button to see only completed tasks.

### Persistence

Your tasks are automatically saved to your browser's local storage. This means you can close the browser or refresh the page, and your tasks will
