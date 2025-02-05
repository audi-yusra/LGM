# WEB TASK 1

# Todo List Web Application

This project is a **Todo List** web application built using **HTML**, **CSS**, and **JavaScript**. It allows users to add, edit, delete, and manage their tasks efficiently. The application also includes a **theme switcher** to customize the appearance and stores todos and themes in **local storage** for persistence across sessions.

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Requirements](#requirements)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Code Explanation](#code-explanation)
7. [Screenshots](#screenshots)
8. [License](#license)

---

## Introduction

The **Todo List** application is a simple yet powerful tool for managing tasks. It provides a clean and intuitive interface for adding, editing, and deleting tasks. The application also includes a **theme switcher** that allows users to choose from multiple themes to personalize their experience. Todos and themes are stored in **local storage**, ensuring that data persists even after the browser is closed.

---

## Features

- **Add Todos**: Add new tasks to the list.
- **Edit Todos**: Update existing tasks.
- **Delete Todos**: Remove tasks from the list.
- **Delete All Todos**: Clear the entire list with one click.
- **Theme Switcher**: Choose from multiple themes to customize the appearance.
- **Local Storage**: Todos and themes are saved in the browser's local storage for persistence.
- **Responsive Design**: Works seamlessly on both desktop and mobile devices.

---

## Requirements

- A modern web browser (Chrome, Firefox, Safari, Edge, etc.).
- No additional installations are required as the application runs entirely in the browser.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/todo-list.git
   cd todo-list
   ```

2. Open the `index.html` file in your browser:
   ```bash
   open index.html
   ```

---

## Usage

1. Open the application in your browser.
2. Use the following features:
   - **Add a Todo**: Type a task in the input field and press `Enter` or click the `+` button.
   - **Edit a Todo**: Click the edit button (pencil icon) next to a task, update the task, and click the checkmark button to save.
   - **Delete a Todo**: Click the delete button (trash icon) next to a task.
   - **Delete All Todos**: Click the "Delete All" button to clear the entire list.
   - **Change Theme**: Click the palette icon in the top-right corner and select a theme from the dropdown.

---

## Code Explanation

### Key Components

1. **HTML Structure**:
   - The `index.html` file defines the structure of the Todo List, including the input field, buttons, and task list.

   ```html
   <div class="container">
       <header>
           <h1>Todo List</h1>
           <div class="input-section">
               <input type="text" placeholder="Add a todo . . ." />
               <button class="btn btn-secondary add-task-button">
                   <i class="bx bx-plus bx-sm"></i>
               </button>
           </div>
       </header>
       <ul class="todos-list"></ul>
   </div>
   ```

2. **CSS Styling**:
   - The `style.css` file provides the styling for the Todo List, including layout, colors, and animations.

   ```css
   .container {
       background: rgba(255, 255, 255, 0.15);
       box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.3);
       backdrop-filter: blur(3px);
       border-radius: 10px;
       padding: 20px;
   }
   ```

3. **JavaScript Functionality**:
   - The `main.js` file handles the logic for adding, editing, deleting, and managing todos.

   ```javascript
   function addToDo(task_input) {
       let task = {
           id: getRandomId(),
           task: task_input.value,
           completed: false
       }
       todos.push(task);
   }
   ```

4. **Theme Switcher**:
   - The `theme_switcher.js` file allows users to switch between different themes and saves the selected theme in local storage.

   ```javascript
   themes.forEach(theme => {
       theme.addEventListener('click', () => {
           const theme_name = theme.getAttribute('theme');
           html.setAttribute('data-theme', theme_name);
           saveTheme(theme_name);
       });
   });
   ```

---
